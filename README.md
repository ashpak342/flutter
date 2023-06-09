*****(Flutter Program Statement)*****

1. Use SafeArea Widget in flutter App development

import 'package:flutter/material.dart';

//This example explains effect of SafeArea widget on view of App
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: SafeArea(
        top: true,
        child: Scaffold(
          body: Text(
            'This is an example explaining use of SafeArea',
            style: TextStyle(color: Colors.green, fontSize: 20),
          ),
        ),
      ),
    );
  }
}


2. Use AppBar Widget in flutter App development
//use any one example given below:

//appbar example 1:
import "package:flutter/material.dart";

void main() {
  runApp(MaterialApp(
    home: Scaffold(
      appBar: AppBar(
        title: Text("FAMT"),
        titleSpacing: 00.0,
        centerTitle: true,
        toolbarHeight: 60.2,
        shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(360)),
        elevation: 0.00,
        backgroundColor: Colors.greenAccent[400],
      ), //AppBar
      body: const Center(
        child: Text(
          'IT Department',
          style: TextStyle(fontSize: 24),
        ), //Text
      ), //Center
    ), //Scaffold
    debugShowCheckedModeBanner: false, //Removing Debug Banner
  )); //MaterialApp
}


//appbar example 2:
import "package:flutter/material.dart";

void main() {
  runApp(MaterialApp(
    home: Scaffold(
      appBar: AppBar(
        title: Text("FAMT"),
        actions: <Widget>[
          IconButton(
            icon: Icon(Icons.comment),
            tooltip: 'Comment Icon',
            onPressed: () {},
          ), //IconButton
          IconButton(
            icon: Icon(Icons.settings),
            tooltip: 'Setting Icon',
            onPressed: () {},
          ), //IconButton
        ], //<Widget>[]
        backgroundColor: Colors.greenAccent[400],
        elevation: 50.0,
        leading: IconButton(
          icon: Icon(Icons.menu),
          tooltip: 'Menu Icon',
          onPressed: () {},
        ), //IconButton
        brightness: Brightness.dark,
      ), //AppBar
      body: const Center(
        child: Text(
          "IT Department",
          style: TextStyle(fontSize: 24),
        ), //Text
      ), //Center
    ), //Scaffold
    debugShowCheckedModeBanner: false, //Removing Debug Banner
  )); //MaterialApp
}



3. Use Row Widget in flutter App development

import 'package:flutter/material.dart';

//Example for Row Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("IT Department"),
      ),
      body: Row(
          mainAxisAlignment: MainAxisAlignment.spaceAround,
          children: <Widget>[
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "TEIT",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            ),
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "and",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            ),
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "FAMT",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            )
          ]),
    );
  }
}



4. Use Column Widget in flutter App development

import 'package:flutter/material.dart';

//Example for Column Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("IT Department"),
      ),
      body: Column(
          mainAxisAlignment: MainAxisAlignment.spaceAround,
          children: <Widget>[
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "TEIT",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            ),
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "TEIT",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            ),
            Container(
              decoration: BoxDecoration(
                  borderRadius: BorderRadius.circular(10), color: Colors.green),
              child: Text(
                "TEIT",
                style: TextStyle(color: Colors.white, fontSize: 25),
              ),
            )
          ]),
    );
  }
}



5. Use Container Widget with child property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating child property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



6. Use Container Widget with color property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating color property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          color: Colors.purple,
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



7. Use Container Widget with height and width property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating Height and Width property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          color: Colors.purple,
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



8. Use Container Widget with margin property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating margin property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          color: Colors.purple,
          margin: EdgeInsets.all(20),
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



9. Use Container Widget with padding property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating padding property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          color: Colors.purple,
          margin: EdgeInsets.all(20),
          padding: EdgeInsets.all(30),
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



10. Use Container Widget with alignment property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating alignment property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          color: Colors.purple,
          alignment: Alignment.bottomCenter,
          margin: EdgeInsets.all(20),
          padding: EdgeInsets.all(30),
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



11. Use Container Widget with decoration property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating decoration property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          //color: Colors.purple,
          alignment: Alignment.center,
          margin: EdgeInsets.all(20),
          padding: EdgeInsets.all(30),
          decoration: BoxDecoration(
            border: Border.all(color: Colors.black, width: 3),
          ),
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



12. Use Container Widget with transform property in flutter App development

import 'package:flutter/material.dart';

//This Example is for demonstrating transform property of Container
void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container example"),
        ),
        body: Container(
          height: 200,
          width: double.infinity,
          color: Colors.purple,
          alignment: Alignment.center,
          margin: EdgeInsets.all(20),
          padding: EdgeInsets.all(30),
         transform: Matrix4.skewX(0.4),
          child: Text("Hello! i am inside a container!",
              style: TextStyle(fontSize: 20)),
        ),
      ),
    );
  }
}



13. Use FlatButton Widget in flutter App development

import 'package:flutter/material.dart';

//This example explains FlatButten Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
          appBar: AppBar(
            title: Text('Flutter Buttons - FlatButton'),
          ),
          body: Center(
              child: Column(children: <Widget>[
            Container(
              margin: EdgeInsets.all(25),
              child: FlatButton(
                child: Text(
                  'Button 1',
                  style: TextStyle(fontSize: 20.0),
                ),
                onPressed: () {},
              ),
            ),
            Container(
              margin: EdgeInsets.all(25),
              child: FlatButton(
                child: Text(
                  'Button 2',
                  style: TextStyle(fontSize: 20.0),
                ),
                color: Colors.cyan,
                textColor: Colors.black,
                onPressed: () {},
              ),
            ),
          ]))),
    );
  }
}

//TextButton

import 'package:flutter/material.dart';

//This example explains FlatButten Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Flutter Buttons - TextButton'),
        ),
        body: Center(
          child: Column(
            children: <Widget>[
              Container(
                margin: EdgeInsets.all(25),
                child: TextButton(
                  child: Text(
                    'Button 1',
                    style: TextStyle(fontSize: 25),
                  ),
                  onPressed: () {},
                ),
              ),
              Container(
                margin: EdgeInsets.all(25),
                child: TextButton(
                  child: Text(
                    'Button 2',
                    style: TextStyle(fontSize: 25),
                  ),
                  onPressed: () {},
                  style: TextButton.styleFrom(
                      foregroundColor: Colors.black,
                      elevation: 2,
                      backgroundColor: Colors.cyan),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}


14. Use RaisedButton Widget in flutter App development

import 'package:flutter/material.dart';

//This example explains Raised Button Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  String msg = 'Flutter - Raised Button';
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Flutter - Raised Button'),
        ),
        body: Container(
          child: Center(
            child: Column(
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Text(
                  msg,
                  style: TextStyle(fontSize: 30, fontStyle: FontStyle.normal),
                ),
                RaisedButton(
                  child: Text(
                    "Click Here",
                    style: TextStyle(fontSize: 20),
                  ),
                  onPressed: _changeText,
                  color: Colors.red,
                  textColor: Colors.white,
                  padding: EdgeInsets.all(8.0),
                  splashColor: Colors.grey,
                )
              ],
            ),
          ),
        ),
      ),
    );
  }

  _changeText() {
    setState(() {
      if (msg == 'Flutter - Raised Button') {
        msg = 'Changed the Text';
      } else {
        msg = 'Flutter - Raised Button';
      }
    });
  }
}

//ElevatedButton

import 'package:flutter/material.dart';

//This example explains Raised Button Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  String msg = 'Flutter - Elevated Button ';
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Flutter - Elevated Button'),
        ),
        body: Container(
          child: Center(
            child: Column(
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Text(
                  msg,
                  style: TextStyle(fontSize: 30, fontStyle: FontStyle.normal),
                ),
                ElevatedButton(
                  child: Text('Click Here'),
                  style: ElevatedButton.styleFrom(
                      primary: Colors.red,
                      padding: EdgeInsets.all(8.0),
                      textStyle: const TextStyle(
                        color: Colors.white,
                        fontSize: 20,
                      )),
                  onPressed: _changeText,
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }

  _changeText() {
    setState(() {
      if (msg == 'Flutter - Raised Button') {
        msg = 'Changed the Text';
      } else {
        msg = 'Flutter - Raised Button';
      }
    });
  }
}


15. Use Floating Action Button Widget in flutter App development

import 'package:flutter/material.dart';

//This example explains Floating Action Button Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Flutter Floating Action Button"),
          backgroundColor: Colors.blue,
        ),
        floatingActionButton: FloatingActionButton(
          child: Icon(Icons.share),
          backgroundColor: Colors.blueAccent,
          foregroundColor: Colors.white,
          onPressed: () => {},
        ),
        // floatingActionButton: FloatingActionButton.extended(
        //   onPressed: () {},
        //   icon: Icon(Icons.account_circle),
        //   label: Text("Profile"),
        // ),
      ),
    );
  }
}



16. Use Dropdown Button Widget in flutter App development

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
        primarySwatch: Colors.blue,
        visualDensity: VisualDensity.adaptivePlatformDensity,
      ),
      home: Scaffold(
        body: Center(
          child: MyHomePage(),
        ),
      ),
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  String? dropdownvalue = 'Flutter';

  @override
  Widget build(BuildContext context) {
    return DropdownButton<String>(
      value: dropdownvalue,
      icon: Icon(Icons.arrow_drop_down),
      iconSize: 25,
      elevation: 16,
      style: TextStyle(color: Colors.blue),
      underline: Container(
        height: 3,
        color: Colors.blueAccent,
      ),
      onChanged: (String? newValue) {
        setState(() {
          dropdownvalue = newValue;
        });
      },
      items: <String>["Flutter", "Java", "Android", "Kotlin", "React Native"]
          .map<DropdownMenuItem<String>>((String val) {
        // ignore: missing_required_param
        return DropdownMenuItem<String>(
          value: val,
          child: Text(val),
        );
      }).toList(),
    );
  }
}



17. Use Icon Button Widget in flutter App development

import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Flutter - Icon Button"),
        ),
        body: Center(
          child: MyStatefulWidget(),
        ),
      ),
    );
  }
}

double _speakervolume = 0.0;

class MyStatefulWidget extends StatefulWidget {
  @override
  _MyStatefulWidgetState createState() => _MyStatefulWidgetState();
}

class _MyStatefulWidgetState extends State<MyStatefulWidget> {
  Widget build(BuildContext context) {
    return Column(
      mainAxisSize: MainAxisSize.min,
      children: <Widget>[
        IconButton(
          icon: Icon(Icons.volume_up),
          iconSize: 50,
          color: Colors.brown,
          tooltip: 'Increase volume by 5',
          onPressed: () {
            setState(() {
              _speakervolume += 5;
            });
          },
        ),
        Text('Speaker Volume: $_speakervolume')
      ],
    );
  }
}



18. Use RichText Widget in flutter App development

import 'package:flutter/material.dart';

//This example exlains RichText Widget
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
// This widget is
//the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'ClipOval',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: MyHomePAGE(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePAGE extends StatefulWidget {
  @override
  _MyHomePAGEState createState() => _MyHomePAGEState();
}

class _MyHomePAGEState extends State<MyHomePAGE> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('FAMTIT'),
        backgroundColor: Colors.green,
      ),
      body: Center(
          child: RichText(
        text: TextSpan(
          text: 'Hello ',
          style: DefaultTextStyle.of(context).style,
          children: <TextSpan>[
            TextSpan(
                text: 'FAMT', style: TextStyle(fontWeight: FontWeight.bold)),
          ],
        ),
      )),
      backgroundColor: Colors.lightBlue[50],
    );
  }
}

class MyClip extends CustomClipper<Rect> {
  Rect getClip(Size size) {
    return Rect.fromLTWH(0, 0, 100, 100);
  }

  bool shouldReclip(oldClipper) {
    return false;
  }
}




19. Use Container Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using Container
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: SafeArea(
          // Container implementation
          child: Container(
            height: 100.0,
            width: 100.0,
            color: Colors.green,
          ),
        ));
  }
}



20. Use GridView Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using Gridview
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  Widget _buildGrid() => GridView.extent(
      maxCrossAxisExtent: 150,
      padding: const EdgeInsets.all(4),
      mainAxisSpacing: 4,
      crossAxisSpacing: 4,
      children: _buildGridTileList(10));

  List<Container> _buildGridTileList(int count) => List.generate(
      count,
      (i) => Container(
            width: 100,
            height: 100,
            color: Colors.blue,
          ));

  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: Center(child: _buildGrid()));
  }
}



21. Use ListView Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using ListView
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  // function returning List view widget
  Widget _buildList() => ListView(
        // name is a listTile widget which is defined below
        children: [
          name('james', 'thomas'),
          name('Ajay', 'kumar'),
          name('Arun', 'das'),
          name('Roxie', 'St'),
          name('Stanlee', 'jr'),
          name('AMC', 'hales'),
          Divider(),
          name('Monty', "Chopra"),
          name('Emmy', 'Ave'),
          name('Chaitanya', ' kumar'),
          name('Rio', 'St'),
        ],
      );

// name is a function returning ListTile widget
  ListTile name(String firstName, String lastName) => ListTile(
        title: Text(firstName,
            style: TextStyle(
              fontWeight: FontWeight.w500,
              fontSize: 20,
            )),
        subtitle: Text(lastName),
        leading: Icon(
          Icons.arrow_back_ios,
          color: Colors.blue[500],
        ),
      );

  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: Center(child: _buildList()));
  }
}



22. Use StackView Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using Stackview
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  // function returning List view widget

// this function returns a stack widget
  Widget _buildStack() => Stack(
        alignment: const Alignment(0.6, 0.6),
        children: [
          Container(
            width: 150,
            height: 150,
            decoration:
                BoxDecoration(color: Colors.black45, shape: BoxShape.circle),
            child: Center(
              child: Text(
                'Mia B',
                style: TextStyle(
                  fontSize: 20,
                  fontWeight: FontWeight.bold,
                  color: Colors.black,
                ),
              ),
            ),
          ),
        ],
      );

  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: Center(child: _buildStack()));
  }
}




23. Use CardView Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using CardView
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  Widget _buildCard() => SizedBox(
        height: 210,
        child: Card(
          elevation: 20,
          child: Column(
            children: [
              ListTile(
                title: Text('FAMT IT',
                    style: TextStyle(fontWeight: FontWeight.w500)),
                subtitle: Text('log writting'),
                leading: Icon(
                  Icons.restaurant_menu,
                  color: Colors.blue[500],
                ),
              ),
              Divider(),
              ListTile(
                title: Text('8080808080',
                    style: TextStyle(fontWeight: FontWeight.w500)),
                leading: Icon(
                  Icons.contact_phone,
                  color: Colors.blue[500],
                ),
              ),
              ListTile(
                title: Text('gfg@contribute.com'),
                leading: Icon(
                  Icons.contact_mail,
                  color: Colors.blue[500],
                ),
              ),
            ],
          ),
        ),
      );

  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: Center(child: _buildCard()));
  }
}




24. Use ListTile Widget in flutter App development.

import 'package:flutter/material.dart';

//Example for explaining Layout using ListTile
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'FAMT',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: AppBar(
          title: Text("IT Department"),
        ),
        body: Container(
          child: ListTile(
            title:
                Text('FAMT IT', style: TextStyle(fontWeight: FontWeight.w500)),
            subtitle: Text('log writting'),
            leading: Icon(
              Icons.restaurant_menu,
              color: Colors.blue[500],
            ),
          ),
        ));
  }
}



25. Use flutter icons in flutter App development.

import 'package:flutter/material.dart';  
  
void main() => runApp(MyApp());  
  
class MyApp extends StatelessWidget {  
  // This widget is the root of your application.  
  @override  
  Widget build(BuildContext context) {  
    return MaterialApp(  
      theme: ThemeData(  
        primarySwatch: Colors.blue,  
      ),  
      home: MyIconPage(),  
    );  
  }  
}  
  
class MyIconPage extends StatefulWidget {  
  @override  
  _MyIconPageState createState() => _MyIconPageState();  
}  
  
class _MyIconPageState extends State<MyIconPage> {  
  @override  
  Widget build(BuildContext context) {  
    return Scaffold(  
      appBar: AppBar(  
        title: Text('Flutter Icon Tutorial'),  
      ),  
      body: Row(  
        mainAxisAlignment: MainAxisAlignment.spaceAround,  
          children: <Widget>[  
            Icon(Icons.camera_enhance),  
            Icon(Icons.camera_front),  
            Icon(Icons.camera_rear),  
      ]),  
    );  
  }  
}  



26. Use flutter image.asset to add image in flutter App development.
steps:
1)create a "assets" folder insde that create another "images" folder (assets/images) in root project folder and paste the image inside that folder.

2)edit "pubspec.yaml" file whcih is avaible in root folder  of project.
search for following code inside this file:
# To add assets to your application, add an assets section, like this:
  # assets:
  #   - images/a_dot_burr.jpeg
  #   - images/a_dot_ham.jpeg

now repalce this code with following code:
# To add assets to your application, add an assets section, like this:
  assets:
     - assets/images/famtitlab.jpg

3)Note- replace the "famtitlab.jpg" file name with your image file name.(in both main.dart and pubspec.yaml file)


4) paste the following code in main.dart file:

import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
// This widget is the root
// of your application

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Insert Image Demo'),
        ),
        body: Center(
          child: Column(
            children: <Widget>[
              Image.asset('assets/images/famtitlab.jpg'),
            ],
          ),
        ),
      ),
    );
  }
}




27. Use Flutter Navigation and Routing in flutter App development.
//use any one example given below:

//1st example:
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(
    title: 'Flutter Navigation',
    theme: ThemeData(
      // This is the theme of your application.
      primarySwatch: Colors.green,
    ),
    home: FirstRoute(),
  ));
}

class FirstRoute extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('First Screen'),
      ),
      body: Center(
        child: ElevatedButton(
          child: Text('Click Here'),
          style: ElevatedButton.styleFrom(
            primary: Colors.orangeAccent,
          ),
          onPressed: () {
            Navigator.push(
              context,
              MaterialPageRoute(builder: (context) => SecondRoute()),
            );
          },
        ),
      ),
    );
  }
}

class SecondRoute extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Second Screen"),
      ),
      body: Center(
        child: ElevatedButton(
          style: ElevatedButton.styleFrom(
            primary: Colors.blueGrey,
          ),
          onPressed: () {
            Navigator.pop(context);
          },
          child: Text('Go back'),
        ),
      ),
    );
  }
}




//2nd example named routes:
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(
    title: 'Named Route Navigation',
    theme: ThemeData(
      // This is the theme of your application.
      primarySwatch: Colors.green,
    ),
    // Start the app with the "/" named route. In this case, the app starts
    // on the FirstScreen widget.
    initialRoute: '/',
    routes: {
      // When navigating to the "/" route, build the FirstScreen widget.
      '/': (context) => HomeScreen(),
      // When navigating to the "/second" route, build the SecondScreen widget.
      '/second': (context) => SecondScreen(),
    },
  ));
}

class HomeScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Home Screen'),
      ),
      body: Center(
        child: ElevatedButton(
          child: Text('Click Here'),
          style: ElevatedButton.styleFrom(
            primary: Colors.orangeAccent,
          ),
          onPressed: () {
            Navigator.pushNamed(context, '/second');
          },
        ),
      ),
    );
  }
}

class SecondScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Second Screen"),
      ),
      body: Center(
        child: ElevatedButton(
          style: ElevatedButton.styleFrom(
            primary: Colors.blueGrey,
          ),
          onPressed: () {
            Navigator.pop(context);
          },
          child: Text('Go back!'),
        ),
      ),
    );
  }
}



28. Use flutter image.asset to add image in flutter App development.
//same as question no. 26


29. Use flutter to implement Gesture in App development.

import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo Application',
      theme: ThemeData(
        primarySwatch: Colors.green,
      ),
      home: MyHomePage(),
    );
  }
}

class MyHomePage extends StatefulWidget {
  @override
  MyHomePageState createState() => new MyHomePageState();
}

class MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Gestures Example'),
        centerTitle: true,
      ),
      body: new Center(
          child: GestureDetector(
              onTap: () {
                print('Box Clicked');
              },
              child: Container(
                height: 60.0,
                width: 120.0,
                padding: EdgeInsets.all(10.0),
                decoration: BoxDecoration(
                  color: Colors.blueGrey,
                  borderRadius: BorderRadius.circular(15.0),
                ),
                child: Center(child: Text('Click Me')),
              ))),
    );
  }
}
