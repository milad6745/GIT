
---

### ✅ مقدمه: Git چیست؟
Git نرم‌افزاری است که به توسعه‌دهندگان کمک می‌کند تا تغییرات کد را ذخیره، پیگیری، مقایسه و بازگردانی کنند. Git بیشتر در کنار GitHub، GitLab یا Bitbucket استفاده می‌شود.

---

## 📦 نصب Git
### Windows:
1. برو به [git-scm.com](https://git-scm.com)
2. روی "Download for Windows" کلیک کن و نصبش کن.
3. Git Bash هم نصب میشه که ترمینال مخصوص Git هست.

### Linux (Ubuntu):
```bash
sudo apt update
sudo apt install git
```

### Mac:
```bash
brew install git
```

---

## 🔧 پیکربندی اولیه
```bash
git config --global user.name "اسم شما"
git config --global user.email "ایمیل شما"
```

---

## 🧪 دستورات مهم Git (به ترتیب یادگیری)

### 1. ساخت مخزن (Repository)
```bash
git init
```

### 2. اضافه کردن فایل‌ها
```bash
git add filename
# یا همه فایل‌ها
git add .
```

### 3. ثبت تغییرات
```bash
git commit -m "توضیح درباره تغییر"
```

### 4. مشاهده وضعیت فایل‌ها
```bash
git status
```

### 5. مشاهده تاریخچه تغییرات
```bash
git log
```

---

## 🌐 کار با مخازن ریموت (مثل GitHub)

### 1. اتصال به GitHub
```bash
git remote add origin https://github.com/username/repo.git
```

### 2. ارسال به سرور (push)
```bash
git push -u origin main
```

### 3. دریافت آخرین تغییرات
```bash
git pull origin main
```

---

## 🧠 سایر دستورات مفید

| دستور | کاربرد |
|-------|--------|
| `git clone` | کپی کردن یک مخزن |
| `git branch` | مدیریت شاخه‌ها |
| `git checkout` | تغییر شاخه یا رفتن به نسخه خاص |
| `git merge` | ترکیب شاخه‌ها |
| `git diff` | مقایسه تغییرات |

---


---

## 🧵 مدیریت شاخه‌ها (Branches)

### ساخت شاخه جدید
```bash
git branch new-branch
```

### رفتن به شاخه دیگر
```bash
git checkout new-branch
```

### ساخت و رفتن به شاخه جدید هم‌زمان
```bash
git checkout -b feature-x
```

### لیست شاخه‌ها
```bash
git branch
```

### ادغام (Merge) شاخه‌ها
فرض کنیم در شاخه `feature-x` تغییراتی انجام داده‌اید و می‌خواهید آن را به `main` ببرید:
```bash
git checkout main
git merge feature-x
```

### حذف شاخه
```bash
git branch -d feature-x
```

---

## 🔁 بازگردانی تغییرات

### 1. بازگردانی فایل به آخرین نسخه کامیت‌شده:
```bash
git checkout -- filename
```

### 2. لغو آخرین commit (بدون حذف تغییرات)
```bash
git reset --soft HEAD~1
```

### 3. لغو commit همراه با حذف تغییرات:
```bash
git reset --hard HEAD~1
```

---

## 🕵️‍♂️ بررسی تفاوت‌ها

### بین فایل تغییر کرده و نسخه‌ی ذخیره‌شده:
```bash
git diff filename
```

### بین دو commit:
```bash
git diff commit1 commit2
```

---

## 📥 کلون کردن مخزن (Clone)
اگر پروژه‌ای روی GitHub هست:
```bash
git clone https://github.com/username/repo.git
```

---

## 🧩 کار با `.gitignore`
برای نادیده‌گرفتن فایل‌ها (مثلاً فایل‌های پیکربندی محلی یا فایل‌های لاگ)، از `.gitignore` استفاده می‌کنیم:

مثال محتوای فایل `.gitignore`:
```
*.log
node_modules/
.env
```

---

## 🔄 تغییر نام یا حذف فایل

### تغییر نام:
```bash
git mv oldname.txt newname.txt
```

### حذف فایل:
```bash
git rm file.txt
```

---

## 🚀 کار با Remote و چندین شاخه

### دریافت تغییرات ریموت بدون ادغام
```bash
git fetch origin
```

### دیدن شاخه‌های ریموت
```bash
git branch -r
```

---

## 🧪 stash کردن تغییرات (وقتی موقتاً نمی‌خواهی commit کنی)

ذخیره موقت:
```bash
git stash
```

بازگردانی تغییرات:
```bash
git stash pop
```

لیست stashes:
```bash
git stash list
```

---

## 📌 Git Tag (نسخه‌گذاری)

### ایجاد تگ:
```bash
git tag v1.0
```

### ارسال تگ به ریموت:
```bash
git push origin v1.0
```

---

ا
