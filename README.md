# 🔋 DualSense Battery Widget

![Languages](https://img.shields.io/github/languages/count/cardi83/PS5-Battery-Widget) ![Top Language](https://img.shields.io/github/languages/top/cardi83/PS5-Battery-Widget) ![Last Commit](https://img.shields.io/github/last-commit/cardi83/Ps5-Battery-Widget)

A floating desktop widget built by **Chris Cardi** to monitor the battery status of a connected **PlayStation 5 DualSense controller** in real time — featuring customizable appearance, transparency toggle, and auto-refreshing status updates via USB or Bluetooth.

## 📖 Overview

This PyQt6-based widget provides:

* Live monitoring of controller connection and charging state
* Accurate battery percentage when connected via USB
* A customizable and draggable user interface
* Seamless transparency toggle and color customization

This project demonstrates practical Python GUI design, device interfacing with `hidapi`, and efficient use of system resources for real-time hardware status tracking.

---

## 📁 Contents

| File                            | Description                                                |
| ------------------------------- | ---------------------------------------------------------- |
| `dualsense_battery_widget.py` | Main script containing the PyQt6 GUI and HID polling logic |
| `README.md`                   | This file                                                  |

---

## 🛠️ Requirements

* Python 3.9+
* [PyQt6](https://pypi.org/project/PyQt6/)
* [hid](https://pypi.org/project/hid/)

---

## [⬛️]>_ Usage

Launch the widget with:

```
python dualsense_battery_widget.py
```

The widget will:

* Float on your desktop (frameless + always-on-top)
* Auto-refresh every 3 seconds
* Display one of the following statuses:
  * 🎮 **Wired** + 🔋 Battery %
  * 🎮 **Wired** + 🔋 Charging ⚡
  * 🎮 **Bluetooth** (Battery unknown)
  * 🎮 **Not Connected**

Right-click the widget to:

* Toggle transparency
* Change background color
* Exit the application

---

## 📌 Notes

* Battery readings are  **only accurate via USB** . Bluetooth mode does not report precise battery levels -- that is faulty by design and it is not currently possible to estimate accurate battery levels via Bluetooth signal.
* Designed for **PlayStation 5 DualSense** controllers with known vendor/product IDs.
* Tested on Windows with Python 3.13.

---

## 💡 Future Ideas

* System tray integration
* Minimized widget view (compact mode)
* Audio/visual low battery alert
