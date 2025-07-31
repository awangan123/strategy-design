# 🤖 Robot Behavior Simulation using Strategy Design Pattern in C++

This repository demonstrates the **Strategy Design Pattern** in C++ by modeling different behaviors for robots (like walking, talking, and flying) using interchangeable strategy classes.

---

## 🧩 Design Pattern Used

**Strategy Pattern**:  
Encapsulates behaviors into separate classes (strategies), allowing you to change a robot's behavior at runtime without altering its class.

---

## 📁 Project Structure


---

## 🚀 Features

- Modular behavior interfaces:
  - `WalkableRobot`: Walking behavior
  - `TalkableRobot`: Talking behavior
  - `FlyableRobot`: Flying behavior
- Multiple concrete behavior implementations:
  - `NormalWalk`, `NoWalk`
  - `NormalTalk`, `NoTalk`
  - `NormalFly`, `NoFly`
- Robot types:
  - `CompanionRobot`
  - `WorkerRobot`
- Flexible runtime behavior assignment

---

## 🛠️ How It Works

Each robot is composed of behavior interfaces rather than hardcoding functionality. For example:

```cpp
Robot* robot1 = new CompanionRobot(new NormalWalk(), new NormalTalk(), new NoFly());
Walking normally...
Talking normally...
Cannot fly.
Displaying friendly companion features...
--------------------
Cannot walk.
Cannot talk.
Flying normally...
Displaying worker efficiency stats...
