# JetIDE
A modern IDE for Android app development on Android Mobile 
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
    
# Contribute Please in it
