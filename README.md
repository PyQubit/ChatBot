# PyQubit AI Chatbot 🤖

**Developer :** Mohammad Mahdi Omidvar

---

## 🌟 Features | امکانات

* AI chatbot powered by **Gemma 3:4b**
* چت‌بات هوشمند با استفاده از **Gemma 3:4b**
* Stores chat history in **SQLite**
* ذخیره تاریخچه پیام‌ها در **SQLite**
* Multi-user support via mobile numbers
* پشتیبانی از چند کاربر با شماره موبایل
* Simple REST API for frontend integration
* API ساده برای اتصال به رابط کاربری
* Supports RTL interface for Persian
* پشتیبانی از رابط راست‌چین برای فارسی

---

## 🛠️ Installation | نصب

### Python Libraries | کتابخانه‌های پایتون

Install required libraries:

```bash
pip install flask flask-cors ollama
```

* `flask` → Web server / سرور وب
* `flask-cors` → AJAX cross-origin support / پشتیبانی AJAX
* `ollama` → AI communication / ارتباط با مدل هوش مصنوعی

---

### AI Model | مدل هوش مصنوعی

Install **Gemma 3:4b** locally:

```bash
ollama pull gemma3:4b
```

* This is the main AI model for the chatbot
* مدل اصلی چت‌بات
* Make sure **Ollama CLI** is installed and working
* حتماً Ollama CLI نصب و فعال باشد

---

## 🚀 How to Run | نحوه اجرا

1. **Run Flask server | اجرای سرور Flask**


2. **Open frontend | باز کردن رابط کاربری**

* Open `index.html` in your browser
* مطمئن شوید AJAX URL به آدرس سرور Flask شما (`http://127.0.0.1:5000`) اشاره می‌کند

---

## 💾 Database | پایگاه داده

* Uses `chatbot.db` (SQLite)
* ذخیره پیام‌های کاربر و پاسخ‌های AI
* Stores last 40 messages per user for context
* ذخیره آخرین ۴۰ پیام برای هر کاربر

---

## 🌐 API

### `GET /`

**Query Parameters | پارامترهای درخواست:**

| Parameter | Type   | Description                             |
| --------- | ------ | --------------------------------------- |
| chat1     | string | User message / پیام کاربر               |
| mobile    | string | User mobile number / شماره موبایل کاربر |

**Response | پاسخ:**

* Returns AI response as HTML-safe text
* بازگشت پاسخ هوش مصنوعی با فرمت HTML

---

## ⚠️ Notes | نکات مهم

* Developer: Mohammad Mahdi Omidvar
* Make sure all Python libraries and Gemma 3:4b model are installed before running
* تمام کتابخانه‌ها و مدل Gemma 3:4b باید قبل از اجرا نصب شده باشند
* Server runs by default on `http://0.0.0.0:5000`

---

## 🎨 Demo | نمونه

**User Input | ورودی کاربر:**

```
Hello, how are you?
```

**AI Response | پاسخ هوش مصنوعی:**

```
Hello! I'm PyQubit AI. How can I assist you today? ✅
```

© 2025 **Mohammad Mahdi Omidvar**
