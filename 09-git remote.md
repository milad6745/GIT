دستور `git remote` در Git برای مدیریت remote repositories (مخازن از راه دور) استفاده می‌شود. این دستور امکان نمایش، اضافه کردن، و حذف remote repositories را فراهم می‌کند. زیرا در یک پروژه Git، ممکن است نیاز به همکاری با چندین remote repository داشته باشید. در زیر، توضیحی در مورد استفاده از `git remote` و یک مثال آورده شده است:

### `git remote`:

1. **نمایش remote repositories موجود:**
   ```bash
   git remote
   ```
   - این دستور لیست تمام remote repositories موجود در پروژه را نمایش می‌دهد.

2. **نمایش اطلاعات دقیقتر درباره remote repositories:**
   ```bash
   git remote -v
   ```
   - این دستور لیست تمام remote repositories را به همراه URL آن‌ها نمایش می‌دهد.

3. **افزودن یک remote repository جدید:**
   ```bash
   git remote add origin https://example.com/repo.git
   ```
   - این دستور remote repository با نام `origin` و URL مشخص شده را به پروژه اضافه می‌کند.

4. **حذف یک remote repository:**
   ```bash
   git remote remove origin
   ```
   یا
   ```bash
   git remote rm origin
   ```
   - این دستور remote repository با نام `origin` را از پروژه حذف می‌کند.

**مثال:**

1. **نمایش remote repositories:**
   ```bash
   git remote
   ```
   - این دستور لیست تمام remote repositories موجود را نمایش می‌دهد.

2. **افزودن یک remote repository جدید:**
   ```bash
   git remote add upstream https://example.com/upstream-repo.git
   ```
   - این دستور remote repository با نام `upstream` و URL مشخص شده را به پروژه اضافه می‌کند.

3. **نمایش اطلاعات دقیقتر درباره remote repositories:**
   ```bash
   git remote -v
   ```
   - این دستور لیست تمام remote repositories را به همراه URL آن‌ها نمایش می‌دهد.

در این مثال، remote repository جدید با نام `upstream` اضافه شده و لیست remote repositories با دستور `git remote -v` نمایش داده می‌شود.
