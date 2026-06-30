# Shared Evidence Contract (ฉบับเริ่มต้น)

โครงการย่อยแต่ละระบบควรสามารถส่งข้อมูลหรือหลักฐานกลับสู่ศูนย์กลาง AUN-QA ได้ในระยะต่อไป โดยเริ่มต้นด้วยการ Export เป็น CSV หรือ JSON ก่อน แล้วจึงพัฒนา REST API เมื่อโครงสร้างข้อมูลนิ่ง

## ฟิลด์ขั้นต่ำ

| Field | ความหมาย | ตัวอย่าง |
|---|---|---|
| `source_system` | รหัสระบบต้นทาง | `P3` |
| `record_id` | รหัสรายการในระบบต้นทาง | `PRJ-2569-001` |
| `title` | ชื่อหลักฐานหรือรายการ | `Project Proposal Approval` |
| `academic_year` | ปีการศึกษา / ภาคเรียน | `2569/1` |
| `related_plo_clo` | PLO/CLO ที่เกี่ยวข้อง | `PLO3, PLO5` |
| `aun_criterion` | เกณฑ์ AUN-QA ที่สนับสนุน | `3, 4, 6, 8` |
| `file_url_or_reference` | ลิงก์ไฟล์/อ้างอิง | `https://...` |
| `evidence_status` | สถานะหลักฐาน | `Draft`, `Submitted`, `Reviewed`, `Approved` |
| `owner` | ผู้รับผิดชอบรายการ | `ทีม P3` |
| `created_at` | วันที่สร้าง | ISO 8601 |
| `updated_at` | วันที่ปรับปรุงล่าสุด | ISO 8601 |

## ตัวอย่าง JSON

```json
{
  "source_system": "P3",
  "record_id": "PRJ-2569-001",
  "title": "Approved Project Proposal",
  "academic_year": "2569/1",
  "related_plo_clo": ["PLO3", "PLO5"],
  "aun_criterion": [3, 4, 6, 8],
  "file_url_or_reference": "https://example.edu/project/PRJ-2569-001/proposal",
  "evidence_status": "Approved",
  "owner": "Project Team 01",
  "created_at": "2026-06-30T00:00:00+07:00",
  "updated_at": "2026-06-30T00:00:00+07:00"
}
```

> ข้อมูลตัวอย่างนี้เป็นข้อมูลสมมติ ห้ามนำข้อมูลส่วนบุคคลหรือเอกสารจริงที่ไม่อนุญาตให้เผยแพร่มาลง repository สาธารณะ
