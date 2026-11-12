<h1 align="center">📍 Family Locator</h1>

<p align="center">
  Real-time family location sharing for Android: see where your loved ones are, check their battery and send quick messages, powered by Firebase.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white" alt="Android">
  <img src="https://img.shields.io/badge/Backend-Firebase-FFCA28?logo=firebase&logoColor=black" alt="Firebase">
  <img src="https://img.shields.io/badge/Language-Kotlin-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin">
  <img src="https://img.shields.io/badge/License-MIT-blue" alt="MIT License">
</p>

---

## ✨ Features

- **Live location**: shares the phone's location in real time on a map
- **Battery status**: shows battery percentage and charging state
- **Quick messages**: family members can send messages straight to the device
- **Background updates**: keeps location fresh even when the app is closed
- **Secure**: data is stored in Firebase and only visible to linked family members

## 📸 Screenshots

| Map | Battery | Messages |
|:---:|:---:|:---:|
| <img src="screenshots/map.png" width="220"> | <img src="screenshots/battery.png" width="220"> | <img src="screenshots/messages.png" width="220"> |

> Put your screenshots in a `screenshots/` folder in the repo.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Kotlin |
| UI | Android XML / Material Design |
| Maps | Google Maps SDK |
| Location | Fused Location Provider API |
| Backend | Firebase Realtime Database / Firestore |
| Auth | Firebase Authentication |

## 🚀 Getting Started

### Prerequisites

- Android Studio (latest stable)
- An Android phone or emulator running Android 8.0+
- A Firebase account

### 1. Clone the repo

```bash
git clone https://github.com/arpangaur07/family-locator.git
cd family-locator
```

### 2. Set up Firebase

1. Go to the [Firebase Console](https://console.firebase.google.com/) and create a project.
2. Add an Android app using this project's package name.
3. Download `google-services.json` and place it in the `app/` folder.
4. Enable **Authentication** and **Realtime Database** (or Firestore).

### 3. Add your Google Maps API key

Get a key from the [Google Cloud Console](https://console.cloud.google.com/) and add it to `local.properties`:

```properties
MAPS_API_KEY=your_api_key_here
```

### 4. Build and run

Open the project in Android Studio, sync Gradle and hit **Run ▶️**.

## 🔐 Permissions

| Permission | Why it's needed |
|---|---|
| `ACCESS_FINE_LOCATION` | Get accurate location |
| `ACCESS_BACKGROUND_LOCATION` | Share location while the app is closed |
| `INTERNET` | Sync with Firebase |
| `POST_NOTIFICATIONS` | Show incoming messages |

## 📂 Project Structure

```
family-locator/
├── app/
│   ├── src/main/java/...    # Activities, services, Firebase logic
│   ├── src/main/res/        # Layouts, drawables, strings
│   └── google-services.json # (not committed)
├── screenshots/
└── README.md
```

## 🗺️ Roadmap

- [ ] Geofence alerts (notify when someone reaches home/college)
- [ ] Location history timeline
- [ ] SOS button
- [ ] Multiple family groups

## ⚠️ Privacy Note

This app is meant for **consensual** location sharing between family members. Everyone being tracked should know and agree.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 👤 Author

**Arpan Gaur**: B.Tech AI & ML, Galgotias University
GitHub: [@arpangaur07](https://github.com/arpangaur07)

---

<p align="center">⭐ If you found this useful, give it a star!</p>
