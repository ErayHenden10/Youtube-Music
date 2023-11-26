import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: InstagramUI(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class InstagramUI extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        backgroundColor: Colors.white,
        title: Text(
          'Instagram',
          style: TextStyle(
            color: Colors.black,
            fontFamily: 'Billabong', 
            fontSize: 30.0,
          ),
        ),
        centerTitle: true,
        leading: IconButton(
          icon: Icon(Icons.camera_alt),
          onPressed: () {
            
          },
          color: Colors.black,
        ),
        actions: <Widget>[
          IconButton(
            icon: Icon(Icons.send),
            onPressed: () {
              
            },
            color: Colors.black,
          ),
        ],
      ),
      body: SingleChildScrollView(
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: <Widget>[
            
            _buildPost(
              'assets/images/resim.jpg.jpg', 
              'Berat Tokuş', 
              'Erciyes Dağından görüntüler :)', 
            ),
            
          ],
          
          
        ),
        
      ),
      
    );
  }

  Widget _buildPost(String imagePath, String username, String description) {
    return Column(
      crossAxisAlignment: CrossAxisAlignment.stretch,
      children: <Widget>[
        Padding(
          padding: EdgeInsets.all(12.0),
          child: Row(
            mainAxisAlignment: MainAxisAlignment.spaceBetween,
            children: <Widget>[
              CircleAvatar(
                radius: 20.0,
                backgroundImage: AssetImage('assets/images/resim.jpg.jpg'), // Kullanıcı profil resmi
              ),
              SizedBox(width: 8.0),
              Text(
                username,
                style: TextStyle(
                  fontWeight: FontWeight.bold,
                ),
              ),
              Spacer(),
              Icon(Icons.more_horiz),
            ],
          ),
        ),
        Image.asset(
          imagePath,
          fit: BoxFit.cover,
          height: 300.0,
        ),
        Padding(
          padding: EdgeInsets.all(12.0),
          child: Row(
            children: <Widget>[
              Icon(Icons.favorite_border),
              SizedBox(width: 8.0),
              Icon(Icons.chat_bubble_outline),
              SizedBox(width: 8.0),
              Icon(Icons.send),
              Spacer(),
              Icon(Icons.bookmark_border),
            ],
          ),
        ),
        Padding(
          padding: EdgeInsets.symmetric(horizontal: 12.0),
          child: Text(
            description,
            style: TextStyle(
              fontWeight: FontWeight.bold,
            ),
          ),
        ),
        SizedBox(height: 12.0),
        Divider(height: 1.0),
      ],
    );
  }
}
