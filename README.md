
# 📘 Setup Tailwind CSS with CLI

این راهنما نحوه نصب، راه‌اندازی و اجرای Tailwind CSS را با استفاده از **Tailwind CLI** توضیح می‌دهد.

---

## 🌐 لینک‌های ضروری

* **دانلود Node.js:**
  [https://nodejs.org/en/download](https://nodejs.org/en/download)

* **سایت رسمی TailwindCSS:**
  [https://tailwindcss.com/](https://tailwindcss.com/)

---

## 🚀 1. نصب Node.js

پس از نصب Node.js برای بررسی:

```bash
npm -v
```

---

## 📦 2. ایجاد پروژه جدید

در پوشه پروژه:

```bash
npm init
```

فایل `package.json` ساخته می‌شود.

---

## 🎨 3. نصب TailwindCSS و CLI

```bash
npm install tailwindcss @tailwindcss/cli
```

---

## 📁 4. ساخت فایل‌های ورودی و خروجی Tailwind

در مسیر پروژه، یک پوشه `src` بسازید و فایل ورودی CSS ایجاد کنید:

**src/input.css**

```css
@import "tailwindcss";
```

---

## 🗂️ ساختار نهایی پوشه‌ها

```
project/
│
├── src/
│   ├── input.css        # فایل ورودی Tailwind
│   ├── output.css       # فایل خروجی (تولید شده توسط CLI)
│   └── index.html       # فایل HTML پروژه
│
├── package.json         # اطلاعات پروژه و پکیج‌ها
└── node_modules/        # وابستگی‌ها
```

---

## ⚙️ 5. اجرای Tailwind CLI (کامپایل + Watch)

برای ساخت و آپدیت خودکار فایل خروجی:

```bash
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```

---

## 🔁 اجرای مجدد اگر فایل‌ها موجود بودند

اگر فایل‌ها قبلاً ساخته شده‌اند، فقط کافیست همان دستور را اجرا کنید:

```bash
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```

---

## 🧩 6. استفاده از Tailwind در HTML

در فایل **src/index.html**:

```html
<link rel="stylesheet" href="./output.css">
```

نمونه استفاده:

```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

---
