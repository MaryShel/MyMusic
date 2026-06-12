# My Music - Android Music Tunes App

A beautiful and feature-rich music player application built with Android Studio using Java.

## Features

### ✅ Implemented Features

1. **Splash Screen**
   - Displays for less than 3 seconds (2.5 seconds)
   - Includes app title and intro text
   - Features a status indicator (animated progress bar)
   - Custom background color theme

2. **Main Screen (Music Library)**
   - Scrollable grid layout with 2 columns
   - Displays 6 songs with album artwork
   - Shows song title, artist name, and duration
   - Play button under each song
   - Title bar with app icon

3. **Play Screen**
   - Large album artwork display
   - Song details (title, artist, duration)
   - Pause button to pause playback
   - Back button to return to main screen
   - Title bar with app icon
   - Vertically scrollable content

4. **Pause Screen**
   - Similar layout to play screen
   - Album artwork with fade effect (50% opacity)
   - Resume button to continue playback
   - Back button to return to main screen
   - Title bar with app icon
   - Status indicator showing "Music Paused"

5. **UI/UX Features**
   - Dark theme with purple and pink accent colors
   - Proper vertical and horizontal alignment
   - All text using string resources (no hardcoded text)
   - Responsive grid layout for different screen sizes
   - Professional color scheme

## Project Structure

```
MyMusic/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/mymusic/
│   │   │   │   ├── SplashActivity.java
│   │   │   │   ├── MainActivity.java
│   │   │   │   ├── PlayMusicActivity.java
│   │   │   │   ├── PauseMusicActivity.java
│   │   │   │   ├── Song.java (Model)
│   │   │   │   └── SongAdapter.java (RecyclerView Adapter)
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_splash.xml
│   │   │   │   │   ├── activity_main.xml
│   │   │   │   │   ├── song_item.xml
│   │   │   │   │   ├── activity_play_music.xml
│   │   │   │   │   └── activity_pause_music.xml
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml
│   │   │   │   │   ├── colors.xml
│   │   │   │   │   └── themes.xml
│   │   │   │   ├── menu/
│   │   │   │   │   └── menu_main.xml
│   │   │   │   └── drawable/ (Place your images here)
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   └── proguard-rules.pro
└── build.gradle
```

## Colors Used

- **Primary**: Purple (#FF6200EE)
- **Primary Dark**: Purple (#FF3700B3)
- **Accent**: Purple (#FF7b2cbf) & Pink (#FFc1121f)
- **Background**: Dark (#FF1a1a2e)
- **Text**: White & Light Gray

## Songs Included

1. Summer Vibes - Alex Johnson (3:45)
2. Night Dreams - Maria Garcia (4:20)
3. Electric Energy - The Beats (3:15)
4. Romantic Hour - Luna Sky (4:50)
5. Jazz Nights - Smooth Jazz Trio (5:30)
6. Urban Rhythm - City Sounds (3:55)

## Required Image Resources

Place the following drawable images in `app/src/main/res/drawable/`:

- `ic_song_1.png` (150x150 dp recommended)
- `ic_song_2.png`
- `ic_song_3.png`
- `ic_song_4.png`
- `ic_song_5.png`
- `ic_song_6.png`
- `ic_launcher_foreground.png` (optional, for toolbar icon)

## Setup Instructions

1. **Clone or create the project** in Android Studio
2. **Create drawable resources**: Add album artwork images to the drawable folder
3. **Build the project**: Gradle will download dependencies
4. **Run on emulator or device**: Select target device and click Run

## Dependencies

- AndroidX AppCompat
- AndroidX ConstraintLayout
- Google Material Components
- AndroidX RecyclerView

## How to Use

1. **Splash Screen**: App loads with animated progress indicator (2.5 seconds)
2. **Main Screen**: Browse all available songs in a grid layout
3. **Play Song**: Click the "Play" button under any song
4. **Pause/Resume**: Use Pause button to pause, Resume to continue
5. **Navigation**: Use back buttons to return to previous screens

## Threading

- Splash screen progress animation runs on a separate thread to prevent UI blocking
- Smooth progress bar animation over the splash duration

## Compatibility

- **Min SDK**: 21 (Android 5.0)
- **Target SDK**: 33 (Android 13)
- **Compilе SDK**: 33

## Future Enhancements

- Actual music playback with MediaPlayer
- Playlist management
- Song search functionality
- Favorites/Bookmarks feature
- Volume control
- Shuffle and repeat modes
- Music metadata display

## Author

Created with Android Studio and Java

---

**Note**: Replace placeholder images with actual album artwork for production use.
