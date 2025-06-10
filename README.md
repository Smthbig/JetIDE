ok# 🚀 JetIDE – Android Development Studio in Your Pocket

> **JetIDE** is a blazing-fast, full-featured Android IDE built for mobile-first developers who want to write, build, and debug Android apps directly on their phone — through a powerful **CLI (Termux)** or rich **Jetpack Compose UI**.

---

## 🎯 Vision

JetIDE redefines mobile app development by delivering a **complete Android Studio alternative** that fits in your pocket. It’s crafted for developers, power users, and learners who want to build **production-grade Android apps anytime, anywhere** — without needing a PC.

---

## 📦 Feature Overview

✅ Dual Mode: **CLI in Termux** + **Native Android App**  
✅ Kotlin & Java Language Support (with LSP support in roadmap)  
✅ Jetpack Compose & XML layout compatible  
✅ Full Android Build Toolchain (Gradle + AAPT + DEX)  
✅ APK Installer & QR Sharing  
✅ ADB Debugging & Logcat Viewer  
✅ Git Integration & GitHub CLI Automation  
✅ Offline AI Assistant (LLaMA.cpp / Gemini / OpenAI)  
✅ Syntax Highlighting (via Prism.js / Monaco)  
✅ Formatters (ktlint / spotless / shell formatter plugins)  
✅ Plugin System for extensibility (via GUI or shell)  
✅ Battery-efficient, ultra-lightweight footprint

---

## 🔧 Architecture & Stack

| Component        | Description                                       |
|------------------|---------------------------------------------------|
| **Termux**       | Shell + environment for CLI-based workflows       |
| **OpenJDK 17+**  | Java runtime for compiling Android apps           |
| **Android SDK**  | Build-tools, platform-tools, ADB, etc.            |
| **Gradle**       | Project automation and APK building               |
| **ADB**          | Device deployment and debugging                   |
| **LSP / Neovim** | Code intelligence and syntax support (WIP)        |
| **llama.cpp**    | Local/offline AI assistant (code generation)      |
| **Gemini API**   | Optional cloud-based assistant (secure via token) |
| **Jetpack Compose** | Rich UI for the native app IDE                 |
| **Prism.js / Monaco** | Syntax highlighting in WebView IDE          |
| **Zenity / YAD** | Optional GUI dialogs for plugin launcher (CLI)    |

---

## 🧪 How It Works

### 💻 CLI Mode (via Termux)

1. Install Termux + JetIDE scripts
2. Auto-install Android SDK, NDK, OpenJDK
3. Create or import your Gradle project
4. Run `./gradlew assembleDebug` to build
5. Install APK directly to device via ADB
6. Debug using `logcat`, `debug.sh`, or emulator shell

### 📱 App Mode (Native Android IDE)

1. Use embedded WebView-based editor (CodeMirror/Monaco)
2. Write code in Kotlin/Java with syntax highlighting
3. Run LLM-backed AI assistant for suggestions
4. Build APK via `ApkBuilder.kt` or invoke CLI under the hood
5. Git, format, or preview Compose — all in-app

---

## 🚀 Getting Started

```bash
# 1. Clone JetIDE installer (Termux CLI mode)
git clone https://github.com/yourname/JetIDE.git
cd JetIDE

# 2. Run one-time environment setup
bash setup.sh

# 3. Build and install your app
bash build.sh ~/MyApp debug

# 4. Debug logs with ADB
bash debug.sh com.example.myapp
````

---

## 📁 Project Structure

### CLI Side (Termux)

```
JetIDE/
├── setup.sh         # One-time Android SDK, JDK, Gradle install
├── build.sh         # APK builder and deployer
├── debug.sh         # ADB logcat viewer + debugger
├── ide-ui/          # WebView UI (Ace/Monaco/Prism.js)
├── plugins/         # Formatters, AI Assist, Git manager, etc.
└── README.md
```

### Native App (Android IDE)

```
com.jetide/
├── MainActivity.kt            # Root Compose-based IDE shell
├── ui/
│   ├── screens/
│   │   ├── EditorScreen.kt    # WebView code editor with Prism
│   │   ├── TerminalScreen.kt  # Embedded shell or CLI interface
│   │   ├── GitScreen.kt       # GitHub/Git UI and config
│   │   └── SettingsScreen.kt  # API key, theme, layout prefs
│   └── theme/
│       ├── Theme.kt           # Material 3 colors and typography
│       └── ColorScheme.kt     # Dark/light scheme support
├── ai/
│   └── AiAssistant.kt         # Gemini / LLaMA.cpp integration
├── git/
│   └── GitManager.kt          # Git commands & repo manager
├── formatter/
│   └── Formatter.kt           # Source formatting engine
├── buildsystem/
│   └── ApkBuilder.kt          # Gradle + AAPT + DEX builder logic
└── plugin/
    └── PluginManager.kt       # Plugin injection system
```

---

## 🧠 AI Assistant Integration

JetIDE supports **offline and online AI assistants**:

| Model          | Mode    | Use Cases                        |
| -------------- | ------- | -------------------------------- |
| **llama.cpp**  | Offline | Full privacy, no internet needed |
| **Gemini API** | Online  | Rich, contextual LLM assistance  |
| **OpenAI API** | Online  | GPT-4/3.5 powered answers        |

### Features:

* Code generation / completion
* Smart fix suggestions
* File summarization & refactoring
* Prompt injection via plugin or button

---

## 📲 Demo Screenshots

*(Coming soon — contribute UI mockups or screenshots!)*

---

## 📅 Roadmap

* [ ] Web IDE with Compose live preview
* [ ] Kotlin LSP integration via Neovim or LSP bridge
* [ ] Plugin marketplace (formatters, snippets, helpers)
* [ ] APK signing + Play Store deploy CLI
* [ ] QR code APK installer + sharer
* [ ] Gemini-powered pair programming mode

---

## 🛠 Requirements

* Android 8.0+ (ARM64 recommended)
* Termux latest version (F-Droid preferred)
* \~2 GB free space for SDK + tools
* Git, curl, unzip installed
* Internet (for setup or Gemini/OpenAI API)

---

## 🧑‍💻 Contributing

JetIDE is open-source and in active development. If you're into mobile dev tools, CLI automation, or Kotlin/Compose magic:

```bash
# Clone and start building
git clone https://github.com/yourname/JetIDE.git
```

Feel free to send pull requests, report bugs, or suggest features!

---

## 📜 License

> MIT License Copyright (c) 2025 Smthbig
 Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


---

## 🙏 Acknowledgements

Inspired by:

* Termux community
* Jetpack Compose & Android SDK CLI
* JetBrains IntelliJ + Android Studio
* Gemini, GPT-4, and LLaMA.cpp projects
* You — the mobile-first developer ❤️



