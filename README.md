Fork of textAngular v1.5.16
===========

This is fork of [textAngular](https://github.com/TwigWorld/textAngular). Forked version removes comment breaking collectstatic's default javascript minification.

In original script, line 1017 of `dist/textAngular.js`:
```
} else /* istanbul ignore next: not tested since identical to blockquote */
if (optionsTagName === 'pre' && taSelection.getStateShiftKey()) {
```

would be minified to:
```
} elseif (optionsTagName === 'pre' && taSelection.getStateShiftKey()) {
```

In case when original Author fixes this in future releses this repo could be abandoned.
