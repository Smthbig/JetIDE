# 🚀 JetIDE – Android Development Studio in Your Pocket

> **JetIDE** is a blazing-fast, full-featured Android IDE built for mobile-first developers who want to write, build, and debug Android apps directly on their phone using Termux.

---

## 🎯 Vision

JetIDE aims to **redefine mobile development** by offering a **complete Android Studio-like experience inside Termux**. It’s designed for coders, power users, and students who want to build production-ready Android apps on-the-go — without ever touching a laptop.

---

# But there is a big problem, I have not much time

## 📦 Features

[] **Full Android App Build System**  
[] Kotlin & Java Support (with LSP)  
[] Jetpack Compose & XML layout compatible  
[] Gradle Project Runner & APK Builder  
[] ADB Debugging & Logcat Viewer  
[] Git Integration + GitHub Automation  
[] Offline AI Code Assistant (via llama.cpp / Gemini)  
[] Syntax Highlighting & Formatter  
[] Plugin System (customizable via shell or GUI)  
[] Terminal-Based or WebView GUI Interface  
[] Lightweight & Battery Friendly  

---

## 🔧 Components & Stack

| Component        | Description                                       |
|------------------|---------------------------------------------------|
| **Termux**       | Shell environment & CLI for Android               |
| **OpenJDK 17+**  | Java runtime for compiling apps                   |
| **Android SDK**  | Command line tools, build-tools, platform-tools  |
| **Gradle**       | App project compilation & packaging               |
| **ADB**          | Debugging and live testing                        |
| **Kotlin LSP**   | Kotlin code suggestions (via LSP or Neovim)       |
| **llama.cpp**    | Offline AI coding assistant                       |
| **Prism.js**     | Syntax highlighter in embedded Web IDE            |
| **Zenity/YAD**   | Optional GUI interface for menu & settings        |

---

## 🧪 How It Works

### Termux Setup

- Install JetIDE scripts in Termux
- Fetch Android SDK + platform tools
- Create, import, or edit a Gradle project
- Build APK using `./gradlew assembleDebug`
- Install directly on your device via ADB
- Debug with `logcat` and interactive CLI

### Optional GUI (Web IDE)

- Embedded WebView UI
- JetBrains-like interface using Ace/Monaco
- Plugin support (Formatter, LSP, AI Assist)

---

## 🚀 Getting Started

```bash
# Clone JetIDE installer
git clone https://github.com/yourname/JetIDE.git
cd JetIDE

# One-time setup
bash setup.sh

# Build and install APK
bash build.sh ~/MyApp debug

# Launch debug log
bash debug.sh com.example.myapp
````

---

## 📁 Project Structure
Cli
```
JetIDE/
├── setup.sh         # One-time environment and SDK install
├── build.sh         # Gradle APK builder and installer
├── debug.sh         # Logcat debugger for Android apps
├── ide-ui/          # Web-based UI (Ace/Monaco/Prism.js)
├── plugins/         # Formatters, AI Assist, Git manager, etc.
└── README.md        # You're reading it
```
App
```
com.jetide
│
├── MainActivity.kt            // Root activity with Compose + NavHost
├── ui/
│   ├── screens/
│   │   ├── EditorScreen.kt    // WebView Code Editor
│   │   ├── TerminalScreen.kt  // Terminal UI or termux shell
│   │   ├── GitScreen.kt       // Git operations UI
│   │   └── SettingsScreen.kt  // Theme/API key/settings
│   └── theme/
│       ├── Theme.kt           // Material3 theme definitions
│       └── ColorScheme.kt     // Optional: expanded color definitions
├── ai/
│   └── AiAssistant.kt         // Gemini/OpenAI Kotlin assistant handler
├── git/
│   └── GitManager.kt          // Git shell interface / JGit wrapper
├── formatter/
│   └── Formatter.kt           // KtLint or Spotless integration
├── buildsystem/
│   └── ApkBuilder.kt          // Compile + DEX + APK creation logic
└── plugin/
    └── PluginManager.kt       // Runtime plugin loading
```
---

## 💡 Roadmap

* [ ] Web IDE with full Compose preview
* [ ] Real-time Kotlin LSP engine
* [ ] Plugin manager (formatter, snippet injector)
* [ ] APK Signing and Play Store integration
* [ ] QR code APK installer
* [ ] AI pair programming mode with Gemini

---

## 🤖 AI Assistant Integration

JetIDE supports **offline AI coding** using:

* [`llama.cpp`](https://github.com/ggerganov/llama.cpp)
* Google Gemini or OpenAI ChatGPT API (via WebView or CLI)

Features:

* Code generation
* Context-aware fix suggestions
* File summarization and refactoring

---

## 📲 Demo Screenshots

> *(Coming soon — you can contribute UI mockups or screenshots!)*

---

## 🛠 Requirements

* Android 8.0+ with Termux
* At least 2 GB free space
* Git, curl, unzip
* Internet connection (for initial setup only)

---

## 🧑‍💻 Contributing

JetIDE is in active development. If you’re passionate about mobile coding, shell automation, or open-source Android tools:

```bash
# Fork it, clone it, hack it!
git clone https://github.com/Smthbig/JetIDE.git
```

Please submit PRs, feature requests, or bug reports.

---

## 📜 License

MIT License © 2025 \[mr]

---

## 📣 Acknowledgements

Inspired by:

* Termux community
* Android SDK CLI
* JetBrains IntelliJ
* Llama.cpp / Gemini APIs
* You — the mobile-first developer ❤️

