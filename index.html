
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
        brightness: Brightness.dark, // प्रीमियम और थियेटर लुक के लिए डार्क थीम
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
  int _currentIndex = 0;

  // चारों मुख्य सेक्शन्स/फोल्डर्स की लिस्ट
  final List<Widget> _screens = [
    const AdvancedVRPlayerScreen(), // 1. अपग्रेटेड 4K VR वीडियो प्लेयर
    const HolyBooksScreen(),         // 2. धार्मिक किताबें
    const StoryWriterScreen(),       // 3. कहानी डायरी
    const ShortVideosScreen(),       // 4. शॉर्ट्स और रील्स
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: SafeArea(child: _screens[_currentIndex]),
      bottomNavigationBar: BottomNavigationBar(
        currentIndex: _currentIndex,
        type: BottomNavigationBarType.fixed,
        backgroundColor: Colors.grey[950],
        selectedItemColor: Colors.amber,
        unselectedItemColor: Colors.white60,
        onTap: (index) {
          setState(() {
            _currentIndex = index;
          });
        },
        items: const [
          BottomNavigationBarItem(icon: Icon(Icons.play_circle_filled), label: '4K VR प्लेयर'),
          BottomNavigationBarItem(icon: Icon(Icons.menu_book), label: 'किताबें (ग्रंथ)'),
          BottomNavigationBarItem(icon: Icon(Icons.edit_note), label: 'कहानी डायरी'),
          BottomNavigationBarItem(icon: Icon(Icons.slideshow), label: 'शॉर्ट्स/रील्स'),
        ],
      ),
    );
  }
}

// ==========================================
// 1. 4K 3D VR वीडियो प्लेयर स्क्रीन (10GB+ फाइल सपोर्ट ढांचा)
// ==========================================
class AdvancedVRPlayerScreen extends StatefulWidget {
  const AdvancedVRPlayerScreen({Key? key}) : super(key: key);

  @override
  State<AdvancedVRPlayerScreen> createState() => _AdvancedVRPlayerScreenState();
}

class _AdvancedVRPlayerScreenState extends State<AdvancedVRPlayerScreen> {
  bool isVRMode = false; // VR बॉक्स हेडसेट के लिए स्प्लिट-स्क्रीन टॉगल
  String videoInfo = "फ़ाइल: 4K_SciFi_Movie_10GB.mp4\nरिज़ॉल्यूशन: 3840x2160 | साइज़: 10.4 GB";

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('⚡ 4K 3D VR Ultra Player'),
        backgroundColor: Colors.black,
        actions: [
          IconButton(
            icon: Icon(isVRMode ? Icons.view_in_ar : Icons.vr_pane_outlined, color: Colors.amber),
            tooltip: "VR बॉक्स मोड ऑन/ऑफ करें",
            onPressed: () {
              setState(() {
                isVRMode = !isVRMode; // नॉर्मल और VR मोड के बीच स्विच करें
              });
            },
          )
        ],
      ),
      body: Column(
        children: [
          // वीडियो प्लेबैक एरिया (भारी 10GB 4K फाइलों को रेंडर करने के लिए)
          Expanded(
            flex: 3,
            child: isVRMode 
              ? buildVRDoubleLensView()  // VR बॉक्स चश्मे के लिए स्क्रीन को दो हिस्सों में बांटेगा
              : buildNormal4KView(),     // नॉर्मल फुल स्क्रीन 4K व्यू
          ),
          
          // वीडियो कंट्रोल और फाइल डिटेल्स एरिया
          Expanded(
            flex: 1,
            child: Padding(
              padding: const EdgeInsets.all(16.0),
              child: Column(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  Text(
                    videoInfo,
                    textAlign: TextAlign.center,
                    style: const TextStyle(color: Colors.white70, fontSize: 13, fontFamily: 'monospace'),
                  ),
                  const SizedBox(height: 10),
                  Row(
                    mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                    children: [
                      IconButton(icon: const Icon(Icons.replay_10, size: 36, color: Colors.white), onPressed: () {}),
                      IconButton(icon: const Icon(Icons.play_circle_filled, size: 50, color: Colors.amber), onPressed: () {}),
                      IconButton(icon: const Icon(Icons.forward_10, size: 36, color: Colors.white), onPressed: () {}),
                    ],
                  ),
                ],
              ),
            ),
          )
        ],
      ),
    );
  }

  // नॉर्मल 4K / 3D साइड-बाय-साइड इंजन व्यू
  Widget buildNormal4KView() {
    return Center(
      child: Stack(
        alignment: Alignment.center,
        children: [
          Container(
            margin: const EdgeInsets.all(8),
            decoration: BoxDecoration(
              border: Border.all(color: Colors.amber.withOpacity(0.3)),
              borderRadius: BorderRadius.circular(12),
              color: Colors.grey[900],
            ),
            child: const Center(
              child: Icon(Icons.movie_creation_outlined, size: 80, color: Colors.white24),
            ),
          ),
          const Positioned(
            bottom: 20,
            child: Chip(
              backgroundColor: Colors.black85,
              label: Text("HARDWARE ACCELERATION ACTIVE (H.265/HEVC)", style: TextStyle(color: Colors.greenAccent, fontSize: 11)),
            ),
          )
        ],
      ),
    );
  }

  // VR स्प्लिट-लेंस व्यू (VR Box / Google Cardboard के लिए)
  Widget buildVRDoubleLensView() {
    return Row(
      children: [
        // बायीं आँख का व्यू (Left Eye)
        Expanded(
          child: Container(
            margin: const EdgeInsets.all(4),
            color: Colors.grey[900],
            child: const Center(
              child: Column(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  Icon(Icons.visibility, color: Colors.amber, size: 40),
                  SizedBox(height: 5),
                  Text("Left Eye (360° VR)", style: TextStyle(fontSize: 10, color: Colors.white60)),
                ],
              ),
            ),
          ),
        ),
        // लेंस एलाइनमेंट के लिए बीच की बॉर्डर लाइन
        Container(width: 2, color: Colors.amber),
        // दायीं आँख का व्यू (Right Eye)
        Expanded(
          child: Container(
            margin: const EdgeInsets.all(4),
            color: Colors.grey[900],
            child: const Center(
              child: Column(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  Icon(Icons.visibility, color: Colors.amber, size: 40),
                  SizedBox(height: 5),
                  Text("Right Eye (360° VR)", style: TextStyle(fontSize: 10, color: Colors.white60)),
                ],
              ),
            ),
          ),
        ),
      ],
    );
  }
}

// ==========================================
// 2. धार्मिक किताबें स्क्रीन (कुरान और गीता फोल्डर)
// ==========================================
class HolyBooksScreen extends StatelessWidget {
  const HolyBooksScreen({Key? key}) : super(key: key);
  
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: const Text('📖 पवित्र ग्रंथ (Holy Books)'), backgroundColor: Colors.black),
      body: ListView(
        padding: const EdgeInsets.all(16),
        children: [
          Card(
            color: Colors.grey[900],
            child: ListTile(
              leading: const Icon(Icons.book, color: Colors.green, size: 30),
              title: const Text('पवित्र कुरान (Holy Quran)', style: TextStyle(fontWeight: FontWeight.bold)),
              subtitle: const Text('अनुवाद, सूरह और पारा के साथ पढ़ें'),
              onTap: () {
                // यहाँ कुरान का पूरा टेक्स्ट पेज खुलेगा
              },
            ),
          ),
          const SizedBox(height: 10),
          Card(
            color: Colors.grey[900],
            child: ListTile(
              leading: const Icon(Icons.book, color: Colors.orange, size: 30),
              title: const Text('श्रीमद्भगवद्गीता (Bhagavad Gita)', style: TextStyle(fontWeight: FontWeight.bold)),
              subtitle: const Text('अध्याय, श्लोक और हिंदी अर्थ के साथ पढ़ें'),
              onTap: () {
                // यहाँ गीता का पूरा टेक्स्ट पेज खुलेगा
              },
            ),
          ),
        ],
      ),
    );
  }
}

// ==========================================
// 3. कहानी लिखने का फोल्डर (Story Writing Diary)
// ==========================================
class StoryWriterScreen extends StatefulWidget {
  const StoryWriterScreen({Key? key}) : super(key: key);

  @override
  State<StoryWriterScreen> createState() => _StoryWriterScreenState();
}

class _StoryWriterScreenState extends State<StoryWriterScreen> {
  final TextEditingController _storyController = TextEditingController();
  List<String> myStories = []; // यूजर की लिखी कहानियों को स्टोर करने के लिए लोकल लिस्ट

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: const Text('✍️ मेरी कहानियों की डायरी'), backgroundColor: Colors.black),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        children: [
          TextField(
            controller: _storyController,
            maxLines: 5,
            style: const TextStyle(color: Colors.white),
            decoration: InputDecoration(
              filled: true,
              fillColor: Colors.grey[900],
              border: const OutlineInputBorder(),
