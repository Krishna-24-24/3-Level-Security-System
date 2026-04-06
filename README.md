# 🔐 3-Level Security System

> A simple, interactive multi-step authentication system built with HTML, CSS, and JavaScript that validates different types of inputs at each security level.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## 🌐 Live Demo

**[https://Krishna-24-24.github.io/3-Level-Security-System/](https://Krishna-24-24.github.io/3-Level-Security-System/)**

---

## 📌 About the Project

This project simulates a **3-step authentication process** using pure HTML, CSS, and JavaScript. Each level tests a different type of user input — from credential validation to math-based captcha to binary conversion — making it a fun and educational demonstration of logical flow and dynamic web behavior.

---

## 🔒 Security Levels

### Level 1 — Login
- User enters a **username and password**
- Credentials are validated against fixed demo values
- On success: proceeds to Level 2
- On failure: shows an **"Invalid Credentials"** alert

> Demo credentials → Username: `Krishna` | Password: `24BCE0592`

---

### Level 2 — Math Captcha
- A **random math expression** is generated (e.g., `7 + 9`)
- User must evaluate and enter the correct answer
- A **Refresh Captcha** button generates a new expression using `Math.random()`
- On success: proceeds to Level 3
- On failure: shows an **"Invalid Captcha"** alert

---

### Level 3 — Decimal to Binary Conversion
- A **random decimal number** is generated (between 5–14)
- User must convert it to its **binary equivalent**
- Validation uses JavaScript's built-in `.toString(2)` method
- On success: shows the **Success Screen** 🎉
- On failure: shows a **"Wrong binary value"** alert

---

### ✅ Success Screen
After passing all three levels, a green success box is displayed confirming **Access Granted**.

---

## 🖼️ Screenshots

| Level 1 — Login | Level 2 — Captcha |
|----------------|------------------|
| Username & password fields | Random math expression to evaluate |

| Level 3 — Binary | Success Screen |
|-----------------|----------------|
| Convert decimal to binary | Green "Access Granted" box |

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| **HTML5** | Structure and layout |
| **CSS3** | Styling, colors, level differentiation |
| **JavaScript** | Logic, validation, random generation |

---

## ⚙️ How It Works

```
User visits page
       ↓
  Level 1: Enter username & password
       ↓ (correct)
  Level 2: Solve random math captcha
       ↓ (correct)
  Level 3: Convert decimal to binary
       ↓ (correct)
  ✅ Access Granted!
```

Each level is a hidden `div` that becomes visible only after the previous level is passed. Wrong answers show an alert and keep the user on the current level.

---

## 📂 Project Structure

```
3-Level-Security-System/
├── index.html     # All HTML, CSS, and JavaScript in one file
└── README.md
```

---

## ✨ Key Concepts Demonstrated

- DOM manipulation with `getElementById` and `style.display`
- Input validation and conditional logic
- `Math.random()` for dynamic captcha and binary challenges
- `.toString(2)` for decimal to binary conversion
- Multi-step UI flow without any frameworks or libraries

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
