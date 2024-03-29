# ToDo App

This isn't really a finished app but more a collection of files teaching me mainly the principles of flutters three trees and keys! This code was produced during the completion of the Flutter course [A Complete Guide to the Flutter SDK & Flutter Framework for building native iOS and Android apps](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/learn/lecture/37130436#overview).


## Topics covered 

- Learned about the three trees (widget tree, element tree, render tree).
- Widget tree is the combination of widgets in the code.
- Element tree is the in memory representation of the widgets. Used to determine required UI updates. -> re-used if possible.
- Render tree is the visible ui building blocks. Updated only when needed via comparison with elment tree. -> UI only partially updated.
- Added code from a [gitHub repo](https://github.com/academind/flutter-complete-guide-course-resources/tree/main/Lecture%20Attachments/07%20Flutter%20Internals/01%20Starting%20Setup/lib) to better understand the trees.
- Learned about better strucutre for flutter apps with extracting widgets into new files and when to call which function to reduce redundent elment checks while going through the trees. Less checks = better performance.
- In addition to the last point: it is good practice to keep the stateful widgets as small as possible.
- Learned more in depth about the usage of keys. Added code from this [gitHub repo](https://github.com/academind/flutter-complete-guide-course-resources/tree/main/Code%20Snapshots/07%20Flutter%20Internals/02%20Refactor%20%26%20Extract%20Widgets/lib/keys) to better understand keys.
- Learned about the way widgets are connected with elements and how the reference can be updated.
- Learned that states are independent from their widgets and connected to the elements. That is why the using the checkableitem without keys breaks the app.
- Learned that flutter checks the reusability of an item based on matching types. If the type od the item and the element is the same than flutter is fine with updating the reference.
- Keys move with the items. Flutter now checks the type and the key and is able to move the keys as well as the states accordingly. In short: it moves the elements.
- Revisited how var, final and const manage memory.