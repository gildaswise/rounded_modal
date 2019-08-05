## [1.0.1] - 2019-08-05

This plugin is now DEPRECATED as you can now do proper borders with the default implementation from `showModalBottomSheet` as follows:

```dart
showModalBottomSheet(
  shape: RoundedRectangleBorder(
     borderRadius: BorderRadius.circular(10.0),
  ),
  backgroundColor: Colors.white,
);
```

## [1.0.0] - 2018-10-12

* Added fix from [@slightfoot](https://gist.github.com/slightfoot/5af4c5dfa52194a3f8577bf83af2e391) that handles the issue of modals hiding the keyboard if any text input is part of its layout

## [0.0.1] - 2018-09-01

* First release for this amazingly simple package
