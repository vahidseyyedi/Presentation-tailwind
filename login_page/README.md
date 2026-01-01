![](./detail/Screenshot%202025-12-05%20173736.png)
---

## 1️⃣ تگ `<body>`

```html
<body class="bg-[#174993] flex items-center justify-center min-h-screen font-byekan">
```

| کلاس             | توضیح                                               |
| ---------------- | --------------------------------------------------- |
| `bg-[#174993]`   | رنگ پس‌زمینه کل صفحه (آبی سفارشی)                   |
| `flex`           | فعال‌سازی Flexbox                                   |
| `items-center`   | تراز عمودی محتوا در مرکز                            |
| `justify-center` | تراز افقی محتوا در مرکز                             |
| `min-h-screen`   | حداقل ارتفاع برابر با کل ارتفاع صفحه                |
| `font-byekan`    | فونت سفارشی (احتمالاً در Tailwind config تعریف شده) |

📌 نتیجه: فرم دقیقاً وسط صفحه قرار می‌گیرد.

---

## 2️⃣ کانتینر اصلی (کارت لاگین)

```html
<div class="bg-white rounded-2xl shadow-2xl flex w-full max-w-4xl overflow-hidden m-2.5">
```

| کلاس              | توضیح                      |
| ----------------- | -------------------------- |
| `bg-white`        | پس‌زمینه سفید              |
| `rounded-2xl`     | گوشه‌های بسیار گرد         |
| `shadow-2xl`      | سایه بزرگ و عمیق           |
| `flex`            | چیدمان افقی ستون‌ها        |
| `w-full`          | عرض 100٪                   |
| `max-w-4xl`       | حداکثر عرض (حدود 896px)    |
| `overflow-hidden` | مخفی کردن محتوای بیرون‌زده |
| `m-2.5`           | مارجین اطراف کارت          |

---

## 3️⃣ بخش تصویر (سمت راست در دسکتاپ)

```html
<div class="hidden md:flex md:w-1/3 items-center justify-center bg-gray-100">
```

| کلاس             | توضیح                                 |
| ---------------- | ------------------------------------- |
| `hidden`         | مخفی در موبایل                        |
| `md:flex`        | از سایز md به بالا نمایش به صورت flex |
| `md:w-1/3`       | یک‌سوم عرض در دسکتاپ                  |
| `items-center`   | مرکز عمودی                            |
| `justify-center` | مرکز افقی                             |
| `bg-gray-100`    | پس‌زمینه خاکستری روشن                 |

📌 این بخش فقط در دسکتاپ دیده می‌شود.

---

### تصویر

```html
<img class="max-h-96 max-w-full object-contain">
```

| کلاس             | توضیح                   |
| ---------------- | ----------------------- |
| `max-h-96`       | حداکثر ارتفاع           |
| `max-w-full`     | عرض حداکثری 100٪        |
| `object-contain` | حفظ نسبت تصویر بدون برش |

---

## 4️⃣ بخش فرم ورود

```html
<div class="w-full md:w-2/3 p-8">
```

| کلاس       | توضیح                |
| ---------- | -------------------- |
| `w-full`   | تمام عرض در موبایل   |
| `md:w-2/3` | دو‌سوم عرض در دسکتاپ |
| `p-8`      | پدینگ داخلی زیاد     |

---

## 5️⃣ عنوان فرم

```html
<h2 class="text-2xl font-bold text-gray-800 mb-6 text-center">
```

| کلاس            | توضیح           |
| --------------- | --------------- |
| `text-2xl`      | اندازه متن بزرگ |
| `font-bold`     | فونت ضخیم       |
| `text-gray-800` | رنگ متن تیره    |
| `mb-6`          | فاصله پایین     |
| `text-center`   | وسط‌چین         |

---

## 6️⃣ فرم و فاصله فیلدها

```html
<form class="space-y-4">
```

| کلاس        | توضیح                        |
| ----------- | ---------------------------- |
| `space-y-4` | فاصله عمودی بین تمام فرزندان |

---

## 7️⃣ لیبل‌ها

```html
<label class="block text-gray-600 mb-1">
```

| کلاس            | توضیح               |
| --------------- | ------------------- |
| `block`         | نمایش در یک خط کامل |
| `text-gray-600` | رنگ خاکستری         |
| `mb-1`          | فاصله پایین کم      |

---

## 8️⃣ اینپوت‌ها

```html
<input class="w-full px-4 py-2 border border-gray-300 rounded-lg
focus:outline-none focus:ring-2 focus:ring-[#174993] focus:border-transparent">
```

| کلاس                       | توضیح                      |
| -------------------------- | -------------------------- |
| `w-full`                   | عرض کامل                   |
| `px-4 py-2`                | پدینگ افقی و عمودی         |
| `border`                   | فعال‌سازی کادر             |
| `border-gray-300`          | رنگ کادر                   |
| `rounded-lg`               | گوشه‌های گرد               |
| `focus:outline-none`       | حذف outline پیش‌فرض        |
| `focus:ring-2`             | حلقه فوکوس                 |
| `focus:ring-[#174993]`     | رنگ حلقه فوکوس             |
| `focus:border-transparent` | مخفی شدن بوردر هنگام فوکوس |

---

## 9️⃣ دکمه ورود اصلی

```html
<button class="w-full bg-[#f7c009] text-white py-2 rounded-lg
hover:bg-[#e98022] transition-colors duration-300 font-semibold">
```

| کلاس                 | توضیح             |
| -------------------- | ----------------- |
| `bg-[#f7c009]`       | پس‌زمینه زرد      |
| `text-white`         | متن سفید          |
| `hover:bg-[#e98022]` | تغییر رنگ در هاور |
| `transition-colors`  | انیمیشن رنگ       |
| `duration-300`       | مدت انیمیشن       |
| `font-semibold`      | فونت نیمه ضخیم    |

---

## 🔟 دکمه ورود از دولت

```html
<button class="bg-white text-gray-900 border border-gray-900
hover:bg-[#174993] hover:text-white">
```

| کلاس                 | توضیح                 |
| -------------------- | --------------------- |
| `bg-white`           | پس‌زمینه سفید         |
| `border`             | کادر                  |
| `hover:bg-[#174993]` | تغییر رنگ در هاور     |
| `hover:text-white`   | تغییر رنگ متن در هاور |

---

## 1️⃣1️⃣ لینک بازیابی رمز

```html
<p class="text-center text-gray-500 mt-4">
<a class="text-gray-800 hover:underline hover:text-[#174993]">
```

| کلاس                   | توضیح          |
| ---------------------- | -------------- |
| `text-center`          | وسط‌چین        |
| `text-gray-500`        | رنگ متن        |
| `hover:underline`      | خط زیر متن     |
| `hover:text-[#174993]` | تغییر رنگ لینک |

---

