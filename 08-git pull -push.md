دستورات `git push` و `git pull` در Git برای ارسال تغییرات به یک remote repository و دریافت تغییرات از remote repository به repository محلی (local) به کار می‌روند. در زیر، توضیحی در مورد هرکدام از این دستورات و مثال‌های مرتبط آمده است:

### `git push`:

- **توضیح:**
  - `git push` برای ارسال تغییرات اعمال‌شده در repository محلی به یک remote repository استفاده می‌شود.

- **مثال:**
  ```bash
  git push origin main
  ```
  - این دستور تغییرات branch `main` را به remote repository با نام `origin` ارسال می‌کند.

### `git pull`:

- **توضیح:**
  - `git pull` برای دریافت تغییرات از remote repository و ادغام آنها با تغییرات محلی استفاده می‌شود.

- **مثال:**
  ```bash
  git pull origin main
  ```
  - این دستور تغییرات branch `main` از remote repository با نام `origin` را دریافت و با تغییرات محلی ادغام می‌کند.

**نکته:**
- در مثال‌های بالا، `main` به عنوان نام branch استفاده شده است. شما می‌توانید نام branch مورد نظر خود را جایگزین کنید.

**مثال کامل:**

1. **ارسال تغییرات به remote repository:**
   ```bash
   git add .
   git commit -m "Commit message"
   git push origin main
   ```

2. **دریافت تغییرات از remote repository:**
   ```bash
   git pull origin main
   ```
   - این دستور تغییرات از remote repository دریافت و با تغییرات محلی ادغام می‌کند.

استفاده از `git push` و `git pull` برای همگام‌سازی تغییرات بین repository محلی و remote repository یکی از اصول اصلی کار با Git است.s
