# Arduino Keypad Alarm System

A simple Arduino alarm system using a 4x4 keypad, password authentication, buzzer, and alarm zones.

## Features

- Password protected arming/disarming
- 4x4 keypad input
- Buzzer and LED alarm output
- Entry/Exit delay zone
- Instant trigger zone
- Serial monitor feedback

---

## Components Used

- Arduino Uno/Nano
- 4x4 Matrix Keypad
- Active Buzzer
- Push buttons or sensors
- Jumper wires
- Breadboard

---

## Libraries

Install these libraries in the Arduino IDE:

- Keypad
- Password

---

## Pin Setup

| Component | Pin |
|---|---|
| Keypad Rows | A0-A3 |
| Keypad Columns | A4-A7 |
| ON/OFF Input | 2 |
| Entry/Exit Zone | 11 |
| Zone 1 | 12 |
| Buzzer | 4 |
| LED | 13 |

---

## Default Password

```cpp
1234
```

---

## How It Works

1. System powers on and waits for the correct password.
2. After entering the password, the alarm arms after a 5 second countdown.
3. If a zone is triggered:
   - LED flashes
   - Buzzer sounds
4. Enter the correct password to disarm the system.

---

## Keypad Controls

| Key | Function |
|---|---|
| 0-9 | Enter password |
| # | Confirm password |
| * | Clear password input |

---

## Future Improvements

- LCD display
- RFID support
- EEPROM password saving
- Motion sensors
- RTC logging
- Solenoid lock integration

---

## Uploading

1. Open the `.ino` file in the Arduino IDE.
2. Install required libraries.
3. Select the correct board and COM port.
4. Upload to the Arduino.

---

## Serial Monitor Example

```text
Alarm will arm in 5 seconds.
ARMED
```

```text
OK.
```

```text
Wrong password!
```
