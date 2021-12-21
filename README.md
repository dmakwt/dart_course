# Dart
### Part1 - Basic

- main method
```dart
void main() {
  
}
```

- print function
```dart
void main() {
  print('أهلا وسهلا');
}
```

- variables (start with lowercase, Camel case, can't start with @ ! etc, you can start with $)
```dart
void main() {
   String name = 'Dhari';
   String name2 = "Dhari";
   int age = 23;
   double height = 174.5;
   bool likesPizza = true;
    
   print(name);
   print(age);
}
```


- var keyword
```dart
void main() {
   var name = 'Dhari';
   var age = 23;
   var height = 174.5;
   var likesPizza = true;
    
   print(name);
   print(age);
}
```

- EX (1) - (2 min)
```dart
// Create some variables to define my firstName, age, height,      
// then    print these variables;    

// SOL
String firstName = 'Dhari';
int age1 = 23;
double height1 = 174;

print('Name: $firstName, age: $age, height: $height');
```

- String methods - toUpperCase(), toLowerCase()
```dart
void main() {
   String title = 'Flutter course';
   print(title.toUpperCase());
   
  title = title.toLowerCase();
  print(title);
}
```

- String methods - replaceAll()
```dart
void main() {
  String myFood = 'I love pasta';
  print(myFood);
  String myFood2 = myFood.replaceAll('pasta', 'pizza');
  print(myFood2);
}
```

- Arithmatics ( + - * / )
```dart
void main() {
  int x = 10;
  int x2 = 20;
  print(x + x2);

  int x3 = x + 11;
  print(x3);
}
```
- EX (2) - (1 min)
```dart
// Try to guess what's the result for the following
void main() {
  double x = 10;
  x+=2;
  print(x);
  x-=3;
  print(x);
  x*=2;
  print(x);
  x/=3;
  print(x);
}
```

- Convert String to double or int
```dart
void main() {
  String height3 = '170';
  double height4 = 4;
  
  // print(height3 + height4);  -> error
  
  print(double.parse(height3) + height4);
}
```

- Convert int or double to String
```dart
void main() {
  int age = 50;
  String myAge = age.toString();
  print(myAge);
  
  // or
  int age = 50;
  String myAge = '$age';
  print(myAge);
  
}
```
- EX (3) - (4 min)
```dart
void main(){

// Create double tempF  = 80
// convert it from Fahrenheit to Celsius
// formula: (°F − 32) / 1.8 = °C
// result: 80.0F = 26.7C

// SOL
double tempF = 80;
double tempC = (tempF - 32) / 1.8;
print('${tempF.toStringAsFixed(1)}F = ${tempC.toStringAsFixed(1)}C');

}
```

- Operators (== , != , >= , > , <= , <)
```dart
void main(){
  print(10 == 5);
  print(10 != 5);
  print(10 >= 5);
  print(10 > 5);
  print(10 <= 5);
  print(10 < 5);
}
```

- Operators (|| , &&)
```dart
void main(){
  print(10 < 5 || 5 < 7);
  print(10 < 5 && 5 < 7);
}
```

- Operators (!)
```dart
void main(){
  print(!(10 > 5));
}
```

- EX (4) - (1 min)
```dart
void main() {
  // Try to guess what's the result for the following
  
  String email = 'dmakwt@gmail.com';
  print(!(email.contains('@')));
}
```

- Comments
```dart
void main() {
  // Hi
  
  /*
    test
    test
  */
}
```

- {}
```dart
void main() {
  int value1 = 10;
  print('value = $value1');
  // {}
  print('value = ${value1 + 1}');
}
```
- var vs const

```dart
void main() {
  var age = 22;
  print(age);
  
  age = 25;
  print(age);

  const age1 = 22;
  print(age1);
  
  final age2 = 22;
  print(age2);
}
```

- dynamic
```dart
void main() {
  dynamic name2 = 'Dhari';
  print(name2);

  name2 = 20;
  print(name2);
}
```

### Part2 - Conditions

- if condition
```dart
void main() {
  var grade = 80;

  if (grade >= 90) {
    print('A');
  } else if (grade >= 80) {
    print('B');
  } else if (grade >= 70) {
    print('C');
  } else if (grade >= 60) {
    print('D');
  } else {
    print('F');
  }
}
```

- EX (5) - (4 min)
```dart
void main() {
  //  Create var age  = 20
  // أذا أكبر من 60 شايب
  // أذا أكبر من 18 شباب
  // أذا أكبر من 15 مراهق
  // غيره طفل
  
}
```

- switch condition
```dart
void main() {
  var score = 1;
  switch (score) {
    case 1:
      print('Gold');
      break;
    case 2:
      print('Silver');
      break;
    case 3:
      print('Bronze');
      break;
    default:
      print('N/A');
      break;
  }
}
```

### Part3 - Looping

- while
```dart
void main() {
  var i = 1;
  
  while (i <= 3) {
    print(i);
    i++;
  }
}
```

- for loop
```dart
void main() {
   for (var x = 1; x <= 3; x++) {
    print(x);
  }
}
```

### Part4 - List (Array)

- Create List - the index start from zero
```dart
void main() {
  // List colors = ['Blue', 'Orange', 'Green'];
  var colors = ['Blue', 'Orange', 'Green'];
  
  print(colors[0]);
  print(colors[1]);
  print(colors[2]); 
  
  // change the list value
  colors[0] = 'Red';
  print(colors[0]);
}
```

- Using for loop inside List
```dart
void main() {
  var colors = ['Blue', 'Orange', 'Green'];
 
  for (var color in colors) {
    print(color);
  }
}
```

- EX (6) - (5 min)
```dart
void main() {
   // Given this list of integers: [1, 4, 2, 7].
  // Write a program that prints the sum of all these values.
  
  // SOL
  var values = [1, 4, 2, 7];
  var sum = 0;
  for (var value in values) {
    sum = sum + value;
    // sum += value;
  }
  
  print(sum);
}
```

- List properties
```dart
void main() {
  var colors1 = ['Blue', 'Orange', 'Green'];
  
  print(colors1.length);
  print(colors1.isEmpty);
  print(colors1.isNotEmpty);
  print(colors1.first);
  print(colors1.last);
}
```

- List method - add(value)
```dart
void main() {
  var colors2 = ['Blue', 'Orange', 'Green'];
  print(colors2);
  
  colors2.add('Red');
  print(colors2);
}
```

- List method - insert(index, value)
```dart
void main() {
  var colors3 = ['Blue', 'Orange', 'Green'];
  print(colors3);
  colors3.insert(0, 'Red');
  print(colors3);
}
```

- List method - removeAt(index)
```dart
void main() {
  var colors4 = ['Blue', 'Orange', 'Green'];
  print(colors4);
  colors4.removeAt(1);
  print(colors4);
}
```

- List method - clear()
```dart
void main() {
  var colors5 = ['Blue', 'Orange', 'Green'];
  print(colors5);
  colors5.clear();
  print(colors5);
}
```

- List method - contains(value)
```dart
void main() {
  var colors6 = ['Blue', 'Orange', 'Green'];
  print(colors6.contains('Blue'));
}
```

- List method - indexOf(value)
```dart
void main() {
  var colors7 = ['Blue', 'Orange', 'Green'];
  print(colors7.indexOf('Green'));
  print(colors7.indexOf('Red'));
}
```


### Part5 - Map (Object)

- Create Map
```dart
void main() {
//       Map<String, dynamic> person = {
//     'name': 'Dhari',
//     'age': 23,
//     'height': 174,
//   };
  
    var person = {
    'name': 'Dhari',
    'age': 23,
    'height': 174,
  };
  
  // Keys not index
  print(person['name']);
  print(person['age']);
}
```

- Change Map values
```dart
void main() {
  var person = {
    'name': 'Dhari',
    'age': 20,
    'height': 174,
  };
  print(person);

  person['age'] = 23;
  print(person);
}
```

- EX (7) - (4 min)
```dart
void main() {
   // Creat 'Map' car,
  // print 'name: 'Tesla', model: 2021, color: white'
}
```

- Map inside List
```dart
void main() {
    var people = [
    {
      'name': 'Dhari',
      'age': 23,
      'height': 174,
    },
    {
      'name': 'Nasser',
      'age': 27,
      'height': 167,
    }
  ];
  
  for (var person in people) {
    print(person);
  }
}
```

### Part6 - null safety

- null safety
```dart
void main() {
  String value1 = 'abc'; // String
  //  String value1 = null; -> error
  
  String? value2 = null; // null or String

  print(value1);
  print(value2);
}
```

### Part7 - Function
- create function
```dart
void sayHi() {
  print('Hi');
  print('Welcome');
}

void main() {
  sayHi();
  sayHi();
  sayHi();
}
```


- pass values inside function
```dart
void main() {
  // Before
  const name = 'Dhari';
  const age = 23;
  print('My name: $name, and my age: $age');

  const name2 = 'Rashid';
  const age2 = 26;
  print('My name: $name2, and my age: $age2');

  // After
  printBio('Dhari', 23);
  printBio('Rashid', 26);
}

void printBio(String name, int age) {
  print('My name: $name, and my age: $age');
}
```

- return value from function
```dart
void main() {
  String bio = printBio('Dhari', 23);
  print(bio);
}

String printBio(String name, int age) {
  return 'My name: $name, and my age: $age';
}
```

- EX (8) -    (5 min)
```dart
// Write a function called sum that takes a List of values as an
// argument (List<double> values), then return the sum of all values

// SOL
void main() {
  var value = sum([2, 3, 5]);
  print(value);
}

double sum(List<double> values) {
  double sum = 0;

  for (var value in values) {
    sum = sum + value;
//     sum += value;
  }
  return sum;
}

```

- positional argument vs named argument
```dart
void main() {
  // before
//   final bio = printBio('Dhari', 23);
//   print(bio);

  // After
//   final bio = printBio(name: 'Dhari', age:23);
  final bio = printBio(age: 23, name: 'Dhari');
  print(bio);
}

String printBio({required String name, required int age}) {
  return 'My name: $name, and my age: $age';
}
```
- default value
```dart
void main() {
  final bio1 = printBio(name: 'Dhari', age: 23);
  print(bio1);

  final bio2 = printBio(name: 'Dhari');
  print(bio2);

}

String printBio({required String name, int age = 30}) {
  return 'My name: $name, and my age: $age';
}
```


- EX (9) - (5 min)
```dart
// Write a function called add that takes two arguments (int a, int b), then return the 
// sum. The arguments should be positional arguments

// SOL
void main() {
  int value1 = add(num1: 1, num2: 3);
  print(value1);
}

int add({required int num1, required int num2}) {
  return num1 + num2;
}
```

- return value ( => )
```dart
void main() {
  int value2 = add2(num1: 10);
  print(value2);
}

int add2({int num1 = 0, int num2 = 0}) => num1 + num2;
```

### Part8 - Class

- Create Class - (Start with Uppercase) (Blueprint, Object oriented programming)
```dart
class Person {
  String name = '';
  int age = 0;
}

void main() {
  final person1 = Person();
  print(person1.name);
  print(person1.age);

  person1.name = 'Dhari';
  person1.age = 23;
  print(person1.name);
  print(person1.age);

  final person2 = Person();
  person2.name = 'Rashid';
  person2.age = 30;
  print(person2.name);
  print(person2.age);
}
```

- Create method
```dart
class Person {
  String name = '';
  int age = 0;

  void printBio() {
    print('Name: $name, Age: $age');
  }
}

void main() {
  final person1 = Person();
  person1.name = 'Dhari';
  person1.age = 23;
  person1.printBio();

  final person2 = Person();
  person2.name = 'Rashid';
  person2.age = 30;
  person2.printBio();
}

```


- Constructor
```dart
class Person {
  String name = '';
  int age = 0;

  // الكوسنركتر هي عبارة عن فكشن راح اتنفذ قبل لا ينشئ لنا الاوبجكت
  Person(String name, int age) {
    this.name = name;
    this.age = age;
  }

  void printBio() {
    print('Name: $name, Age: $age');
  }
}

void main() {
  // Before
//    final person1 = Person();
//    person1.name = 'Dhari';
//    person1.age = 23;
//    person1.printBio();

  // After
  final person1 = Person('Dhari', 23);
  person1.printBio();
}
```

- Constructor shortcut
```dart
class Person {
  String name = '';
  int age = 0;

  Person(this.name, this.age);

  void printBio() {
    print('Name: $name, Age: $age');
  }
}

void main() {
  // After
  final person1 = Person('Dhari', 23);
  person1.printBio();
}
```

- Named argument
```dart
class Person {
  final String name;
  final int age;

  Person({required this.name, required this.age});

  void printBio() {
    print('Name: $name, Age: $age');
  }
}

void main() {
  final person1 = Person(name: 'Dhari', age: 22);
  person1.printBio();
}
```

- EX (10) - (5 min)
```dart
// Write a class called (Product) with two properties
// 1- name, 2- price
// write one method that print the details
// Ex..   "Name of Product: iPhone, Price: 1300"

class Product {
  final String name;
  final double price;

  Product({required this.name, required this.price});

  void printDetails() {
    print('Name of Product: $name, Price: \$$price');
  }
}

void main() {
  // After
  final iPhone = Product(name: 'iPhone', price: 1300.99);
  iPhone.printDetails();

//   person1.age = 55; error الان المتغير عبارة عن ثابت
}

```



- Flutter widgets
```dart

class Widget {
  void build() {
    print('Build my widget');
  }
}

class Text extends Widget {
  String text;
  TextStyle style;

  Text(this.text, {required this.style});
  
  @override
  void build() {
    print('Text widget: $text');
  }
  
}

class TextStyle {
  String color;
  double fontSize;

  TextStyle({required this.color, required this.fontSize});
}

void main() {
  Widget customText = Text(
    'Hi',
    style: TextStyle(color: 'Red', fontSize: 14),
  );
  
  
  customText.build();
  
}
```




