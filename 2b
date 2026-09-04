import 'package:flutter/material.dart';

void main() {
  runApp(LayoutDemoApp());
}

class LayoutDemoApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Layout Structures Demo',
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(
          title: Text('Row, Column & Stack Layouts'),
          backgroundColor: Colors.deepPurple,
        ),
        body: SingleChildScrollView(
          child: Padding(
            padding: const EdgeInsets.all(16.0),
            child: Column(
              crossAxisAlignment: CrossAxisAlignment.stretch,
              children: [
                Text(
                  'Row Layout (Horizontal)',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Row(
                  mainAxisAlignment: MainAxisAlignment.spaceAround,
                  crossAxisAlignment: CrossAxisAlignment.center,
                  children: [
                    Icon(Icons.home, color: Colors.blue),
                    Text('Home'),
                    ElevatedButton(onPressed: () {}, child: Text('Click')),
                  ],
                ),
                Divider(),
                Text(
                  'Column Layout (Vertical)',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Column(
                  crossAxisAlignment: CrossAxisAlignment.start,
                  children: [
                    Icon(Icons.person, color: Colors.orange),
                    Text('Profile'),
                    ElevatedButton(onPressed: () {}, child: Text('Edit')),
                  ],
                ),
                Divider(),
                Text(
                  'Nested Row & Column',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Row(
                  children: [
                    Expanded(
                      child: Column(
                        children: [
                          Text('Left Section'),
                          Icon(Icons.arrow_left),
                        ],
                      ),
                    ),
                    Expanded(
                      child: Column(
                        children: [
                          Text('Right Section'),
                          Icon(Icons.arrow_right),
                        ],
                      ),
                    ),
                  ],
                ),
                Divider(),
                Text(
                  'Row with Expanded Widgets',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Row(
                  children: [
                    Expanded(child: Container(height: 50, color: Colors.red)),
                    Expanded(child: Container(height: 50, color: Colors.green)),
                    Expanded(child: Container(height: 50, color: Colors.blue)),
                  ],
                ),
                Divider(),
                Text(
                  'Stack Layout (Overlapping)',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Center(
                  child: Container(
                    width: 200,
                    height: 200,
                    color: Colors.grey[300],
                    child: Stack(
                      alignment: Alignment.center,
                      children: [
                        Container(width: 150, height: 150, color: Colors.red),
                        Container(width: 100, height: 100, color: Colors.green),
                        Container(width: 50, height: 50, color: Colors.blue),
                        Positioned(
                          right: 10,
                          bottom: 10,
                          child: Text(
                            'Positioned Text',
                            style: TextStyle(
                              color: Colors.white,
                              backgroundColor: Colors.black,
                            ),
                          ),
                        ),
                      ],
                    ),
                  ),
                ),
                Divider(),
                Text(
                  'Stack with Image & Text',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                ),
                SizedBox(height: 10),
                Center(
                  child: Stack(
                    alignment: Alignment.bottomCenter,
                    children: [
                      Image.network(
                        'https://images.pexels.com/photos/674010/pexels-photo674010.jpeg?cs=srgb&dl=pexels-anjana-c-169994674010.jpg&fm=jpg',
                        width: 200,
                        height: 200,
                        fit: BoxFit.cover,
                      ),
                      Container(
                        width: 200,
                        color: Colors.black54,
                        padding: EdgeInsets.all(4),
                        child: Text(
                          'Flutter Logo',
                          style: TextStyle(color: Colors.white),
                          textAlign: TextAlign.center,
                        ),
                      )
                    ],
                  ),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}
