# rounded_modal

A custom implementation of `showModalBottomSheet`.

Instead of overriding the entire theme of the app (which caused problems in various parts of my app) as suggested by other solutions on "How to set rounded corners of a modal?", I decided to take a look at the implementation for `showModalBottomSheet` and find the problem myself. 

## Getting Started

Turns out that all that was needed was wrapping the main code for the modal in a Theme widget that contains the `canvasColor: Colors.transparent` trick. I also made it easier to customize the radius and the background color of the modal itself.

```Dart
import 'package:rounded_modal/rounded_modal.dart';

showRoundedModalBottomSheet(
   context: context,
   radius: 10.0,  // This is the default
   color: Colors.white,  // Also default
   builder: (context) => ???,
);
```

For help getting started with Flutter, view our online [documentation](https://flutter.io/).

For help on editing package code, view the [documentation](https://flutter.io/developing-packages/).
