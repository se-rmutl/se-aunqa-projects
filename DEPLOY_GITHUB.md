# การนำ Repository ขึ้น GitHub

## 1. สร้าง Repository บน GitHub

สร้าง repository ใหม่ในองค์กร `se-rmutl` ด้วยชื่อ:

```text
se-aunqa-projects
```

เลือก **ไม่ต้อง** เพิ่ม README / `.gitignore` / License ในหน้า GitHub เพราะ ZIP นี้มีไฟล์เหล่านี้แล้ว

## 2. Push จากโฟลเดอร์ที่แตก ZIP

```bash
git status
git remote -v
git push -u origin main
```

Remote `origin` ถูกตั้งไว้ล่วงหน้าเป็น:

```text
https://github.com/se-rmutl/se-aunqa-projects.git
```

## 3. เปิด GitHub Pages

ไปที่ **Settings → Pages** แล้วกำหนด:

- Source: Deploy from a branch
- Branch: `main`
- Folder: `/ (root)`

จากนั้นหน้า catalog จะเข้าผ่าน:

```text
https://se-rmutl.github.io/se-aunqa-projects/
```
