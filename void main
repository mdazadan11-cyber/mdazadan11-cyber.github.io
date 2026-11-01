import 'package:flutter/material.dart';

void main() {
  runApp(const MySuperApp());
}

class MySuperApp extends StatelessWidget {
  const MySuperApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: '4K VR Media & Books Super App',
      theme: ThemeData(
        primarySwatch: Colors.deepPurple,
        brightness: Brightness.dark, // प्रीमियम और थियेटर लुक के लिए
        scaffoldBackgroundColor: Colors.black,
      ),
      home: const MainHomeScreen(),
    );
  }
}

class MainHomeScreen extends StatefulWidget {
  const MainHomeScreen({Key? key}) : super(key: key);

  @override
  State<MainHomeScreen> createState() => _MainHomeScreenState();
}

class _MainHomeScreenState extends State<MainHomeScreen> {
  int currentIndex = 0;

  final List<Widget> screens = [
    const HomeTab(),
    const VRTab(),
    const BooksTab(),
    const ProfileTab(),
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: screens[currentIndex],
      bottomNavigationBar: BottomNavigationBar(
        backgroundColor: const Color(0xFF161B22),
        selectedItemColor: Colors.deepPurpleAccent,
        unselectedItemColor: Colors.grey,
        type: BottomNavigationBarType.fixed,
        currentIndex: currentIndex,
        onTap: (i) => setState(() => currentIndex = i),
        items: const [
          BottomNavigationBarItem(icon: Icon(Icons.home), label: 'Home'),
          BottomNavigationBarItem(icon: Icon(Icons.vrpano), label: '4K VR'),
          BottomNavigationBarItem(icon: Icon(Icons.menu_book), label: 'Books'),
          BottomNavigationBarItem(icon: Icon(Icons.person), label: 'Profile'),
        ],
      ),
    );
  }
}

class HomeTab extends StatelessWidget {
  const HomeTab({super.key});
  @override
  Widget build(BuildContext context) {
    return const Center(
      child: Column(
        mainAxisAlignment: MainAxisAlignment.center,
        children: [
          Icon(Icons.movie_filter, size: 80, color: Colors.deepPurple),
          SizedBox(height: 20),
          Text('4K VR Media & Books', style: TextStyle(fontSize: 24, fontWeight: FontWeight.bold)),
          Text('Super App is Ready', style: TextStyle(color: Colors.grey)),
        ],
      ),
    );
  }
}

class VRTab extends StatelessWidget {
  const VRTab({super.key});
  @override
  Widget build(BuildContext context) => const Center(child: Text('VR Media Screen'));
}

class BooksTab extends StatelessWidget {
  const BooksTab({super.key});
  @override
  Widget build(BuildContext context) => const Center(child: Text('Books Screen'));
}

class ProfileTab extends StatelessWidget {
  const ProfileTab({super.key});
  @override
  Widget build(BuildContext context) => const Center(child: Text('Azad - mdazadan11-cyber'));
}
