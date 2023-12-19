# git branch
دستور `git branch` در Git برای مدیریت و مشاهده branch‌ها استفاده می‌شود. زیرا این دستور امکان ایجاد، حذف، نمایش و جابه‌جایی بین branch‌ها را فراهم می‌کند. در زیر، توضیحی در مورد استفاده از `git branch` برای ساخت و جابه‌جایی بین branch‌ها آمده است:

### `git branch`:

1. **ساخت یک branch جدید:**
   ```bash
   git branch new_branch_name
   ```
   - این دستور یک branch با نام `new_branch_name` ایجاد می‌کند. اما برای جابه‌جایی به آن branch نیاز به دستور جداگانه `git checkout` یا `git switch` دارید.

2. **نمایش لیست تمام branch‌ها:**
   ```bash
   git branch
   ```
   - این دستور لیست تمام branch‌های موجود را نمایش می‌دهد. branch فعلی با یک `*` نشان داده می‌شود.

3. **جابه‌جایی به یک branch دیگر:**
   ```bash
   git checkout branch_name
   ```
   یا
   ```bash
   git switch branch_name
   ```
   - این دستور به branch دیگری جابه‌جا می‌شود. از نسخه Git 2.23 به بعد، توصیه می‌شود از `git switch` به جای `git checkout` استفاده کنید.

4. **ساخت و جابه‌جایی به branch جدید به یک دستور:**
   ```bash
   git switch -c new_branch_name
   ```
   یا
   ```bash
   git checkout -b new_branch_name
   ```
   - این دستور همزمان یک branch جدید ایجاد می‌کند و به آن branch جابه‌جا می‌شود.

**نکته:**
- از `git switch` به جای `git checkout` برای جلوگیری از ابهامات استفاده کنید، زیرا `git switch` برای جابه‌جایی بین branch‌ها بهتر عیب‌یابی شده است.
