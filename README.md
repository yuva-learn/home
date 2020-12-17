<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Learn Flutter in 30 days](#learn-flutter-in-30-days)
  - [Day 1:](#day-1)
    - [Getting started with the right resources.](#getting-started-with-the-right-resources)
  - [Day 2:](#day-2)
    - [Getting dirty with the code.](#getting-dirty-with-the-code)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Learn Flutter in 30 days
This repository is designed to learn flutter in 30 days. The task are designed in such a way a person with basic programming sense can **self-learn** flutter in 30 days.

 

## Day 1:
### Getting started with the right resources.

A brief overview of what the flutter framework is and what its capabilities are can be found in the links below.
1. [https://flutter.dev/]()
2. [https://medium.com/coding-with-flutter/whats-great-about-flutter-c1b4e44c69ac](https://medium.com/coding-with-flutter/whats-great-about-flutter-c1b4e44c69ac)
3. [https://medium.com/flutterdevs/what-is-flutter-its-benefits-and-limitations-c795c94dfb16](https://medium.com/flutterdevs/what-is-flutter-its-benefits-and-limitations-c795c94dfb16)

## Day 2:
### Getting dirty with the code.

Please use the following url to run your dart code online. [https://dartpad.dev/](https://dartpad.dev/) You can copy paste the following code and run it in the given url.

```dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Welcome to Flutter',
      home: Scaffold(
        appBar: AppBar(
          title: Text('Welcome to Flutter'),
        ),
        body: Center(
          child: Text('Hello World'),
        ),
      ),
    );
  }
}
```
