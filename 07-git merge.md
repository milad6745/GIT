دستور `git merge` در Git برای ادغام (merge) تغییرات از یک branch به branch دیگر استفاده می‌شود. با استفاده از این دستور، می‌توانید تغییرات اعمال‌شده در یک branch را به branch دیگری اضافه کنید. در زیر، یک مثال از استفاده از `git merge` آورده شده است:

### `git merge`:

1. **ایجاد یک branch فرعی:**
   ```bash
   git branch feature_branch
   git checkout feature_branch
   ```
   یا
   ```bash
   git checkout -b feature_branch
   ```
   - این دستورات یک branch به نام `feature_branch` ایجاد کرده و به آن جابه‌جا می‌شوند.

2. **اعمال تغییرات در branch فرعی:**
   - اعمال تغییرات در فایل‌ها و commit کردن.

3. **بازگشت به branch اصلی (مثلاً `main` یا `master`):**
   ```bash
   git checkout main
   ```
   - با این دستور به branch اصلی باز می‌گردیم.

4. **ادغام تغییرات branch فرعی با branch اصلی:**
   ```bash
   git merge feature_branch
   ```
   - با این دستور، تغییرات اعمال‌شده در `feature_branch` به branch اصلی (`main`) اضافه می‌شوند.

5. **حل تداخل‌ها (conflicts) در صورت وجود:**
   - اگر در ادغام تداخل‌ها وجود داشته باشد، Git از شما خواهد خواست تداخل‌ها را حل کنید و سپس ادامه دهید.

**مثال:**

- فرض کنید تغییراتی در `feature_branch` انجام شده است.
- حالا با دستور `git merge feature_branch` تغییرات این branch به branch اصلی اضافه می‌شوند.

```bash
# ایجاد branch فرعی
git branch feature_branch
git checkout feature_branch

# اعمال تغییرات در feature_branch
# commit تغییرات

# بازگشت به branch اصلی
git checkout main

# ادغام تغییرات از feature_branch به main
git merge feature_branch
```

این مثال نشان می‌دهد چگونه تغییرات اعمال‌شده در یک branch فرعی با استفاده از `git merge` به branch اصلی اضافه می‌شوند.
