<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->

# List Major English Words
This package is a dictionary of English words that includes the Major System number and definition for each word.


## Getting started
1) Update 'pubspec.yaml' 'dependencies' to include:
`list_major_english_words: ^1.0.0`
2) Then import into your `your.dart` file like so:  
`import 'package:list_major_english_words/list_major_english_words.dart';`

## Usage

To use, declare a variable. Then access an element, and get it's major number and definition:  

```dart
//GET WORDS
List<Map<String, List<String>>> dicWords = list_major_english_words;
//GET A WORD OBJECT:
Map<String, List<String>> dicObj = dicWords[0];
//GET FIRST OBJECT KEY:
String word = dicObj.keys.toList().first;
//GET MAJOR NUMNBER:
String majorNumber = dicObj[word]?[0];
//GET MAJOR DEFINITION:
String definition = dicObj[word]?[1];
```