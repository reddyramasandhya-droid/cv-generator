# 📄 CV Generator

> Capstone Project 3 · Full Stack Python Internship at [CodingBrains](https://codingbrains.in)

A Django web app where a user fills in a simple form and gets a ready-to-use CV as a PDF.

🔗 **Live Demo:** https://ramasandhyareddy377.pythonanywhere.com
💻 **Source Code:** https://github.com/reddyramasandhya-droid/cv-generator

---

## 📌 Overview
Writing a CV from scratch is slow, and formatting it is even slower. I built this project to solve that: enter your details once, and the app turns them into a clean, formatted CV. It is the third capstone project of my Full Stack Python internship, and it is my first project that combines form handling, PDF generation and live deployment.

## ✨ Features
- Easy form with fields for Name, Email, Mobile, About, Degree, University, School, Previous Work and Skills
- Formatted CV generated from the submitted details
- PDF export using `pdfkit`
- Deployed and publicly accessible on PythonAnywhere

## 🛠️ Tech Stack
| Layer | Technology |
|---|---|
| Backend | Python 3.12+, Django 6.1 |
| PDF generation | pdfkit, wkhtmltopdf |
| Frontend | HTML, CSS |
| Database | SQLite |
| Hosting | PythonAnywhere |

## 📂 Project Structure
```
cv-generator/
├── manage.py
├── requirements.txt
├── resume/          # project settings and URL configuration
└── app/             # views, templates and forms
```

## ⚙️ Getting Started

**Prerequisites:** Python 3.12 or newer, and [wkhtmltopdf](https://wkhtmltopdf.org/downloads.html) for PDF export.

```bash
# 1. Clone the repository
git clone https://github.com/reddyramasandhya-droid/cv-generator.git
cd cv-generator

# 2. Create and activate a virtual environment
python -m venv env
env\Scripts\activate           # Windows
source env/bin/activate        # macOS / Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set up the database and run the server
python manage.py migrate
python manage.py runserver
```
Then open http://127.0.0.1:8003/ in your browser.

## 🚀 Deployment on PythonAnywhere
1. Clone the repo in a Bash console.
2. Create a virtualenv with Python 3.12+: `mkvirtualenv --python=/usr/bin/python3.13 cv-env`
3. Install packages: `pip install -r requirements.txt`
4. On the **Web** tab, set the source code path, virtualenv path and WSGI file.
5. Run `python manage.py migrate` and `python manage.py collectstatic`.
6. Click **Reload**.

## 📚 What I Learned
- Building a Django project end to end: models, views, forms and templates
- Turning user input into a formatted document and exporting it as a PDF
- Managing dependencies with `requirements.txt` and virtual environments
- Deploying a Django app to a live server and fixing real deployment errors
- Using Git and GitHub to keep local and server code in sync

## 🧩 Challenges I Faced
- **Dependency setup on the server:** I fixed `requirements.txt` problems and matched the Python version on PythonAnywhere to what Django needs.
- **Git conflicts on the server:** a local edit blocked `git pull`. I learned to make changes on GitHub and pull them, not edit files on the server.
- **PDF generation:** `pdfkit` depends on an external tool (`wkhtmltopdf`), so I had to handle it separately from `pip` packages.

## 🔮 Future Improvements
- Multiple CV templates to choose from
- User login to save and edit CVs
- Live preview before downloading
- Input validation and a mobile-friendly layout

## 📸 Screenshots
| Form | 

<img width="1830" height="905" alt="Image" src="https://github.com/user-attachments/assets/514ace2d-a43a-43ed-b83f-1d4710b247c5" /> 
| Generated CV|<img width="1097" height="722" alt="Image" src="https://github.com/user-attachments/assets/16ba3105-67d7-417b-a5b2-a6a58d4f6069" /> 

## 👩‍💻 Author
**Somula Rama Sandhya**
BTech AIML (2024–2028), Presidency University, Bangalore
📧 reddyramasandhya@gmail.com · 🐙 [GitHub](https://github.com/reddyramasandhya-droid)
