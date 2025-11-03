# 🌐 Flask Basic Website

This is a simple **Flask web application** that demonstrates how to create multiple routes and render HTML templates using Jinja2.

---

## 🚀 Features
- Flask framework with basic routing  
- Separate HTML templates for each page  
- Dynamic titles passed from Flask to HTML  

---

## 🧩 Project Structure
```
future/
│
├── app.py
├── templates/
│   ├── index.html
│   └── about.html
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Create and activate a virtual environment (optional but recommended)
```bash
python -m venv venv
venv\Scripts\activate    # On Windows
source venv/bin/activate # On Mac/Linux
```

### 2️⃣ Install Flask
```bash
pip install flask
```

### 3️⃣ Run the Flask app
```bash
python app.py
```

The app will start at:
```
http://127.0.0.1:5000/
```

---

## 🧠 How It Works

### **Routes**
- `/` → Renders **index.html** (Home page)
- `/about` → Renders **about.html** (About page)

### **Template Rendering**
Each route uses:
```python
return render_template('filename.html', title='PageTitle')
```
Flask automatically looks for HTML files inside the **templates/** directory.

---

## 🧾 Example HTML Template

**templates/index.html**
```html
<!DOCTYPE html>
<html>
<head>
    <title>{{ title }}</title>
</head>
<body>
    <h1>Welcome to {{ title }} Page!</h1>
    <a href="/about">Go to About Page</a>
</body>
</html>
```

---

## 🛠️ Troubleshooting

If you get:
```
jinja2.exceptions.TemplateNotFound: index.html
```
Make sure your HTML files are inside a folder named **templates/** in the same directory as `app.py`.

---

## 👨‍💻 Author
**Vikas Pandit**  
📦 GitHub: [Vikas17554](https://github.com/Vikas17554)

---

## 📜 License
This project is open-source and free to use.
