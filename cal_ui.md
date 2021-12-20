```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);
  
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        // backgroundColor: Colors.blue,
        body: Center(
            child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Row(
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Container(
                  margin: EdgeInsets.all(10),
                  width: 75,
                  height: 75,
                  child: Center(
                    child: Text('C'),
                  ),
                  color: Colors.green[200],
                ),
                Container(
                  margin: EdgeInsets.all(10),
                  width: 75,
                  height: 75,
                  child: Center(
                    child: Text('+/-'),
                  ),
                  color: Colors.green[200],
                ),
                Container(
                  margin: EdgeInsets.all(10),
                  width: 75,
                  height: 75,
                  child: Center(
                    child: Text('%'),
                  ),
                  color: Colors.green[200],
                ),
                Container(
                  margin: EdgeInsets.all(10),
                  width: 75,
                  height: 75,
                  child: Center(
                    child: Text('÷'),
                  ),
                  color: Colors.green[200],
                ),
              ],
            ),
          ],
        )),
      ),
    );
  }
}



```
