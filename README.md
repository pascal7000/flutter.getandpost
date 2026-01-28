CSC315 Remote Demo App 🚀
A Flutter application built for CSC315 that demonstrates consuming a REST API using the Repository Pattern. The app fetches data from JSONPlaceholder and displays it in a clean, scrollable list.

📱 Screenshots
<img width="740" height="687" alt="screenshot" src="https://github.com/user-attachments/assets/1340d693-e325-4b15-a39d-810159a9229b" />

✨ Features
GET Request: Fetches a list of posts from https://jsonplaceholder.typicode.com/posts.
POST Request: Includes logic to create new posts via the Repository.
Asynchronous UI: Uses FutureBuilder to handle loading states and data display.
Clean Architecture: Separates logic into distinct layers (UI, Data, Logic).
🛠️ Project Structure
The project follows a modular structure for better maintainability:


lib/
├── main.dart                   # UI Layer (FutureBuilder & ListView)
├── models/
│   └── post.dart               # Data Model (fromJson / toJson)
└── repository/
└── post_repository.dart    # API Logic (http.get / http.post)

📦 Dependencies
http: ^1.x.x
flutter/material.dart
🚀 How to Run
Clone the repository:

git clone https://github.com/pascal7000/flutter.getandpost
cd csc315_remote_demo
Install dependencies:

flutter pub get
Run the app: (Recommended to run on Chrome if Android emulators are not set up)

flutter run -d chrome

