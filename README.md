# Floating Ribbon Util Azul

[![pub package](https://img.shields.io/badge/pub-v1.0.0-blue)](https://pub.dev/packages/floating_ribbon_util_azul) [![Build Status](https://mouadzizi.com)](https://mouadzizi.com) [![LICENSE](https://img.shields.io/badge/license-MIT-green)](https://github.com/azulmouad/floating_ribbon_util_azul/blob/main/LICENSE)

Floating Ribbon Util Azul is an updated Flutter package for creating floating ribbons on images. This version is a copy of the previous package, now enhanced with updates and fixes, ensuring compatibility with the latest Flutter versions.

<p>
    <img src="https://github.com/101Loop/Floating-Ribbon/blob/master/example.gif?raw=true" alt="Floating Ribbon Example"/>
</p>

## Dependency

To include this package in your project, add the following line to your `pubspec.yaml` file:


dependencies:
  floating_ribbon_util_azul: any


## How To Use

> To achieve the shimmering effect, you must also include the `skeleton_text` package in your `pubspec.yaml`:

```yaml
dependencies:
  skeleton_text: any
```

> Below is the code to reproduce the floating ribbon effect:

```dart
import 'package:skeleton_text/skeleton_text.dart';
import 'package:floating_ribbon_util_azul/floating_ribbon_util_azul.dart';

FloatingRibbonUtilAzul(
  height: 85,
  width: 85,
  childHeight: 75,
  childWidth: 75,
  child: Padding(
    padding: const EdgeInsets.all(8.0),
    child: FlutterLogo(),
  ),
  childDecoration: BoxDecoration(color: Colors.grey),
  ribbon: SkeletonAnimation(
    child: Center(
      child: Text(
        'Exclusive',
        style: TextStyle(
          color: Colors.white,
        ),
        textAlign: TextAlign.center,
      ),
    ),
  ),
  shadowHeight: 5,
);
```

## Getting Started

This project serves as a foundation for a Dart [package](https://flutter.dev/developing-packages/)—a library module that facilitates code sharing across multiple Flutter or Dart projects.

For assistance in getting started with Flutter, please refer to our [online documentation](https://flutter.dev/docs), which provides tutorials, sample projects, mobile development guidance, and a comprehensive API reference.

---

```
