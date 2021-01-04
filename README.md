<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Learn Flutter in 30 days](#learn-flutter-in-30-days)
  - [Day 1:](#day-1)
    - [Getting started with the right resources.](#getting-started-with-the-right-resources)
  - [Day 2:](#day-2)
    - [Getting dirty with the code.](#getting-dirty-with-the-code)
  - [Day 3:](#day-3)
    - [Understanding the diff. between stateless and stateful widgets.](#understanding-the-diff-between-stateless-and-stateful-widgets)
  - [Day 4:](#day-4)
  - [Day 5:](#day-5)
    - [Basics of git](#basics-of-git)
  - [Day 6:](#day-6)
    - [Local installation.](#local-installation)
  - [Day 7:](#day-7)
    - [Route Navigation](#route-navigation)
  - [Day 8](#day-8)
  - [Day 9](#day-9)
  - [Day 10](#day-10)
  - [Day 11](#day-11)
    - [Json Serialization and deserialisation](#json-serialization-and-deserialisation)
  - [Day 12](#day-12)
    - [Git branching.](#git-branching)
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

## Day 3:
### Understanding the diff. between stateless and stateful widgets.

Widgets are the building blocks for constructing UI in flutter. The entire app is treated as a `Widget` and all 'elements' within are extended from `Widget` class as well.
Flutter builds these widgets based on the properties and state variables passed to them.
Here we will try to understand the difference between a `StatelessWidget` and a `StatefulWidget`.

The above example given for [day 2](#day-2) is an example of stateless widget.

The following is an example of `StatefulWidget`.
```dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      home: MyHomePage(title: 'Flutter Demo Home Page'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key key, this.title}) : super(key: key);

  final String title;

  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  int _counter = 0;

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(
        child: Text('You have pushed the button $_counter times.',
            style: TextStyle(fontSize: 20)),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: () {
          setState(() {
            _counter++;
          });
        },
        tooltip: 'Increment',
        child: Icon(Icons.add),
      ),
    );
  }
}
```

[More info about these can be found here](https://flutter.dev/docs/development/ui/interactive)
## Day 4:
Best pratices in programming

## Day 5:
### Basics of git
Basics of git
[https://www.youtube.com/watch?v=SWYqp7iY_Tc](https://www.youtube.com/watch?v=SWYqp7iY_Tc_)

Flutter Navigator. Navigatation to another page
[https://www.youtube.com/watch?v=wH16ROWAtAk](https://www.youtube.com/watch?v=wH16ROWAtAk)


## Day 6:
### Local installation.
Install flutter in local machine and clone the personal repositories.

## Day 7:
### Route Navigation
[Simple Navigation](https://flutter.dev/docs/cookbook/navigation/navigation-basics)

[Navigating using named routes](https://flutter.dev/docs/cookbook/navigation/named-routes)

## Day 8
Troubleshooting with existing code

## Day 9
Making network calls. An example project has been provided
[https://github.com/yuva-learn/eg_network](https://github.com/yuva-learn/eg_network)

## Day 10
Troubleshooting with existing code

## Day 11
### Json Serialization and deserialisation
[https://flutter.dev/docs/development/data-and-backend/json](https://flutter.dev/docs/development/data-and-backend/json)

Have a look at this video tutorial to get an idea of how to convert large dart objects to json easily.
[Flutter json serialization](https://www.youtube.com/watch?v=8fFoLs9qVQA)

## Day 12

### Git branching. 
How to create branches and collaborate.


## Day 13 - 15
### Code Practicing

## Day 16
### Understanding Constraints
[https://flutter.dev/docs/development/ui/layout/constraints](https://flutter.dev/docs/development/ui/layout/constraints)


## Day 17
## UI design task

