# my coding notebook

## table of contents
- [Flutter Notes](#flutter-notes)
  - [what is flutter?](#what-is-flutter)
  - [key terms and definintions]()
  - [layout and design widegts]()
  - [definitions with structures](#definitions-with-structures)
- [Code Definitions](#code-definitions)
- [code definiontions][notebook style guide]

## flutter notes


### What is flutter?
-definition:
-why is it useful:



## definitions with structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|      | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |  the main function is like pressing ‘play’ and showing the starting screen | main.dart void main() => runApp(MyPortfolioApp()); |
|      | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |it defines the rooms, layout, and style before you furnish it.  | return MaterialApp     debugShowCheckedModeBanner: false,     title: 'TSA Portfolio', |
|      | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |it gives the basic structure so you can place actors, props, and decorations in the right spots.  |return Scaffold(     body: Column( |
|      | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` | Like a stack of books on a shelf—each book is placed on top of the previous one in a straight line.  | child: Column(     children: [ |
|      | A widget that shows things side-by-side. | `Row(...)` |  Like people standing in a line holding hands—each person is next to the other in a straight row. |   child: Row( |
|      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |  Like a gift box: it holds items inside and can be decorated with wrapping paper, ribbons, or a label. |  Container(            width: 200,           height: 200, |
|      | A widget to display text on the screen. | `Text('Hello')` | Like a sign or label in a store that shows a message to people passing by. |  const Text(            'HI EVERYONE,\nWelcome to the | 
|      | A widget to show an image using a link from the internet. | `Image.network('https://...')` |  Like viewing a photo on Instagram or a website—the app fetches it from the internet and shows it on your screen. | child: Image.network(url, width: 100, height: 100, fit: BoxFit.cover), |
|      | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` | Like a doorbell button—you press it, and it triggers an action (someone rings the bell). |  ElevatedButton(        onPressed: () => Navigator.pushNamed(context, '/alt'), | 
|      | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` | A stop sign always says “STOP.” |  (context) => const HomeScreen(), |
|      | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |  A digital clock, a like button that toggles, or a shopping cart counter. | class InfoCard extends StatelessWidget { |
|      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` | Like using a GPS with saved addresses: instead of typing the full location each time, you just say “Take me home |  | 
|      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |  Like putting bubble wrap around an item in a box — it creates space so the item isn’t touching the edges. |    onPressed: () => Navigator.pushNamed(context, '/showcase'), |
|      | Aligns content in the center of the screen or container. | `Center(child: ...)` |  Like putting a painting right in the middle of a wall instead of off to the side. |  |
|      | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` | Like words in a paragraph: when you reach the end of the line, the text automatically wraps to the next line. |  child: const Text('Next'), | 
|      | This marks a method as one that’s replacing a method in a parent class. | `@override` | Like following a recipe but deciding to tweak one step — you’re replacing the original instruction with your own. |  |
|      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |Like an architect’s blueprint — it shows exactly what should appear and how it’s arranged.  |  @override
  Widget build(BuildContext context) { |
|      | Required in every widget class to describe what to show. | `build` | Like a blueprint an architect makes before constructing a building—it tells exactly what goes where. | build(BuildContext context) { |
|      | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |Like a GPS or map in a city — it tells you exactly where you are so you can find nearby places or navigate.  | (BuildContext context) { |
|      | A keyword used to pass a value to the parent widget. | `super.key` | Like giving your home address to the postal service so they know exactly where to deliver your mail. |  super.key,
    required this.imageUrl, |
|      | A keyword that means the value won't change and is set once. | `const` | Like a permanent stamp on a document — it cannot be changed once applied. |    const Padding( |











| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|      | A named container used to store a value that may change. | `var x = 5;` |  |  |
|      | A fixed value that cannot change once set. | `const PI = 3.14;` |  |  |
|      | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |  |  |
|      | A sequence of characters used to represent words or text. | `"Hello World"` |  |  |
|      | Whole number values. | `int age = 16;` |  |  |
|      | Number values with decimals. | `double age = 16.2;` |  |  |
|      | A value that can be true or false. | `bool isLoggedIn = false;` |  |  |
|      | A collection of values in a specific order. | `List<String> names = [];` |  |  |
|      | A special value that means “nothing.” | `String? name = null;` |  |  |
|      | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |  |  |
|      | The information passed into a function to change how it works. | `greet(String name)` |  |  |
|      | The result a function gives back. | `return total;` |  |  |
|      | Where a variable or function can be used. | (No set syntax — concept-based) |  |  |
|      | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |  |  |
|      | A specific version of a class. | `Dog myDog = Dog();` |  |  |
|      | A variable that belongs to a class/object. | `String name;` |  |  |
|      | A function that belongs to a class. | `void bark() {}` |  |  |
|      | A special function used to set up a class when it’s created. | `Dog(this.name);` |  |  |
|      | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |  |  |
|      | Changing how a built-in or inherited function behaves. | `@override` |  |  |
|      | A function that does not return a value. | `void printMessage() {}` |  |  |


















