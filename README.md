# add
home and all add
import 'package:flutter/material.dart';
void main()=> runApp(HomePage());
class HomePage extends StatefulWidget{
  @override
  _HomePageState createState() => _HomePageState();
}
class _HomePageState extends State<HomePage> {
  @override
  Widget build(BuildContext) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.deepOrange,
          title: Text("JIBON SHOP"),
          actions: <Widget> [
            new IconButton(onPressed: null, icon: Icon(Icons.search,color: Colors.white,))
          ],
        ),
        drawer: new Drawer(
          child: new ListView(
            children: <Widget> [
              new UserAccountsDrawerHeader(
                accountName: Text("JIBON"),
                accountEmail: Text("mdzibonranabd.com"),
                currentAccountPicture: GestureDetector(
                  child: new CircleAvatar(
                    backgroundColor: Colors.cyanAccent,
                    child: Icon(Icons.person, color: Colors.orange,),
                  ),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("Home"),
                  leading: Icon(Icons.home),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("shopping"),
                  leading: Icon(Icons.add),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("Setting"),
                  leading: Icon(Icons.settings),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("About"),
                  leading: Icon(Icons.dashboard),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("Calls"),
                  leading: Icon(Icons.call),
                ),
              ),
              InkWell(
                onTap: () {},
                child: ListTile(
                  title: Text("Times"),
                  leading: Icon(Icons.access_time_outlined),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
