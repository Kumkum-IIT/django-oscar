# Django Oscar Project

This repository contains an e-commerce project built using **Django Oscar**, a powerful and extensible framework for building e-commerce applications in Django.

---

## 🛒 Overview

Django Oscar provides a modular, domain-driven architecture that allows developers to customize almost every component of the system. This project uses Oscar’s core apps (catalogue, basket, checkout, dashboard, payments, etc.) along with third‑party integrations.

---

## 🚀 Features

* Fully featured e‑commerce foundation using Django Oscar
* Modular and extensible architecture
* Separate dashboard interface for admin management
* Built‑in apps for catalogue, checkout, orders, users, payments, shipping, vouchers, reviews, offers, and more
* Customizable models and views via Oscar’s overriding mechanism
* Third‑party utilities:

  * `widget_tweaks`
  * `haystack`
  * `treebeard`
  * `sorl-thumbnail`
  * `django_tables2`

---

## 🗂️ Project Structure

* **oscar_project/** – Main project folder

  * `settings.py` – Contains Django + Oscar app configuration
  * `urls.py` – URL router integrating Oscar’s URLs
  * `wsgi.py` / `asgi.py` – Deployment entry points
* **manage.py** – Django management CLI
* **requirements.txt** – Dependency list

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <repo-url>
cd django-oscar
```

### 2. Create and activate a virtual environment

```bash
python -m venv env
source env/bin/activate  # Windows: env\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run migrations

```bash
python manage.py migrate
```

### 5. Start development server

```bash
python manage.py runserver
```

Visit:
**Frontend:** [http://127.0.0.1:8000](http://127.0.0.1:8000)
**Dashboard:** [http://127.0.0.1:8000/dashboard/](http://127.0.0.1:8000/dashboard/)

---

## 🧩 Customization

Django Oscar allows overriding:

* models
* templates
* forms
* views
* dashboard modules

This project can be extended by creating a new app and letting Oscar pick it up using `OSCAR_REQUIRED_APPS` and `OSCAR_OPTIONAL_APPS`.

---

## 📝 Notes

* Ensure database (SQLite/Postgres) is properly configured in `settings.py`.
* Some Oscar features (like search) require search backend setup (Haystack + Elasticsearch/Solr).
* For production, additional setup (static files, WSGI server, cache, secure settings) is needed.

---

## 🤝 Contributing

Pull requests and issue reports are welcome.

---

## 📄 License

This project uses the open-source Django Oscar license terms.
