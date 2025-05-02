# 🛒 ECOMMERCE PLATFORM



A full-featured ecommerce platform built using Django and MySQL, with user authentication, product management, order tracking, and feedback system.


---

## 🧩 Features

### 🧍‍♂️ Customer Functions

* View/search products without login
* Add/remove items to/from cart without login (no duplicates)
* Must login to purchase
* Register and login system
* Simulated payment page (⚠️ do not use real details)
* Track order status (Pending, Confirmed, Delivered)
* Download order invoices
* Send feedback to admin (even without logging in)

### 👨‍💼 Admin Functions

* Admin login via:

```bash
py manage.py createsuperuser
```

* Dashboard showing customer/product/order stats
* Add/Edit/Delete/View Products
* Edit/Delete/View Customer Profiles
* View/Delete Orders
* Update Order Status
* Read Customer Feedback

### 🛠️ Smart Features

* Fraud check: deleting a customer also deletes their orders
* Deleting unavailable products also clears those from orders
* Cart check before purchase to avoid empty orders

---

## ⚙️ Installation Guide

### 1. 📦 Dependencies

Install Python and required packages:

```bash
pip install django==3.0.5
pip install django-widget-tweaks
pip install xhtml2pdf
```

### 2. 💻 Setup

* Download and extract this project
* In terminal:

```bash
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```

* Open browser at:

```
http://127.0.0.1:8000/
```

---

## 📬 Contact Form Setup (for Feedback page)

Edit `settings.py`:

```python
EMAIL_HOST_USER = 'youremail@gmail.com'
EMAIL_HOST_PASSWORD = 'your email password'
EMAIL_RECEIVING_USER = 'youremail@gmail.com'
```

Then enable less secure apps in Gmail:
[https://myaccount.google.com/lesssecureapps](https://myaccount.google.com/lesssecureapps)

---

## ⚠️ Known Issues

* Editing profile logs user out due to credential changes
* Cart popup appears only on logo click (pending fix)

---

## 🙋‍♂️ Contributor

* [Your GitHub Name](https://github.com/LucasCatty)

---

## 💬 Feedback

Suggestions are welcome!

* [https://www.instagram.com/](#)


---

> 🚫 *This project is for academic/demo purposes. Not production-ready.*
