# طريقة الشغل في المستودع

## القاعدة الذهبية
**لا أحد يرفع مباشرة على `main`.** كل شغل يمشي كذا:

```
Issue  →  Branch  →  Commits  →  Pull Request  →  مراجعة من زميل  →  Merge
```

## 1) قبل ما تبدأ
- اختر مهمتك من لوحة المشروع (Projects) وحط نفسك **Assignee** على الـIssue.
- اسحب آخر نسخة:
  ```bash
  git checkout main
  git pull
  ```

## 2) افتح فرع باسم واضح
```bash
git checkout -b docs/12-problem-statement      # نوع/رقم-الـIssue-وصف-قصير
```
الأنواع: `docs/` كتابة · `research/` بحث · `design/` تصميم · `feat/` كود · `fix/` إصلاح · `data/` بيانات

## 3) اكتب Commits واضحة
```bash
git add .
git commit -m "docs: add problem statement draft (#12)"
git push -u origin docs/12-problem-statement
```
اكتب رقم الـIssue في الرسالة `(#12)` عشان ينربط تلقائي.

## 4) افتح Pull Request
- اكتب في الوصف `Closes #12` عشان تنقفل المهمة لحالها بعد الدمج.
- اطلب مراجعة من زميل واحد على الأقل.
- بعد الموافقة → **Squash and merge** ثم احذف الفرع.

## ممنوعات
- ❌ رفع بيانات كبيرة (صور أقمار، GeoTIFF، ملفات > 50MB) — حطها في Google Drive وحط الرابط في `data/README.md`.
- ❌ رفع مفاتيح أو ملفات `.env` أو credentials حق Earth Engine.
- ❌ أسماء أو بيانات شخصية من المقابلات — ملخصات بدون أسماء فقط.
- ✅ أي استخدام لـClaude أو أي أداة AI يتسجل في `ai-log/ai-usage-log.md`.
