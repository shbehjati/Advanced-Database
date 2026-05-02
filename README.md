# پایگاه داده پیشرفته — Advanced Database Systems

سایت درس پایگاه داده پیشرفته برای مقطع کارشناسی ارشد

## 🚀 راه‌اندازی روی GitHub Pages

### مرحله ۱: ایجاد ریپازیتوری

```bash
git init
git remote add origin https://github.com/USERNAME/advanced-db-course.git
```

### مرحله ۲: ساختار پوشه‌ها

```
/
├── index.html          ← فایل اصلی سایت
├── README.md
├── notes/              ← یادداشت‌های درس
│   ├── lecture-01-intro.pdf
│   ├── lecture-02-storage.pdf
│   └── ...
├── assignments/        ← صورت تکالیف
│   ├── hw1.pdf
│   └── ...
├── solutions/          ← حل تکالیف
│   ├── sol1.pdf
│   └── ...
├── quizzes/            ← کوئیزها
│   ├── quiz1.pdf
│   └── ...
└── exams/              ← امتحانات
    ├── midterm.pdf
    └── final.pdf
```

### مرحله ۳: فعال‌سازی GitHub Pages

1. به **Settings** ریپازیتوری بروید
2. بخش **Pages** را انتخاب کنید
3. در **Source** گزینه **Deploy from a branch** را انتخاب کنید
4. شاخه **main** و پوشه **/ (root)** را انتخاب کنید
5. روی **Save** کلیک کنید

سایت شما در آدرس زیر در دسترس خواهد بود:
```
https://USERNAME.github.io/advanced-db-course/
```

## ✏️ افزودن فایل‌های جدید

### افزودن یادداشت درس

۱. فایل PDF را در پوشه `notes/` قرار دهید
۲. در `index.html` آرایه `notesData` را ویرایش کنید:

```javascript
const notesData = [
  {
    title: "جلسه ۱۳: OLAP و Data Warehouse",
    date: "۱۵ اردیبهشت",
    file: "notes/lecture-13-olap.pdf",
    pages: "—"
  },
  // ...
];
```

### افزودن تکلیف

در آرایه `assignmentsData` یک آیتم اضافه کنید:

```javascript
{ title: "تکلیف ۷: ...", date: "مهلت: ...", file: "assignments/hw7.pdf", pages: "—" }
```

### تغییر اطلاعات درس

در بخش hero فایل `index.html` این قسمت‌ها را ویرایش کنید:

```html
<div class="badge">CS Graduate Course — نیمسال دوم ۱۴۰۳–۱۴۰۴</div>
<h1>پایگاه داده پیشرفته</h1>
<p class="hero-sub">دانشگاه — گروه مهندسی کامپیوتر</p>
```

## 📦 دستورات Git برای به‌روزرسانی

```bash
# افزودن فایل‌های جدید
git add notes/lecture-13-olap.pdf
git add index.html

# ثبت تغییرات
git commit -m "add lecture 13 notes"

# ارسال به GitHub
git push origin main
```

GitHub Pages به‌صورت خودکار سایت را به‌روز می‌کند (معمولاً ۱–۲ دقیقه).

## 🎨 شخصی‌سازی

### تغییر رنگ اصلی

در بخش `:root` فایل CSS:
```css
--accent: #4f8ef7;   /* رنگ اصلی آبی */
--accent2: #a78bfa;  /* رنگ بنفش */
--accent3: #34d399;  /* رنگ سبز */
```

### تغییر فونت

```css
font-family: 'Vazirmatn', sans-serif;
```
