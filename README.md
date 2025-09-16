# my coding notebook

## table of contents
[Code Definitions](#code_definitions)
[what is flutter?]#what-is-flutter)
[key terms and definintions]
[layout and design widegts]
[definitions with structures]
[code definiontions][notebook style guide]

## flutter notes


### What is flutter?
-definition:
-why is it useful:



| Term | Definition and Description | Base Structure | Real Life Example | App Example |

|------|----------------------------|----------------|-------------------|-------------|

|      | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |  |  | the main function is like pressing ‘play’ and showing the starting screen

|      | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  |  | it defines the rooms, layout, and style before you furnish it.

|      | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |  |  | it gives the basic structure so you can place actors, props, and decorations in the right spots.

|      | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |  |  | Like a stack of books on a shelf—each book is placed on top of the previous one in a straight line.

|      | A widget that shows things side-by-side. | `Row(...)` |  |  | Like people standing in a line holding hands—each person is next to the other in a straight row.

|      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |  |  | Like a gift box: it holds items inside and can be decorated with wrapping paper, ribbons, or a label.

|      | A widget to display text on the screen. | `Text('Hello')` |  |  | Like a sign or label in a store that shows a message to people passing by.

|      | A widget to show an image using a link from the internet. | `Image.network('https://...')` |  |  | Like viewing a photo on Instagram or a website—the app fetches it from the internet and shows it on your screen.

|      | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |  |  | Like a doorbell button—you press it, and it triggers an action (someone rings the bell).

|      Like a doorbell button—you press it, and it triggers an action (someone rings the bell).

|      | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |  |  |

|      | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |  |  |

|      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  |  |

|      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |  |  |

|      | Aligns content in the center of the screen or container. | `Center(child: ...)` |  |  |

|      | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |  |  |

|      | This marks a method as one that’s replacing a method in a parent class. | `@override` |  |  |

|      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |  |

|      | Required in every widget class to describe what to show. | `build` |  |  |

|      | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |

|      | A keyword used to pass a value to the parent widget. | `super.key` |  |  |

|      | A keyword that means the value won't change and is set once. | `const` |  |  |
