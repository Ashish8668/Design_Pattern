# Smart Home Design Patterns Project

This repository contains a small Java project demonstrating common design patterns used to build a simple smart home system (factory, proxy and basic device abstraction).

**Files Included**
- `Device.java`: Core device interface/abstraction.
- `DeviceFactory.java`: Factory to create concrete device instances.
- `DeviceProxy.java`: Proxy implementation to control access to devices.
- `AirConditioner.java`, `DoorLock.java`, `Fan.java`, `Light.java`: Concrete device implementations.
- `SmartHomeHub.java`: Hub that manages devices (usage of factory/proxy).
- `SmartHomeApp.java`: Example application / entry point that runs the demo.

**Overview**
This project demonstrates how to structure simple device classes and apply the Factory pattern to instantiate devices and the Proxy pattern to manage access/control. It is implemented in plain Java with no external dependencies.

**Prerequisites**
- Java Development Kit (JDK) 8 or newer installed and available on your `PATH`.
- (Optional) Visual Studio Code with Java extensions for development and debugging.

**Clone the repository**
Use the repository URL to clone locally (replace the URL if your repo is hosted somewhere else):

```powershell
git clone https://github.com/Ashish8668/Design_Pattern.git
cd Design_Pattern
```

If you're working from the existing local folder (`DP_Project`), skip cloning and open that folder in VS Code instead.

**Compile & Run (PowerShell / Terminal)**
From the project root where the `.java` files are located, run:

```powershell
javac *.java
java SmartHomeApp
```

If you prefer to compile into an output directory first:

```powershell
javac -d out *.java
java -cp out SmartHomeApp
```

**Run in Visual Studio Code**
- Open VS Code and choose `File` → `Open Folder...` then select the project folder (e.g., `Design_Pattern` or your local `DP_Project`).
- Install the recommended Java extensions (for example: **Language Support for Java(TM) by Red Hat**, **Debugger for Java**, and **Java Test Runner**).
- Ensure your `JAVA_HOME` is set and VS Code detects the JDK (check the Java configuration in the status bar).
- To run the app:
  - Open `SmartHomeApp.java` and use the Run Code / Play button provided by the Java extension, or
  - Open an integrated terminal in VS Code and run the `javac` / `java` commands shown above.
- To debug, create or use the Java debug configuration (VS Code will often offer to create one automatically when you run/debug a Java file).

**Project Notes**
- This repo is educational: it focuses on illustrating patterns and is intentionally small and dependency-free.
- You can extend the project by adding more device types, persisting device states, or adding a GUI or REST API.

**License & Contribution**
- Contributions or improvements are welcome — open a PR or edit locally.
