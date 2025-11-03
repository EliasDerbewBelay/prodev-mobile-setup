Here’s a well-structured `README.md` tailored to your Expo Router setup task:

---

# 📱 First React Native App with Expo Router

This project documents the setup and scaffolding process of a mobile application using the **Expo Router** template. It also includes observations from running the `reset-project` command to better understand the development environment.

---

## 🎯 Objective

- Scaffold a new Expo project using the **Expo Router** template.
- Modify the home screen to personalize the app.
- Run and test the application on a physical device using **Expo Go**.
- Understand the purpose and effect of the `reset-project` command.

---

## 🛠️ Setup Steps

### 1. Navigate to Project Directory

```bash
cd prodev-mobile-setup
```

### 2. Initialize the Project

```bash
npx create-expo-app@latest .
```

- Selected the **Expo Router** template during setup.
- Installed all required dependencies automatically.

### 3. Modify the Home Screen

- Opened the file: `app/(tabs)/index.tsx`
- Located the default text: `Welcome!`
- Replaced it with:
  ```tsx
  <Text>First App Created</Text>
  ```

### 4. Run the Application

```bash
npx expo start
```

- **iOS**: Scanned the QR code using the Camera app.
- **Android**: Scanned the QR code using the **Expo Go** app.
- The app launched successfully on the physical device with the updated home screen text.

---

## 🔄 Resetting the Project

### Command Used

```bash
npm run reset-project
```

### Observations

- The command cleared the Metro bundler cache and reset the development environment.
- It helped resolve issues like stale builds or unexpected runtime behavior.
- After resetting, the app recompiled cleanly and ran without issues.
- No project files or code were deleted — only the cache and temporary build artifacts were cleared.

---

## 📁 File Structure Overview

```
prodev-mobile-setup/
├── app/
│   ├── (tabs)/           # Tab-based navigation screens
│   │   └── index.tsx     # Home screen (modified)
│   └── _layout.tsx       # Navigation layout
├── assets/               # Images, fonts, etc.
├── node_modules/         # Installed dependencies
├── package.json          # Project metadata and scripts
├── tsconfig.json         # TypeScript configuration
└── README.md             # Project documentation
```

---

## ✅ Summary

This setup provides a solid foundation for building scalable mobile apps using **React Native + Expo Router**. The `reset-project` command is a helpful tool for maintaining a clean development environment, especially when debugging.
