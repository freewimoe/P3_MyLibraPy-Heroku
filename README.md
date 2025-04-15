# 📚 MyLibraPy (CLI Version)

A simple command-line app for managing your personal library.  
This version is designed to be run as a Python script and is deployed on **Heroku as a worker dyno**.

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

⚠️ **Note:** This is a CLI (Command Line Interface) app. It runs on Heroku as a background process (worker) and does **not** expose a web interface.

🔗 **Heroku app:**  
[https://mylibrapy-cli.herokuapp.com/](https://mylibrapy-cli.herokuapp.com/)  
👉 This will show an error if accessed via browser – that's expected for CLI apps.

---

## 📁 Repository

The source code for this deployment is available on GitHub:

🔗 [https://github.com/freewimoe/P3_MyLibraPy-Heroku](https://github.com/freewimoe/P3_MyLibraPy-Heroku)

You can also find:

- 🔹 The original CLI version:  
  [https://github.com/freewimoe/P3_MyLibraPy](https://github.com/freewimoe/P3_MyLibraPy)

- 🔹 An experimental Flask version (non-assessed):  
  [https://mylibrapy-flask-f0d2bbe3d176.herokuapp.com/](https://mylibrapy-flask-f0d2bbe3d176.herokuapp.com/)

---

## 🛠️ How Heroku Runs This CLI App

Heroku doesn't support interactive CLI apps (like `input()`) in a browser context.

This app is deployed using a `Procfile` that tells Heroku to launch:

```
worker: python my_libra.py
```

This launches the app as a **worker dyno**, which is suitable for background processes, not web frontends.

---

## 🧪 Local Testing

Since interactive CLI apps don't work via browser, you can run the app locally:

```bash
git clone https://github.com/freewimoe/P3_MyLibraPy-Heroku.git
cd P3_MyLibraPy-Heroku
pip install -r requirements.txt
python my_libra.py
```

---

## 📌 Notes for Reviewers

This project represents the **CLI version** of MyLibraPy and follows all requirements of the PP3 assignment brief.  
The Heroku deployment is included to demonstrate deployment skills, even though Heroku cannot accept live user input for CLI apps.  

All logic and features are fully functional and tested in a local environment.

---

## 👨‍💻 Author

**Friedrich-Wilhelm Möller**  
Code Institute Student – 2025 Cohort  
Germany 🇩🇪