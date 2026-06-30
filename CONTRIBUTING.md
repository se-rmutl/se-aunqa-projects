# แนวทางการมีส่วนร่วม (Contributing)

## ก่อนเริ่มงาน

1. อ่าน Project Brief ของโครงการที่รับผิดชอบ
2. สร้าง Issue หรือแจ้งงานที่ทำให้ชัดเจน
3. แยกงานเป็น branch ของตนเอง
4. ห้าม commit ข้อมูลส่วนบุคคล รหัสผ่าน API key หรือข้อมูลแบบสอบถามจริง

## การตั้งชื่อ branch

```text
feature/p3-proposal-workflow
fix/p4-qr-search-ui
docs/p2-mapping-rules
```

## การตั้งชื่อ commit

```text
feat(p3): add proposal submission workflow
fix(p4): handle empty QR asset search
docs(p1): clarify evidence status definitions
```

## Pull Request ขั้นต่ำ

ทุก Pull Request ควรระบุ:

- ปัญหาหรือเป้าหมายของการเปลี่ยนแปลง
- สิ่งที่แก้ไขหรือเพิ่ม
- วิธีทดสอบ
- ภาพหน้าจอหรือ Demo URL เมื่อเป็นงาน UI
- ผลกระทบต่อ Evidence Package / AUN-QA (ถ้ามี)

## คุณภาพขั้นต่ำก่อนส่งงานปลายภาค

- README การติดตั้งและใช้งาน
- Sample data ที่ไม่ใช่ข้อมูลจริง
- Test cases สำหรับ workflow หลัก
- สรุปขอบเขตที่ทำแล้วและงานที่เลื่อนทำในอนาคต
