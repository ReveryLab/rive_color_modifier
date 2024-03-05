# Rive Color Modifier

This package provides an easy and straightforward way to modify the Color of specific components within [Rive](https://rive.app/) animations at runtime, while also maintaining their opacity (alpha values) throughout the animation.

### If you like this package, please leave a like on [pub.dev](https://pub.dev/packages/rive_color_modifier) and star on [GitHub](https://jsimon.dev/)

## Features

- **RiveColorComponent**: Enables dynamic color application and manipulation within Rive animations, providing a robust toolset for developers to control the color properties effectively.

- **RiveColorModifier**: A focused utility to modify and adjust colors within Rive animations, allowing for precise and detailed color transformations.

## Getting started

To start using this package, add it as a dependency in your `pubspec.yaml` file:

```yaml
dependencies:
  rive_color_modifier: ^1.0.0
```

## Usage

This package allows you to dynamically modify the Color properties of specific components in your Rive Animations. Below is an example demonstrating how to use `RiveColorModifier` along with `RiveColorComponent` to change the color of particular [Shapes](https://help.rive.app/editor/fundamentals/shapes-and-paths) within an animation.

You just have to provide the [Artboard](https://help.rive.app/editor/fundamentals/artboards) of the [Rive](https://rive.app/) asset you are using to the RiveColorModifier, and in the components property, you pass a RiveColorComponent for each Shape you want to change the color of. You also pass the name of the [Fill](https://help.rive.app/editor/fundamentals/fill-and-stroke) or [Stroke](https://help.rive.app/editor/fundamentals/fill-and-stroke) and then the Color you want it to have. Super simple!

```dart
RiveColorModifier(
  artboard: _eyeArtboard,
  components: [
    RiveColorComponent(
      shapeName: 'Eye Pupil Off',
      fillName: 'Pupil Fill',
      color: colors.primary,
    ),
    RiveColorComponent(
      shapeName: 'Eye Border Off',
      strokeName: 'Eye Border Stroke',
      color: colors.primary,
    ),
  ],
)
```

## Additional information

For more information on how to use this package, or if you want to contribute, please visit the [GitHub repository](https://jsimon.dev/). If you encounter any issues or have feature requests, please file them in the issue tracker.

Don't forget to like the package if you find it useful, and if you have any suggestion, please let me know.

Your feedback and contributions are welcome to help improve this package!