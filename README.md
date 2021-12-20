# Dart
### Part1

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

EX (5) - (4 min)
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


