# 🎵 Music Player in C

A console-based Music Player implemented in C using a **Circular Doubly Linked List** for playlist management and the **Windows Multimedia API (MCI)** for audio playback.

## 📌 Features

* Add songs to the playlist
* Delete songs from the playlist
* Display all songs in the playlist
* Play the current song
* Pause and resume playback
* Stop playback
* Navigate to the next song
* Navigate to the previous song
* Circular playlist traversal
* Dynamic memory allocation for playlist management

---

## 🛠 Technologies Used

* C Programming Language
* Circular Doubly Linked List Data Structure
* Windows Multimedia API (`mmsystem.h`)
* Dynamic Memory Management

---

## 📂 Data Structure

The playlist is implemented using a **Circular Doubly Linked List**.

Each node stores:

```c
typedef struct Node {
    char path[PATH_LEN];
    struct Node *prev;
    struct Node *next;
} Node;
```

### Advantages

* Efficient traversal in both forward and backward directions
* Circular nature enables continuous playlist looping
* Easy insertion and deletion of songs

---

## 🎮 Available Commands

| Command | Description        |
| ------- | ------------------ |
| a       | Add a song         |
| d       | Delete a song      |
| l       | Display playlist   |
| p       | Play current song  |
| u       | Pause song         |
| r       | Resume song        |
| s       | Stop song          |
| n       | Play next song     |
| b       | Play previous song |
| q       | Quit application   |

---

## 🚀 How to Run

### Requirements

* Windows Operating System
* GCC Compiler (MinGW) or any C Compiler supporting Windows APIs

### Compilation

```bash
gcc music_player.c -o music_player -lwinmm
```

### Execution

```bash
music_player.exe
```

---

## 📋 Example Usage

```text
Enter command: a
Enter song filename or path:
C:\Music\song1.mp3

Added: C:\Music\song1.mp3

Enter command: p
Playing: C:\Music\song1.mp3

Enter command: n
Playing: C:\Music\song2.mp3
```

---

## ⚙️ Functional Modules

### Playlist Management

* Add Song
* Delete Song
* Display Playlist

### Playback Controls

* Play
* Pause
* Resume
* Stop

### Navigation

* Next Song
* Previous Song

---

## 🧠 Concepts Demonstrated

* Circular Doubly Linked Lists
* Dynamic Memory Allocation
* File Path Handling
* Multimedia Programming in C
* Windows API Integration
* Menu-Driven Console Applications

---

## 🔮 Future Enhancements

* Shuffle Playlist
* Repeat Mode
* Volume Control
* MP3 Metadata Display
* Playlist Save/Load Feature
* Graphical User Interface (GUI)
* Song Search Functionality

---

## 📜 License

This project is developed for educational and learning purposes.

---

## 👨‍💻 Author
Kuppa Vijaya Sankari
Developed as a Data Structures and C Programming project demonstrating the implementation of a Music Playlist Manager using Circular Doubly Linked Lists.
