# 🚀 Android Assignment (Forked & Extended)

> 📦 **Original Repository:** [Android Assignment provided by Miare firm](https://github.com/miare-ir/AndroidAssignment)  
> This repository is a **fork** of the original Miare firm assignment provided for a technical task.  
>  
> 🔧 My version includes:
> - ✨ **Refactoring**
> - 🧠 **Architectural improvements**
> - 🎨 **Modern Jetpack Compose–based UI implementation**
> - 🧪 **Unit & UI tests** for reliability and scalability
>  


> 🔎 Explore my full implementation in the dedicated branch →  
> **[`morz_sheikhi`](https://github.com/MohShMehr/AndroidAssignment/tree/morz_sheikhi)**

---

## 📸 Screenshots

<p align="center">
  <img src="screenshots/splash.png" alt="Splash" width="32%">
  <img src="screenshots/home_dark.png" alt="Home Screen" width="32%">
  <img src="screenshots/followed_players.png" alt="Followed Players Screen" width="32%">
  <img src="screenshots/sort_bt.png" alt="Sort bottom sheet" width="32%">
</p>

<p align="center">
  <em>✨ Material 3 · Dark & Dynamic Theme Supported</em>
</p>

---

## 🧠 About My Implementation

The original codebase served as a starting point.  
In my version, I **redesigned the architecture**, **migrated the UI to Jetpack Compose**, and added **clean, testable, and reactive layers** to make the project production-ready.

### 🧩 Key Enhancements
- 🧱 **Clean Architecture** — clear separation of `data`, `domain`, and `presentation`
- 💉 **Hilt DI** across modules
- 🧭 **Navigation-Compose** for screen transitions
- ⚙️ **State management with ViewModel + StateFlow**
- 🎨 **Jetpack Compose (Material 3)** UI
- 🔄 **Repository pattern** with Retrofit + Room
- 🧪 **Testing-ready** use cases & abstractions

---

## 🏗️ Architecture Overview

This project follows a **Multi-Module Clean Architecture** pattern to achieve scalability, modularity, and testability.

```text
app/
├── Main application module (entry point, DI setup)
├── Depends on feature modules


core/
├── data/ → Repositories & data sources
├── database/ → Room entities & DAO
├── designsystem/ → Shared UI components & themes
├── domain/ → UseCases & domain models
├── model/ → Core shared models
├── network/ → Retrofit, API interfaces
└── ui/ → Shared Compose utilities


feature/
├── followedplayers/ → Feature module for managing followed players
└── home/ → Feature module for home screen & list display
```


✅ **Benefits:**
- Independent **feature modules** for better build times and separation of concerns  
- **Core modules** shared across all features (network, data, design system, etc.)  
- Highly **scalable** for adding new features  
- Easier **testing and maintenance** with clear boundaries  
- Supports both **unit** and **UI testing**

---

## ⚙️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| **Architecture** | Multi-Module · Clean Architecture · MVI |
| **UI** | Jetpack Compose · Material 3 · Design System Module - Paging 3|
| **DI** | Hilt |
| **Async / Reactive** | Kotlin Coroutines · Flow · StateFlow |
| **Network** | Retrofit · Jakson |
| **Database** | Room |
| **Testing** | JUnit · MockK · Espresso · Compose UI Tests |
| **Build / Tools** | Gradle (KTS) · Version Catalogs · Kotlin DSL |
| **Modularity** | Core / Feature separation for scalability |

---

> 🧠 The modular structure allows isolated development of each feature while keeping shared logic centralized in `core/`, ensuring both **code reusability** and **build performance optimization**.

## 🌿 Branches

| Branch | Description |
|-------|-------------|
| `main` | Original company assignment (unmodified) |
| [`morz_sheikhi`](https://github.com/MohShMehr/AndroidAssignment/tree/morz_sheikhi) | My improved implementation with Compose + Clean Architecture |

To check out my branch:
```bash
git checkout morz_sheikhi



