# 🎵 DataFlair Python MP3 Music Player App

## 📋 Overview
This is a straightforward MP3 music player application built with **Python**. It uses **tkinter** for the graphical user interface and **pygame.mixer** for handling audio playback. This app lets you add, play, pause, stop, resume, and navigate through your collection of MP3 songs.

---

## 🚀 Features
- 🎼 **Add Songs**: Easily add multiple MP3 files to your playlist.
- ⏯ **Playback Controls**: Standard functions like Play, Pause, Stop, and Resume.
- ⏪⏩ **Navigation**: Move between songs with Previous and Next buttons.
- ❌ **Delete Song**: Remove unwanted songs from your playlist.
- 🖥 **User-Friendly Interface**: A clean and intuitive design for ease of use.

---

## 🧰 Prerequisites
Before running this application, you’ll need the following Python libraries:

- `pygame`: Essential for audio playback.
- `tkinter`: Typically included with Python, this is for the graphical interface.

Install `pygame` using pip:

```bash
pip install pygame
```

## ▶️ How to Run

### 💾 Save the Code
Save the provided Python code into a file, for example, `music_player.py`.

### 📁 Organize Your Music (Recommended)
It's a good idea to keep your MP3s in a dedicated folder.  
The `addsongs()` function defaults to looking in a `Music/` directory if it's in the same location as your script.

### 🏃‍♂️ Run the Script
Open your terminal or command prompt, navigate to the directory where you saved the file, and run:

```bash
python music_player.py
```
## 🎮 Usage

### 🎵 Adding Songs
- Click on **"Menu"** in the top menu bar.
- Select **"Add songs"**.
- A file dialog will appear. Browse to your MP3 files, select one or more, and click **"Open"**.  
  The songs will appear in the playlist.

### ▶️ Playing a Song
- Select a song from the listbox by clicking on it.
- Click the **"Play"** button.

### ⏱ Controlling Playback
- **Pause**: Click to temporarily stop the current song.
- **Resume**: Continue playback from where it was paused.
- **Stop**: End the current song and clear its selection.
- **Prev**: Play the song before the current one.
- **Next**: Play the song after the current one.

### 🗑 Deleting a Song
- Select the song to remove from the listbox.
- Click on **"Menu"** > **"Delete song"**.  
  The selected song will be removed from your playlist.
## ⚠️ Important Notes and Adjustments

### 🔧 File Paths
The code uses hardcoded paths like:
- `C:/Users/DataFlair/python-mp3-music-player/`
- `C:/Users/lenovo/Desktop/DataFlair/Notepad/Music/`

Update these paths in the `addsongs()`, `Play()`, `Previous()`, and `Next()` functions to match the actual location of your music files.

💡 For better flexibility, store the **full path** of each song when it's added to the playlist.

---

### 🛠 Error Handling
The current code lacks detailed error handling. It does not manage cases such as:
- Pressing **Play** without a selected song.
- Trying to go **Next** or **Prev** beyond the playlist boundaries.

✅ Consider adding `try-except` blocks to gracefully handle such scenarios.

---

### 🎨 User Experience Enhancements
You can enhance the user experience by adding:
- Display of the **currently playing song** title.
- **Volume controls**.
- A **progress bar** showing playback progress.
- **Shuffle** and **repeat** playback options.

---

### 📁 Code Organization
To improve readability and structure:
- Move function definitions to the **top of the script** before they are called.

