# แนวทางจัดการ Source Code ของแต่ละทีม

Repository `se-aunqa-projects` เป็น **Project Hub กลาง** สำหรับเอกสารร่วม ภาพ mockup และมาตรฐานกลาง เพื่อให้ข้อมูลของ P1–P6 ไม่กระจัดกระจาย

## ทางเลือกที่แนะนำ

ให้แต่ละทีมสร้าง repository ของตนเองสำหรับ source code เช่น

```text
se-aunqa-p1-evidence-workbench
se-aunqa-p2-plo-clo-mapping
se-aunqa-p3-student-project-journey
se-aunqa-p4-lab-readiness
se-aunqa-p5-active-learning
se-aunqa-p6-stakeholder-insight
```

แต่ละทีมต้องใส่ลิงก์ย้อนกลับมายัง Project Hub นี้ใน README ของทีม และทำตามข้อกำหนดร่วมเรื่อง MVP, Test, Documentation และ Evidence Package

## กรณีใช้ repository เดียว

หากผู้สอนต้องการให้ใช้ repository เดียว ให้สร้างโฟลเดอร์แยกดังนี้

```text
projects/
├── P1-evidence-workbench/
├── P2-plo-clo-mapping/
├── P3-student-project-journey/
├── P4-lab-readiness/
├── P5-active-learning/
└── P6-stakeholder-insight/
```

ข้อดีคือดูภาพรวมง่าย ข้อควรระวังคือ CI/CD, dependency และสิทธิ์การแก้ไขอาจซับซ้อนขึ้นเมื่อหลายทีมทำงานพร้อมกัน
