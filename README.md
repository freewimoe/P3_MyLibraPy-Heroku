# MyLibraPy (CLI Version)

A simple command-line app for managing your personal library.
This version of the app is intended to be run as a Python script and is deployed on **Heroku as a worker dyno**.

---

## 📦 Features

- Add books to your collection
- View and search your books
- Edit and delete entries
- Export to CSV
- View statistics by genre and reading status

---

## 🚀 Deployment

### ✅ Live Deployment (Heroku)

⚠️ **Note:** This is a CLI (Command Line Interface) app. It runs on Heroku as a background process (worker) and does not expose a web interface.

🔗 **Heroku app:**  
[https://mylibrapy-cli.herokuapp.com/](https://mylibrapy-cli.herokuapp.com/)  
👉 This will show an error if accessed via browser – that's expected for CLI apps.

---

## 📁 Repository

The source code is available on GitHub:

🔗 [https://github.com/freewimoe/P3_MyLibraPy-Heroku](https://github.com/freewimoe/P3_MyLibraPy-Heroku)

---

## 🛠️ How Heroku Runs This CLI App

Heroku doesn't support interactive input like `input()` in a terminal.  
This app is deployed with a `Procfile` that defines:

worker: python my_libra.py

This starts the app as a **worker dyno**.

---

## 🧪 Testing

The app cannot be interacted with via Heroku UI.

If you'd like to run the app locally:

```bash
git clone https://github.com/freewimoe/P3_MyLibraPy-Heroku.git
cd P3_MyLibraPy-Heroku
pip install -r requirements.txt
python my_libra.py

## 📌 Notes for Reviewers
This project is the CLI version of MyLibraPy, following the PP3 assignment requirements.

The Heroku app is only used to demonstrate deployment capability – it cannot receive user input in a hosted environment.

All required functionality is implemented and tested locally.

## 👨‍💻 Author
Friedrich-Wilhelm Möller
Code Institute Student 2025