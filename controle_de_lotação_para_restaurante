# layuot_para_restaurant


import 'package:flutter/material.dart';

void main() {

  runApp(
      MaterialApp(

        home: Home()));
}

class Home extends StatefulWidget {
  @override
  _HomeState createState() => _HomeState();
}

class _HomeState extends State<Home> {
  int _people=0;

  // ignore: unused_field
  String  _infoText = "Get In";

  void _changePeople(int delta){
    setState(() {
       _people += delta;
        if (_people < 0){_infoText= "You can Close now";
      } else if (_people <= 10 ) { _infoText = "Get In ";
        } else { _infoText ="God Job :) ";
        }

      } );
  }

  @override


  Widget build(BuildContext context) {

    return Stack(
      children: <Widget>[
        Image.asset(
          "image/restaurant.jpg",
          fit: BoxFit.cover,
          height: 1000.0,
        ),

        Column(

          children: <Widget>[
            Text("Pessoas : $_people",
                style: TextStyle(
                    color: Colors.white,
                    fontStyle: FontStyle.italic,
                    fontSize: 40.0)),
            Row(
                mainAxisAlignment: MainAxisAlignment.center,
                children: <Widget>[
                  Padding(
                      child:
                      FlatButton(
                        child: Text("in",
                            style: TextStyle(
                                fontSize: 45.0, color: Colors.white)),
                        onPressed: () {_changePeople(1);},),
                      padding: EdgeInsets.all(10.0)


                  ),

                  Padding(
                      child:
                      FlatButton(
                        child: Text("out",
                            style: TextStyle(
                                fontSize: 40.0, color: Colors.white)),
                        onPressed: () {_changePeople(-1);},),
                      padding: EdgeInsets.all(10.0)

                  ),
                ]),

            Row(
                mainAxisAlignment: MainAxisAlignment.center,
                children: <Widget>[

                  Text(_infoText,
                      style: TextStyle(
                          color: Colors.white38,
                          fontStyle: FontStyle.italic,
                          fontSize: 40.0)),
                ] )
          ],



        )

      ],

    );

  }
}

