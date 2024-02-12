# `git stash`

اگر فایل‌هایی در پروژه شما وجود دارند که به Git افزوده نشده‌اند (untracked files) و شما می‌خواهید آنها را در یک stash موقت ذخیره کنید، می‌توانید از `git stash` استفاده کنید. در اینجا یک مثال برای این حالت آورده شده است:

1. فرض کنید چند فایل جدید ایجاد کرده‌اید که به Git افزوده نشده‌اند:

   ```bash
   touch file1.txt
   touch file2.txt
   ```

2. حالا چک کنید که فایل‌های جدید به Git افزوده نشده‌اند:

   ```bash
   git status
   ```

   خروجی شما ممکن است مشابه زیر باشد:

   ```bash
   Untracked files:
     (use "git add <file>..." to include in what will be committed)

         file1.txt
         file2.txt
   ```

3. حالا از `a- git stash` برای ذخیره فایل‌های untracked استفاده کنید:

   ```bash
   git stash -a
   ```

   این دستور stash فایل‌های untracked را در یک stash موقت ذخیره می‌کند.

4. حالا می‌توانید به شاخه دیگری بروید یا تغییرات دیگری اعمال کنید.

5. برای بازیابی فایل‌های untracked از stash:

   ```bash
   git stash apply
   ```

   یا اگر می‌خواهید stash را حذف کنید:

   ```bash
   git stash pop
   ```

   با این دستورات، تغییرات untracked شما از stash بازیابی می‌شوند.
