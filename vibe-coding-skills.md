---
marp: true
theme: default
paginate: true
size: 16:9
header: 'vibe coding @ CPMatch'
style: |
  @import url('https://fonts.googleapis.com/css?family=Google+Sans:400,500,700&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+Thai:wght@400;500;600;700&family=JetBrains+Mono:wght@400;700&display=swap');
  :root {
    --brand: #F5273E; --amber: #E07B00; --green: #059669;
    --ink: #1A1A1E; --muted: #5b5b66; --faint: #9a9aa6;
    --line: #E6E6EC; --card: #F7F7F9; --code: #F2F2F6;
  }
  section {
    font-family: 'Google Sans','Noto Sans Thai',-apple-system,'Segoe UI',sans-serif;
    font-size: 24px; color: var(--ink); background: #ffffff;
    padding: 54px 62px; line-height: 1.5;
  }
  h1 { color: var(--ink); font-size: 44px; letter-spacing: -.5px; margin: 0 0 .2em; }
  h2 { color: var(--ink); font-size: 33px; margin: 0 0 .3em; }
  h3 { color: var(--ink); font-size: 25px; font-weight: 600; }
  h4 { color: var(--brand); font-size: 20px; margin: 0 0 .25em; }
  strong { color: var(--brand); }
  em { color: var(--muted); }
  a { color: var(--brand); }
  code { font-family: 'JetBrains Mono',monospace; font-size: .82em; color: var(--brand); background: var(--code); padding: 1px 5px; border-radius: 4px; }
  pre { background: #1c1c22; border: 1px solid #2a2a33; border-radius: 10px; padding: 16px 18px; font-size: 16px; line-height: 1.45; }
  pre code { color: #e6e6ec; background: none; padding: 0; }
  table { font-size: 19px; border-collapse: collapse; width: 100%; }
  th { background: var(--brand); color: #fff; font-weight: 600; }
  td, th { border: 1px solid var(--line); padding: 7px 12px; text-align: left; }
  tr:nth-child(even) td { background: var(--card); }
  blockquote { border-left: 5px solid var(--amber); background: #fff8ee; padding: 10px 18px; color: var(--ink); font-size: .92em; border-radius: 0 8px 8px 0; }
  header { color: var(--faint); font-size: 13px; }
  ul, ol { margin: .2em 0; }
  li { margin: .15em 0; }
  img { border-radius: 12px; }
  .mono { font-family: 'JetBrains Mono',monospace; color: var(--brand); letter-spacing: 2px; font-size: 15px; font-weight: 700; }
  .muted { color: var(--muted); }
  .amber { color: var(--amber); font-weight: 700; }
  .green { color: var(--green); font-weight: 700; }
  .red   { color: var(--brand); font-weight: 700; }
  .cols  { display: grid; grid-template-columns: 1fr 1fr; gap: 26px; align-items:center; }
  .card  { background: var(--card); border: 1px solid var(--line); border-radius: 10px; padding: 14px 18px; }
  .card-brand { border: 1.5px solid var(--brand); background:#fff; }
  .card-amber { border: 1.5px solid var(--amber); background:#fff; }
  .card-green { border: 1.5px solid var(--green); background:#fff; }
  .bar { display: flex; border-radius: 8px; overflow: hidden; font-weight: 700; margin: .3em 0 .6em; }
  .bar > div { padding: 12px 16px; color:#fff; }
  .flow { font-family:'JetBrains Mono',monospace; font-weight:700; color:var(--brand); font-size:18px; }
  .pill { font-weight:700; font-size:.8em; padding:2px 10px; border-radius:999px; }
  .pill-done { background:#e7f6ef; color:var(--green); }
  .pill-wip  { background:#fdf3e3; color:var(--amber); }
  .pill-todo { background:#fdeaec; color:var(--brand); }
  .buzz span { display:inline-block; background:#fdeaec; border:1px solid #f6c9cf; color:#c01528; font-weight:700; font-size:.78em; padding:4px 11px; border-radius:999px; margin:3px 4px 0 0; }
  section.lead { justify-content: center; }
  section.lead h1 { font-size: 52px; }
  section.lead h3 { color: var(--muted); font-weight: 600; }
  section.painpoint { background:#fbf5ee; }
  section.divider { background:#0e0e14; color:#fff; justify-content:center; }
  section.divider h1, section.divider h2 { color:#fff; }
  section.divider p { color:#c4c4d0; }
  section.divider .secnum { font-family:'JetBrains Mono',monospace; font-size:84px; color:var(--brand); font-weight:700; line-height:1; }
  section.divider .mono { color:#ff8a96; }
---

<!-- _class: lead -->
<!-- _paginate: false -->
<!-- _header: '' -->

<span class="mono">WORKSHOP · CPMatch</span>

# ทักษะที่ทำให้ “เก่ง” ขึ้น

### สิ่งที่แยก *vibe coding เล่นสนุก* ออกจาก **ใช้กับงานจริง**

---

<!-- _class: painpoint -->

<span class="mono">// vibe coding ที่ทำผิด</span>

## เร็ว… แต่พังเงียบ ๆ

<div class="cols">
<div>

<span class="buzz"><span>หนี้โค้ด</span> <span>บั๊กที่มองไม่เห็น</span> <span>ช่องโหว่หลุด</span> <span>merge มั่ว</span> <span>ไม่มีใครเข้าใจโค้ด</span></span>

</div>
<div>

![w:560](bg_painpoint.png)

</div>
</div>

---

<span class="mono">// AGENDA</span>

## วันนี้เราจะไปทางไหน

| # | หัวข้อ |
|---|---|
| 1 | ภาพรวม + 4 ทักษะ vibe coding |
| 2 | **Context Engineering** ← ใจกลาง |
| 3 | gstack 30 วินาที → ตัวอย่างจริง: ระบบฐานข้อมูลพนักงาน |
| 4 | Vibe QA: กำกับ AI เขียน test |
| 5 | Multi-agent: ใช้ AI เป็นทีม (PO) |
| 6 | สำหรับหัวหน้าทีม vibe coding |
| 7 | นำไปใช้ · เครื่องมือ · ปิดท้าย |

---

<!-- _class: divider -->

<span class="secnum">01</span>

<span class="mono">SECTION</span>

## ภาพรวม + 4 ทักษะ

vibe coding คืออะไร และทักษะอะไรบ้างที่เปลี่ยน “เล่นสนุก” ให้เป็น “งานจริง”

---

<span class="mono">// ภาพรวม · vibe coding</span>

## vibe coding คืออะไร — แล้วทำไมต้องฝึก

*บอก AI ว่า “อยากได้อะไร” แล้วมันเขียนโค้ดให้ — เราขับด้วย **intent** ไม่ใช่พิมพ์เองทุกบรรทัด*

<div class="cols">
<div class="card card-green">

#### เล่นสนุก = ทำได้ทันที
พิมพ์สั้น ๆ ก็ได้ของเลย เหมาะกับลองไอเดีย · prototype · งานเล็กที่พังก็ไม่เป็นไร

</div>
<div class="card card-amber">

#### งานจริง = ไม่ง่ายแบบนั้น
codebase ใหญ่ + ทำกันเป็นทีม + ต้องขึ้น production → ปล่อยตามใจ AI = พังแบบเงียบ ๆ

</div>
</div>

> **AI เขียนเร็วขึ้นหลายเท่า** — แต่ถ้าคุมไม่เป็น มันก็สร้างบั๊ก / หนี้โค้ด / ช่องโหว่ ได้เร็วขึ้นหลายเท่าเหมือนกัน

4 ทักษะถัดไป คือสิ่งที่เปลี่ยน *“เล่นสนุก”* ให้กลายเป็น **“ใช้กับงานจริงได้”**

---

<span class="mono">// ROADMAP · 4 ทักษะ + เซฟตี้</span>

## 4 ทักษะที่แยก “เล่นสนุก” ออกจาก “งานจริง”

*แต่ละทักษะแก้ปัญหาหนึ่งที่ AI มักทำพังเวลาเจองานจริง*

<div class="cols">
<div>

**01 · Context engineering** — ป้อนบริบทที่ถูก
<span class="muted">ปัญหา: AI เห็นแค่ไฟล์ที่เปิด เลยเดาโครงสร้าง/กฎผิด</span>
**ทักษะ:** เขียน rule file (`CLAUDE.md`) commit เข้า repo

**02 · สั่งแบบ spec ไม่ใช่ vibe**
<span class="muted">ปัญหา: สั่งคลุมเครือ → AI เดา edge case/security เองมั่ว</span>
**ทักษะ:** ระบุ input·output·เงื่อนไข + “วางแผนก่อน”

</div>
<div>

**03 · วินัยการ review**
<span class="muted">ปัญหา: โค้ด AI ดูดีแต่ผิดได้ · ที่ merge = คุณเป็นเจ้าของ</span>
**ทักษะ:** อ่าน diff ทุกบรรทัด + รันจริงเช็ก

**04 · รู้จัก 70% problem**
<span class="muted">ปัญหา: AI พาไป ~70% แต่ 30% สุดท้ายมันตัน</span>
**ทักษะ:** กำงานสำคัญ (security·architecture) ไว้คุมเอง

</div>
</div>

> **เซฟตี้ · Git hygiene** — commit เล็ก commit บ่อย เวลา AI หลุดโลกจะย้อนกลับได้ในก้าวเดียว

---

<!-- _class: divider -->

<span class="secnum">02</span>

<span class="mono">SECTION · ใจกลาง workshop</span>

## Context Engineering

ป้อนบริบทที่ใช่ให้ AI รู้จักโปรเจกต์ของคุณ — ทักษะที่ใช้เวลามากที่สุดวันนี้

---

<span class="mono">01 / CONTEXT ENGINEERING</span>

## บริบทดี = ผลลัพธ์ดี

*agent รู้แค่สิ่งที่อยู่ใน context — บริบทห่วย = ผลห่วย ไม่เกี่ยวว่าโมเดลเก่งแค่ไหน*

<div class="cols">
<div class="card card-amber">

#### ถ้าไม่ให้บริบท → AI พลาด
- **เดา convention ผิด** — ตั้งชื่อ/วางไฟล์ไม่ตรงทีม
- **สร้างไฟล์ผิด layer** — วาง logic ผิดที่
- **ละเมิดกฎที่มองไม่เห็น** — commit เอง · แก้ migration เก่า
- **reinvent** — เขียน util / component ซ้ำของที่มี

</div>
<div class="card card-green">

#### ป้อนบริบทให้ดี → ทำไง
- **rule file commit เข้า repo** — `CLAUDE.md`/`AGENTS.md`
- **ชี้ไฟล์ให้ตรง** — `@file` / ระบุ path อย่าให้เดา
- **“ใช่” ไม่ใช่ “เยอะ”** — ไฟล์ไม่เกี่ยวเจือจางโมเดล
- **ให้ตรวจงานเองได้** — บอกคำสั่ง test/lint · `/clear` เมื่อ session รก

</div>
</div>

> **ราก:** model เก่ง generate แต่ไม่รู้จัก codebase คุณ — เห็นแค่ไฟล์ที่เปิดในรอบนั้น

---

<span class="mono">// PART 2 · CONTEXT ENGINEERING</span>

## Prompt engineering ต่างกับ Context engineering ยังไง

*ทั้งคู่คือการ “บอกบริบท” ให้ AI — ต่างกันที่บอกครั้งเดียวจบ หรือบอกไว้ให้ใช้ซ้ำได้ตลอด*

| | Prompt engineering | Context engineering |
|---|---|---|
| **เก็บไว้ที่ไหน** | พิมพ์สดในแชต ครั้งต่อครั้ง | ไฟล์ในโปรเจกต์ที่ commit ลง repo |
| **อยู่ได้นานแค่ไหน** | หายไปเมื่อปิดแชต | อยู่ถาวร ใช้ซ้ำได้ทุก session |
| **ใครได้ใช้** | เฉพาะคนที่พิมพ์ตอนนั้น | ทั้งทีม + AI ทุกตัว + คนมาทีหลัง |
| **พอโปรเจกต์โตขึ้น** | ต้องพิมพ์ย้ำเองซ้ำ ๆ | เขียนครั้งเดียว AI โหลดให้เอง |

> พูดง่าย ๆ: **context file = เอกสาร onboarding ของ AI** — ถ้าต้องอธิบายเรื่องเดิมซ้ำทุก session แปลว่ามันควรย้ายไปอยู่ในไฟล์

---

<span class="mono">// PART 2 · CONTEXT ENGINEERING</span>

## README ≠ context file

<div class="cols">
<div class="card">

### README.md
*ผู้อ่าน: มนุษย์ · ตอบ “ติดตั้ง/รันยังไง”*

- prerequisites · install
- build / test
- license · contributing

</div>
<div class="card card-brand">

### CONTEXT.md
*ผู้อ่าน: AI agent · ตอบ “ทำงานในโค้ดนี้ยังไงให้ถูก”*

- architecture & layer rules
- naming convention เป๊ะ ๆ
- recipe เพิ่ม feature · gotchas

</div>
</div>

**README ของ CLI boilerplate = ไร้ค่าต่อ AI — ความรู้จริงอยู่ใน `CONTEXT.md`**

---

<span class="mono">// PART 2 · CONTEXT ENGINEERING</span>

## 3 layers — แยกตามความถี่ที่เปลี่ยน

<div class="cols">
<div>

![w:440](bg_layers.png)

</div>
<div>

**3 · FEATURE** — `CONTEXT_<feature>.md`
กำลังทำอะไร · เสร็จ/ค้างตรงไหน · <span class="red">เปลี่ยนทุกวัน</span>

**2 · ARCHITECTURE** — `CONTEXT.md`
codebase ทำงานยังไง · recipe · <span class="amber">เปลี่ยนตอน refactor</span>

**1 · ENTRY** — `CLAUDE.md`
“อ่านอะไรก่อน” + กฎเหล็ก · <span class="green">เปลี่ยนนาน ๆ ครั้ง</span>

</div>
</div>

*บน (แดง) เปลี่ยนบ่อย → ล่าง (เทา) durable · แยกไฟล์ตามความถี่ → AI โหลดเฉพาะที่ใช้ ไม่ stale ทั้งก้อน*

---

<span class="mono">// PART 2 · LAYER 1</span>

## Layer 1 · ENTRY — เขียนครั้งเดียว ทุก AI อ่านเจอ

*ไฟล์ entry บาง ๆ ที่ชี้ไป CONTEXT.md + กฎเหล็ก · เขียน source เดียว แล้ว mirror ลงทุกชื่อ*

<div class="cols">
<div>

```text
# CLAUDE.md   <!-- mirror → AGENTS.md · อย่าแก้มือ -->
อ่านก่อน: @CONTEXT.md (สถาปัตยกรรม + recipe)

## Hard rules
- ห้าม git commit เอง · ถามก่อนแก้ schema
- ไม่ชัด → ถาม ห้ามเดา
## Commands
pnpm dev · pnpm test · pnpm lint
```

</div>
<div>

| Tool | ไฟล์ที่อ่าน |
|---|---|
| Claude Code | `CLAUDE.md` |
| Cursor | `.cursorrules` |
| Windsurf | `.windsurfrules` |
| Copilot | `.github/copilot-instructions.md` |
| Gemini | `GEMINI.md` |
| Codex / generic | `AGENTS.md` |

</div>
</div>

*เขียน source เดียว → mirror ทุกชื่อ · ถ้าเขียนแค่ `CLAUDE.md` เพื่อนที่ใช้ Cursor จะไม่ได้ context*

---

<span class="mono">// PART 2 · LAYER 2</span>

## CONTEXT.md — template + recipe

<div class="cols">
<div>

**Layer 2 = “codebase นี้ทำงานยังไง”**
รวมกฎสถาปัตยกรรม · naming · gotchas ของแต่ละ subsystem ไว้ที่เดียว

ของมีค่าสุดคือ **recipe เพิ่ม feature** — เขียนเป็น checklist ให้ AI ทำตามได้เป๊ะทุกครั้ง →

</div>
<div>

```text
# CONTEXT.md — Employee DB (ตัดมาส่วน recipe)
## กฎเวลาสร้าง feature ใหม่
1 แก้ prisma/schema.prisma + สร้าง migration ใหม่
2 อัปเดต lib/schema/employee.ts (Zod)
3 เพิ่ม app/api/employees/route.ts
    validate ก่อนแตะ Prisma
4 สร้าง /employees + /employees/new
    ใช้ schema เดียวกับ API
5 เพิ่ม API test + e2e ตาม AC
6 ห้ามแก้ migration ที่ apply แล้ว
```

</div>
</div>

**ทำซ้ำทุก subsystem → AI เรียนครั้งเดียว apply ได้ทุกที่ · เป้าหมาย: ผ่าน review รอบแรก**

---

<span class="mono">// PART 2 · LAYER 3</span>

## Traffic-light = handoff ที่อ่านออกทันที

```markdown
# CONTEXT_addEmployee.md — People Hub (Layer 3)
> สถานะ: Context + spec draft เสร็จ — รอเคลียร์ auth/startDate
> URL: /employees + /employees/new
> Workspace rules apply (ห้าม git commit เอง)
```

| Status | Item | Note |
|---|---|---|
| <span class="pill pill-done">DONE</span> | CONTEXT.md / CLAUDE.md | กฎโปรเจกต์พร้อมใช้ |
| <span class="pill pill-wip">กำลังทำ</span> | Requirement + AC | รอเคลียร์ auth/startDate |
| <span class="pill pill-todo">NOT STARTED</span> | Prisma + API + UI + tests | ลงมือหลัง plan ผ่าน review |

*เปิดมาพรุ่งนี้รู้ทันทีว่าค้างตรงไหน — ไม่ต้อง re-investigate*

---

<span class="mono">01 / CONTEXT · ตัวอย่างจริง</span>

## ไฟล์ rule ที่ commit เข้า repo

<div class="cols">
<div>

```markdown
# people-hub / Employee DB
Stack: Next.js · PostgreSQL + Prisma · Zod
Run: pnpm dev   Test: pnpm test
DB: pnpm prisma migrate dev

## Rules
- Validate input with Zod before Prisma
- Use Prisma only — no raw SQL
- Duplicate email → 409 (no stack trace)
- Do not edit applied migrations
- Reuse lib/schema/employee.ts in API + UI
```

</div>
<div>

**บอก stack + คำสั่ง** — ไม่เดา framework / วิธีรัน test
**ชี้ pattern ที่มีอยู่** — “ใช้ `lib/schema/employee.ts` ร่วมกัน” = ไม่แยก validation คนละชุด
**เขียนข้อห้ามไว้** — กันมันหลุดออกนอกแนวทางทีม

</div>
</div>

**commit ไฟล์เดียว → ทุก session + ทุกคนในทีม ได้บริบทเดียวกันทันที**

---

<span class="mono">01 / CONTEXT · TEMPLATE</span>

## Context file สำหรับ web + API + DB

*เริ่มโปรเจกต์ใหม่ — ใส่ข้อมูลพวกนี้ใน `CLAUDE.md` / `AGENTS.md` แล้ว commit ตั้งแต่วันแรก*

<div class="cols">
<div>

**Project & Stack** — ภาพรวม+โดเมน · FE·API·DB+ORM · runtime/pm/version
**Commands** — install·dev·build · test·lint·format · db: migrate·seed·reset
**Structure & Rules** — โครงโฟลเดอร์ · naming/error/import · “ทำตาม pattern ใน \<ไฟล์\>”

</div>
<div>

**Database** — schema + กฎ migration · ห้ามแก้ migration ที่ apply แล้ว · ใช้ ORM
**API & Security** — route + response/error · validation (zod) + status · auth + secret (ห้าม commit)
**Testing & Guards** — framework/coverage · ห้ามเพิ่ม dependency โดยไม่ถาม · ถามก่อนแก้ schema

</div>
</div>

---

<span class="mono">// GSTACK · 30 วินาที</span>

## ก่อนเข้าตัวอย่าง: gstack คือทีมช่วยงานที่เรียกด้วย command

*gstack = ชุด skill / command ที่ห่อ workflow ให้ Claude Code — ตอนนี้แค่รู้พอว่า command ที่เห็นใน case มาจากที่นี่*

<div class="cols">
<div class="card card-brand">

#### คำสั่งที่จะเห็นใน case
- `/review` ให้ AI ช่วยตรวจ diff / หาบั๊ก
- `/qa` ให้ AI ช่วยทดสอบ scenario
- `/ship` ช่วยสรุปงานก่อนส่ง PR

</div>
<div class="card card-green">

#### ตอนนี้ต้องจำแค่นี้
- skill = shortcut ของ workflow ที่ทำซ้ำบ่อย
- คนยังเป็นคนตัดสินใจและ review เสมอ
- ติดตั้งใน Claude Code: `install gstack`
- รายละเอียด command อื่น ๆ ค่อยดูท้าย workshop

</div>
</div>

> ให้มอง gstack เป็น “ทีมช่วยงาน” ที่เรียกเป็น command ได้ — ไม่ใช่ตัวแทน judgment ของเรา

---

<!-- _class: divider -->

<span class="secnum">03</span>

<span class="mono">SECTION</span>

## ตัวอย่างจริง

ระบบฐานข้อมูลพนักงาน — จาก context ไปสู่ spec · plan · review · จุดที่คนต้องคุมเอง

---

<span class="mono">// PART 3 · ตัวอย่างจริง</span>

## ตัวอย่าง: ระบบฐานข้อมูลพนักงาน

*1 feature: “เพิ่มพนักงานใหม่” — ไล่ตั้งแต่ init จนเริ่ม implement*

<p class="flow">1 Init › 2 Context › 3 Spec › 4 Plan › 5 Implement › 6 Review</p>

- **Init → Context** — ให้ AI ร่าง context file ตาม template เรา review
- **Spec → Plan** — เขียน user story + AC → สั่ง AI วางแผนก่อนเขียนโค้ด
- **Implement → Review** — ลงมือทีละ step · review ทุกก้อน · คุมงาน 30% สุดท้ายเอง

---

<span class="mono">// PART 3 · STEP 1 — INIT</span>

## ไม่ต้องเขียน context เอง — ให้ AI ร่าง

*ใช้ prompt ให้ AI ร่างโครง แล้วเรา review (AI scan/draft · human review)*

<div class="card card-brand">

**① เปิดด้วย (framing)**
“เริ่มโปรเจกต์ใหม่: ระบบฐานข้อมูลพนักงาน (web app + REST API + PostgreSQL) ยังไม่มีโค้ด ช่วยร่าง `CONTEXT.md` แล้ว mirror เป็น `CLAUDE.md`/`AGENTS.md` — อย่าเพิ่งเขียนโค้ด feature ถ้าไม่ชัดให้ถามก่อน ห้ามเดา”

</div>
<div class="card card-brand">

**② กำหนดโครงสร้างที่ต้องมี**
“ขอหัวข้อครบ: Hard rules · Project+โดเมน · Stack · Commands · Structure · Conventions · Database(no raw SQL) · API & Security · Testing — ใช้ตาราง+tree, ชื่อไฟล์อังกฤษ, กฎเจาะจง+ตรวจได้”

</div>

**→ AI ร่าง → review + แก้กฎให้ตรงทีม → commit + mirror ทุกชื่อไฟล์**

---

<span class="mono">// PART 3 · ผลลัพธ์ STEP 1</span>

## CONTEXT.md ที่ AI ร่างออกมา

*เรา review + แก้กฎให้ตรงทีม → commit เข้า repo*

```markdown
# CONTEXT.md — Employee DB
Stack: Next.js · API routes · PostgreSQL + Prisma · Zod
Run: pnpm dev   Test: pnpm test   DB: pnpm prisma migrate

## โครงสร้าง
app/employees/        หน้า list / create / edit
app/api/employees/    route handlers
lib/schema/           Zod schema (แชร์ client/server)
prisma/schema.prisma  ตาราง + migration

## กฎ (hard rules)
- ทุก input ผ่าน Zod ก่อนแตะ DB
- ใช้ Prisma เท่านั้น — ห้าม raw SQL
- อีเมลซ้ำ → ตอบ 409 (ไม่หลุด stack trace)
- ห้ามแก้ migration ที่ apply แล้ว · ถามก่อนแก้ schema

## recipe เพิ่ม field ใหม่
1 แก้ prisma schema → migrate
2 อัปเดต Zod schema
3 แก้ API + UI ที่ใช้ schema ร่วม
4 เพิ่ม test ครอบ field ใหม่
```

*__CLAUDE.md__ (Layer 1) = ไฟล์บาง ๆ ที่ชี้มาอ่าน `CONTEXT.md` นี้ + กฎเหล็ก แล้ว mirror เป็น `AGENTS.md` อัตโนมัติ*

---

<span class="mono">// PART 3 · ผลลัพธ์ STEP 1 (Layer 1)</span>

## CLAUDE.md — ไฟล์ entry ที่ชี้มา CONTEXT.md

*บาง ๆ · กฎเหล็ก + ชี้ว่าให้อ่านอะไรก่อน · mirror เป็น `AGENTS.md` อัตโนมัติ*

```markdown
# CLAUDE.md — Employee DB   <!-- mirror → AGENTS.md · อย่าแก้มือ -->
## อ่านก่อนเริ่มงาน
1. @CONTEXT.md            architecture · กฎ · recipe (ของจริงอยู่นี่)
2. @CONTEXT_<feature>.md   งานที่กำลังทำ (ถ้ามี)
## Hard rules (ห้ามพลาด)
- ห้าม git commit / push เอง — ให้คนกด
- ห้ามแก้ migration ที่ apply แล้ว · ถามก่อนแก้ schema
- ห้ามเพิ่ม dependency ใหม่ · ไม่ชัด → ถามก่อน ห้ามเดา
## Commands
dev: pnpm dev   ·   test: pnpm test   ·   lint: pnpm lint
## Skills
/review ก่อนเปิด PR   ·   /qa เทสต์ browser จริง
```

---

<span class="mono">// PART 3 · SKILL 02 — SPEC</span>

## ใน case นี้: สั่งแบบ spec ไม่ใช่ vibe

*ก่อนให้ AI เขียน เราเปลี่ยนคำสั่งกว้าง ๆ ให้เป็น input/output/edge case ที่ตรวจได้*

<div class="cols">
<div class="card" style="border-color:var(--brand)">

#### ✗ Vibe คลุมเครือ
“ทำระบบเพิ่มพนักงานหน่อย”
*→ AI ต้องเดา field, auth, validation, response, edge case เองเกือบหมด*

</div>
<div class="card card-green">

#### ✓ Spec ชัด
HR เพิ่มพนักงานใหม่ด้วย name/email/department/position/startDate/status, email unique → 409, field ว่าง → error ใต้ช่อง, สำเร็จ → กลับ list เห็นทันที, มี test happy + invalid + duplicate

</div>
</div>

> **นิสัยที่ใช้ใน step นี้**
> • **วางแผนก่อนเขียน** — “เสนอแนวทางก่อน อย่าเพิ่งเขียนโค้ด” เพื่อจับ ambiguity ตั้งแต่ยังถูก
> • **แตกเป็นก้าวเล็ก** — DB · validation · API · UI · tests แยก review ได้ทีละก้อน

---

<span class="mono">// PART 3 · REQUIREMENT → PLAN</span>

## เขียน spec → ให้ AI วางแผนก่อน

<div class="cols">
<div class="card">

**Requirement** — เพิ่มพนักงานใหม่ (HR ใช้)
*ฟิลด์: ชื่อ-สกุล · email(unique) · แผนก · ตำแหน่ง · วันเริ่มงาน · สถานะ*

**AC:**
- กรอกครบ → บันทึกได้
- email ซ้ำ → error ไม่บันทึก
- สำเร็จ → กลับ list เห็นทันที
- ฟิลด์ว่าง → เตือนใต้ช่อง
- <span class="amber">วันเริ่มงานอนาคต? ← ยังไม่ชัด</span>

</div>
<div class="card card-brand">

**Plan ที่ AI ตอบกลับ**
<span class="amber">ถามก่อน:</span> กติกาวันเริ่มงาน · แผนก/ตำแหน่ง free-text หรือ dropdown · ใครมีสิทธิ์ (auth)

**แผน (commit ทีละก้อน):**
1. Prisma model + migration
2. Zod schema (แชร์ client/server)
3. API POST + GET
4. UI ฟอร์ม + list
5. Tests (happy / ซ้ำ / invalid + e2e)

</div>
</div>

---

<span class="mono">// PART 3 · ผลลัพธ์ PLAN</span>

## แผนเต็มที่ AI เสนอกลับมา

*สั่ง “วางแผนก่อน อย่าเพิ่งเขียนโค้ด” → ได้แผนที่ review ได้ก่อนลงมือ*

```markdown
# PLAN — เพิ่มพนักงานใหม่

## ถามก่อน (ต้องเคลียร์)
- วันเริ่มงานเป็นอนาคต: อนุญาตไหม?
- แผนก/ตำแหน่ง: free-text หรือ dropdown?
- ใครมีสิทธิ์เพิ่มพนักงาน (auth)?

## ขั้นตอน (commit ทีละก้อน)
1 Prisma model Employee + migration
   └ name · email@unique · deptId · position · startDate · status
2 Zod schema employeeCreate (แชร์ client/server)
3 API POST + GET /api/employees · email ซ้ำ → 409
4 UI ฟอร์ม (shadcn + zodResolver) + หน้า list
5 Tests: happy · email ซ้ำ · invalid · e2e

## เสร็จเมื่อ (Definition of Done)
test ผ่าน + เพิ่มพนักงานผ่าน UI ได้จริง
```

> **แผนผ่าน review แล้ว → สั่งให้ลงมือ:** “อ่าน `@CONTEXT.md` + แผนนี้ แล้วลงมือ **step 1 (Prisma model + migration)** ทีละก้อน · ทำตาม recipe ใน CONTEXT.md · หยุดให้ review ก่อนไป step ถัดไป · ห้าม commit เอง”

---

<span class="mono">// PART 3 · IMPLEMENT</span>

## ลงมือทีละ step — review ทุกก้อน

| # | step | review focus |
|---|---|---|
| 1 | **DB** · Prisma model + migration | field/unique · ดู migration ก่อน apply |
| 2 | **Validation** · Zod schema แชร์ client/server | ครบ field · error message ไทย |
| 3 | **API** · POST/GET · อีเมลซ้ำ→409 | status code · ไม่หลุด stack trace |
| 4 | **UI** · shadcn + zodResolver (`/ux-ui-pro-max`) | ใช้ schema เดียวกับ API · redirect |
| 5 | **Tests** · api + e2e ตาม AC | test สะท้อน AC จริง · รันผ่าน |

> ปิดงาน: `/review` (หาบั๊ก) › `/qa` (เทสต์ browser จริง) › `/ship` (เปิด PR) — ของ gstack

---

<span class="mono">// PART 3 · SKILL 03 — REVIEW</span>

## ระหว่าง implement: อยู่ใน loop เสมอ

*โค้ดที่ merge เข้าไป คุณเป็นเจ้าของ — “AI เขียน” ไม่ใช่ข้ออ้างใน PR*

- ✓ **อ่าน diff ทุกก้อนตามแผน** — DB · validation · API · UI · tests ต้องเข้าใจว่าทำไมเปลี่ยน
- ✓ **ดู migration ก่อน apply** — field/unique/index ถูกไหม และไม่แก้ migration ที่ apply แล้ว
- <span class="amber">▲</span> **ระวัง failure mode คลาสสิก** — API/แพ็กเกจที่ไม่มีจริง · logic ดูดีแต่ผิด · ช่องโหว่ security · secret หลุด
- ✓ **verify อย่าเชื่อ** — รันจริง รัน test เช็ค duplicate email / invalid field / permission
- <span class="amber">▲</span> **architecture อยู่ในหัวคุณ** — AI มองแค่ local ต้องสั่ง reuse schema/helper/pattern เดิม

---

<span class="mono">// PART 3 · SKILL 04 — 70% PROBLEM</span>

## ท้าย case: รู้ว่าเมื่อไหร่ต้องคุมเอง

<div class="bar">
<div style="flex:0 0 70%;background:var(--brand)">70% · AI พาไปถึง</div>
<div style="flex:0 0 30%;background:var(--amber)">30% · งานของคุณ</div>
</div>

*ระบบพนักงานดูเหมือน CRUD ธรรมดา แต่ 30% สุดท้ายคือกฎข้อมูลส่วนบุคคล สิทธิ์ และ schema ที่พลาดแล้วเจ็บจริง*

<div class="cols">
<div class="card card-brand">

**ปล่อยให้ AI เต็มที่**
scaffold CRUD · ฟอร์ม · validation message · test boilerplate · refactor ตาม pattern · เพิ่ม state/loading/error

</div>
<div class="card card-amber">

**ต้องลงมือคุมเอง**
auth/role ของ HR · PDPA/ข้อมูลเงินเดือน · schema/migration · error semantics · approve ก่อน release

</div>
</div>

<p class="green" style="text-align:center">AI ขยาย judgment ที่คุณมีอยู่แล้ว — มี = เร็วขึ้น / ไม่มี = พังเร็วขึ้น</p>

---

<!-- _class: divider -->

<span class="secnum">04</span>

<span class="mono">SECTION</span>

## Vibe QA — สั่ง AI เขียน test

เขียน test ให้ครอบโจทย์ ด้วยการ prompt ที่ดี + คิดแบบ QA

---

<span class="mono">// VIBE QA · แนวคิด</span>

## QA เปลี่ยนจาก “เขียน test” → “กำกับ AI เขียน test”

*งานหลักของ QA ไม่ใช่พิมพ์ test เอง — แต่คือรู้ว่า “ต้องเทสอะไร” แล้วสั่ง AI + ตรวจว่ามันครอบจริง*

<div class="cols">
<div class="card card-green">

#### ปล่อยให้ AI ทำ
- ร่าง test case จาก AC + spec
- เขียน boilerplate · API · scenario/e2e
- รันแล้ววนแก้จนผ่าน

</div>
<div class="card card-amber">

#### QA ต้องคุมเอง
- ชี้ว่า “อะไรต้องเทส” — edge case · scenario · ทุก AC
- ตรวจว่า test **ประกบ AC จริง** ไม่ใช่ test ที่ไล่ตามโค้ด (pass เสมอ)
- จับ AI ที่ “แก้โค้ดให้ test ผ่าน” หรือ mock จนไม่ได้เทสอะไร

</div>
</div>

> คุณค่าของ QA ยุค vibe = **judgment ว่าครอบพอไหม** ไม่ใช่ความเร็วในการพิมพ์ test

---

<span class="mono">// VIBE QA · วงจร</span>

## วงจร Vibe QA — สั่ง · ตรวจ · วน

*ปล่อย AI ทำหนัก แต่คนคุมที่ “ขั้นตรวจ” (3) — ตัดสินว่าครอบ AC พอหรือยัง*

<p class="flow">1 AC/Plan › 2 AI ร่าง cases › 3 QA review › 4 AI เขียน+รัน (/qa) › 5 ครอบ AC ✓</p>

> ถ้า step 3 เจอ AC ที่ยังไม่มี test → **วนกลับ step 2** · จุดที่คนต้องอยู่คือ “ตัดสินว่าครอบพอ” ไม่ใช่พิมพ์ test เอง

---

<span class="mono">// VIBE QA · PROMPT</span>

## prompt เขียน test (ประกบ plan + ตามของเดิม)

<div class="cols">
<div>

```text
# prompt เขียน test
เขียน test ให้ feature "เพิ่มพนักงาน"
อ้างอิง AC ใน @CONTEXT.md
ทำตาม pattern เดิมใน @tests/
 (โครงสร้าง · การตั้งชื่อ · helper เหมือนเดิม)

ครอบ 2 ระดับ:
- API: POST /employees → 201/409/400/403
- Scenario e2e: กรอกฟอร์ม → เห็นใน list → แก้ได้

ทุก AC ต้องมี test ประกบ + เคสพัง (ว่าง·ซ้ำ·สิทธิ์)
ใช้ framework เดิมในโปรเจกต์
ห้ามแก้ business logic เพื่อให้ test ผ่าน
```

</div>
<div>

**อ้างอิงของเดิมเสมอ** — ชี้ `@tests/` ให้ AI ลอก pattern/helper เดิม อย่าตั้ง convention ใหม่
**ครอบ 2 ระดับ** — API + **scenario (e2e)** ตาม flow ผู้ใช้
**ประกบ AC** — ขอ list คู่ AC ↔ test ก่อน → review → ค่อยเขียน · ปิดด้วย `/qa`

</div>
</div>

---

<span class="mono">// VIBE QA · CONTEXT FILE</span>

## QA ควร prompt อะไรใส่ context file

*เขียนกฎ test ลง `CONTEXT.md` ครั้งเดียว → ทุก session AI เขียน test สไตล์เดียวกัน*

<div class="cols">
<div>

```text
# prompt: เพิ่มส่วน Testing ใน CONTEXT.md
อ่าน @tests/ แล้วสรุปเป็นกฎลง CONTEXT.md:
- framework + ที่อยู่ test + วิธีรัน
- naming + โครงสร้าง (table-driven?)
- ระดับที่ต้องมี: API + scenario(e2e)
- กฎ: ทุก AC ต้องมี test ประกบ
- helper/fixture ที่ reuse ได้
```

</div>
<div>

```text
# ผลลัพธ์: ส่วน ## Testing ใน CONTEXT.md
- framework: vitest · อยู่ใน tests/
- รัน: pnpm test · e2e: pnpm test:e2e
- ทุก endpoint = table-driven + scenario
- ทุก AC ต้องมี test ประกบ (AC ↔ test)
- ใช้ helper ใน tests/_helpers.ts
- ห้ามแก้ logic เพื่อให้ test ผ่าน
```

</div>
</div>

> QA ที่เก่งไม่ได้แค่เขียน test เก่ง — แต่ทำให้ “กฎการเทส” อยู่ใน context ที่ AI + ทั้งทีมใช้ร่วมกัน

---

<!-- _class: divider -->

<span class="secnum">05</span>

<span class="mono">SECTION</span>

## Multi-agent — ทำงานเป็นทีม AI

ไม่ใช่แค่งาน dev — ใช้ AI หลายตัวแบ่งบทบาท ช่วยงาน PO / product ได้

---

<span class="mono">// PO + MULTI-AGENT</span>

## ไม่ใช่แค่ dev — PO ก็ใช้ AI เป็น “ทีม” ได้

*แทนที่จะถาม AI ตัวเดียวทำงาน PO ทั้งหมด → แบ่งเป็นทีม agent แต่ละตัวมีบทบาท แล้วคุณเป็นคนเคาะ*

<div class="cols">
<div>

- **Research** — สรุปปัญหา · ตลาด · คู่แข่ง · feedback
- **Story writer** — แตก epic → user story + AC
- **Critic / Risk** — หา edge case · ความเสี่ยง

</div>
<div>

- **Prioritization** — จัดลำดับ RICE / MoSCoW
- **Orchestrator + คุณ (PO)** — รวมผล · ตัดสินใจ · เคาะสุดท้าย

</div>
</div>

> **Pattern:** orchestrator → agents ทำงานขนาน → critic ค้าน/ตรวจ → **human อนุมัติ**

---

<span class="mono">// PO + MULTI-AGENT · WORKFLOW</span>

## จาก idea → backlog ที่พร้อมใช้

<p class="flow">1 Research › 2 Story writer › 3 Critic/Risk › 4 Prioritize › 5 คุณ (PO)</p>

<div class="card">

**ผูกกับทักษะใน workshop**
**Context:** ทุก agent อ่าน product context เดียวกัน ·
**Spec:** ให้ agent ถาม ambiguity ก่อนร่าง ·
**Review:** critic ค้านก่อน คน PO เคาะทีหลัง

</div>

> คน PO ไม่ได้หายไป — เปลี่ยนจาก “เขียนเองทุกอย่าง” เป็น **“คุมทีม AI + ตัดสินใจ”**

---

<span class="mono">// MULTI-AGENT · ไฟล์บริบทร่วม</span>

## ตัวอย่าง PRODUCT_CONTEXT.md

*ไฟล์เดียวที่ agent ทุกตัวอ่านร่วมกัน — เข้าใจ product ตรงกันก่อนเริ่ม*

```markdown
# PRODUCT_CONTEXT.md — People Hub (ระบบ HR)

## Vision
ให้ HR จัดการข้อมูลพนักงานครบใน 1 ที่ ลดงานเอกสารซ้ำ

## Personas
- HR Officer — เพิ่ม/แก้พนักงาน · ออกรายงาน
- Manager    — ดูทีมตัวเอง · อนุมัติวันลา
- Employee   — ดู/แก้ข้อมูลตัวเอง

## Constraints
- PDPA: ข้อมูลส่วนบุคคลห้ามหลุด / ห้าม log
- UI ภาษาไทย · เงินเดือนเห็นเฉพาะ HR

## Success metric
- เพิ่มพนักงานใหม่ < 2 นาที · ลด ticket แก้ข้อมูล 50%

## Out of scope (ตอนนี้)
- payroll คำนวณภาษี · mobile app
```

---

<span class="mono">// MULTI-AGENT · PROMPT</span>

## prompt ที่สั่งทีม agent

<div class="cols">
<div>

```text
# orchestration prompt
ทำตัวเป็นทีม PO 4 บทบาท ทำงานต่อกัน
อ่าน PRODUCT_CONTEXT.md ก่อนเสมอ:

1) RESEARCHER สรุปปัญหา + คู่แข่ง 3 ราย
2) PM เขียน epic → user story + AC
3) RISK หา edge case + คำถามที่ยังไม่ตอบ
4) PRIORITIZER จัดลำดับด้วย RICE

กฎ: ข้อมูลไม่พอให้ “ถามก่อน” ห้ามเดา
จบแล้วสรุปเป็นตารางให้ PO เคาะ
```

</div>
<div>

**3 อย่างที่ทำให้ prompt เวิร์ก**
1. ชี้ให้อ่าน context file ก่อน
2. บังคับให้ “ถาม” เมื่อไม่ชัด (จับ ambiguity)
3. ขอ output รูปแบบที่ตรวจง่าย (ตาราง)

**เริ่มเล็ก** — 1 prompt หลายบทบาทก่อน → ค่อยแยกเป็นหลาย agent จริงเมื่อจำเป็น

</div>
</div>

---

<span class="mono">// MULTI-AGENT · ตัวอย่างหน้าจอ</span>

## หน้าจอตอน agent คุยกัน

> **RESEARCHER:** คู่แข่งหลัก 3 ราย — จุดต่างของเราคือใช้ง่าย + ภาษาไทยเต็มระบบ

> **PM:** ร่าง 5 user stories + AC แล้ว เช่น “HR เพิ่มพนักงาน → ถ้า email ซ้ำต้องเตือน”

> **RISK:** ขอถามก่อน 2 ข้อ — วันเริ่มงานเป็นอนาคตได้ไหม? · ใครเห็นเงินเดือนบ้าง?

> <span class="green">**คุณ (PO):**</span> วันเริ่มงานอนาคตได้ · เงินเดือนเห็นเฉพาะ HR → ไปต่อได้

> **PRIORITIZER:** จัดลำดับ RICE: 1) เพิ่มพนักงาน 2) ค้นหา/กรอง 3) ออกรายงาน

*เห็น “ทาง” ของแต่ละ agent → ตรวจได้ว่าใครคิดอะไร และเข้าไปแก้จุดที่ผิดได้ตรงจุด*

---

<span class="mono">// MULTI-AGENT · เครื่องมือ</span>

## เครื่องมือที่ช่วยได้

<div class="cols">
<div class="card card-brand">

#### product context file
`PRODUCT_CONTEXT.md` — vision · persona · constraint · glossary ให้ทุก agent อ่านร่วม แล้ว commit ไว้ใน repo

</div>
<div class="card card-brand">

#### gstack = multi-agent สำเร็จรูป
`/office-hours` เจาะไอเดีย · `/plan-ceo-review` กลยุทธ์/scope · `/autoplan` review หลาย role

</div>
</div>

> ไม่ต้องสร้างเองทั้งหมด — gstack มีทีม agent ให้ใช้เลย (ดูสไลด์เครื่องมือแนะนำท้าย ๆ)

---

<!-- _class: divider -->

<span class="secnum">06</span>

<span class="mono">SECTION · สำหรับหัวหน้าทีม</span>

## นำทีม vibe coding ยังไงให้รอด

เครื่องมือแรงขึ้น = ทีมไปได้เร็วขึ้น หรือพังเร็วขึ้น — อยู่ที่คนนำวางระบบ

---

<span class="mono">// TEAM LEAD · ข้อควรปฏิบัติ</span>

## 7 ข้อที่หัวหน้าทีมต้องวางให้ทีม

<div class="cols">
<div>

- **ตั้งมาตรฐานกลาง** — context file ระดับทีม commit ให้ทุกคน + AI ใช้ baseline เดียว
- **review เป็นกติกา** — โค้ด AI ผ่าน review เท่า PR คน · ห้าม merge สิ่งที่ไม่มีใครเข้าใจ
- **แบ่งงานตาม 70%** — ปล่อย AI งานซ้ำ · ให้คนคุม security · architecture · hot path
- **สั่งให้ reuse ไม่เขียนซ้ำ** — ให้ AI หา component/util ที่มีอยู่มาใช้ก่อน · สั่ง refactor รวมโค้ดซ้ำ

</div>
<div>

- **Definition of Done** — = รันจริง + test ผ่าน ไม่ใช่แค่ “compile ได้”
- **วาง guardrails** — permission · แยก branch · ห้าม agent แตะ secret / prod
- **วัดที่ outcome** — feature ที่ส่งได้ + คุณภาพ ไม่ใช่จำนวนบรรทัด/วัน

</div>
</div>

> **ระวัง:** junior ที่พึ่ง AI จนไม่เข้าใจโค้ด = ทีมโตช้า — ให้เข้าใจสิ่งที่ AI เขียน + แชร์ prompt/recipe ที่เวิร์กให้ทั้งทีม

---

<!-- _class: divider -->

<span class="secnum">07</span>

<span class="mono">SECTION</span>

## นำไปใช้ + ปิดท้าย

งานที่เอาไปใช้ได้เลย · Git hygiene · เครื่องมือแนะนำ · ติดตั้ง

---

<span class="mono">// USE CASES · ตัวอย่างงานจริง</span>

## งานที่เอาไปใช้ได้เลย

<div class="cols">
<div>

- **เริ่มงานใน codebase ที่ไม่คุ้น**
  *“อธิบาย flow การ auth ไล่จากไฟล์ไหนบ้าง”*
- **เขียน test ให้โค้ดที่ยังไม่มี**
  *“เขียน table-driven test ครอบ edge case”*
- **Refactor กว้าง ๆ**
  *“แยก logic นี้เป็น service ตาม pattern ใน X”*

</div>
<div>

- **Debug จาก error / log**
  *“นี่ stack trace — หาสาเหตุ + เสนอ fix”*
- **Boilerplate / งานซ้ำ ๆ**
  *“สร้าง CRUD endpoint ตามแบบที่มีอยู่”*
- **แปลง / พอร์ตโค้ด**
  *“แปลงสคริปต์ bash นี้เป็น Go”*

</div>
</div>

---

<span class="mono">SAFETY NET</span>

## Git hygiene = กล้าเร็วได้

*ตาข่ายนิรภัยที่ทำให้กล้าปล่อยให้ AI ลองได้ โดยย้อนกลับได้เสมอ*

1. **commit เล็ก · commit บ่อย** — rollback ง่ายเวลา AI หลุดโลก ย้อนแค่ก้าวเดียว ไม่ใช่ทั้งวัน
2. **git diff คือพื้นที่ review** — ทุก change ผ่านสายตาคุณก่อน merge เสมอ
3. **อย่าปล่อย change ค้างกองพะเนิน** — ของที่ยังไม่ commit เยอะ ๆ = ย้อนกลับไม่สะอาด แยกของดี/เสียไม่ออก

---

<span class="mono">// SKILLS · ใช้งาน</span>

## skill คืออะไร — แล้วใช้ยังไง

*skill = workflow สำเร็จรูปที่เรียกด้วย `/command` — แทนการพิมพ์ prompt ยาว ๆ ซ้ำ ๆ*

<div class="cols">
<div class="card card-green">

#### ใช้ง่าย ๆ
- พิมพ์ `/<ชื่อ>` เช่น `/review` · `/qa` · `/ship`
- skill ทำงานหลาย step ให้เอง — ไม่ต้องพิมพ์ prompt ยาว
- ส่ง argument เพิ่มได้

</div>
<div class="card card-brand">

#### ทำไมดีกว่า prompt สด
- มาตรฐานเดียวทั้งทีม — ใครเรียกก็ได้ผลเหมือนกัน
- deterministic + version-controlled
- best practice ฝังอยู่ในตัว skill

</div>
</div>

> ที่เห็นใน workshop นี้: `/review` หาบั๊ก · `/qa` เทส · `/ship` เตรียมส่งงาน · `/office-hours` เจาะไอเดีย

---

<span class="mono">// SKILLS · บริหาร</span>

## บริหาร skill ให้ทั้งทีมได้ใช้

<div class="cols">
<div class="card">

#### ติดตั้ง & ขอบเขต
- **project skill** (ใน repo) vs **global** (เครื่องตัวเอง)
- commit skill เข้า repo → ทั้งทีม + CI ใช้เหมือนกัน
- เปิด/ปิดเฉพาะที่ต้องใช้ได้

</div>
<div class="card">

#### เขียน skill เอง
- ห่อ workflow ที่ทำซ้ำบ่อยเป็น skill (เช่น “สร้าง CRUD ตาม pattern”)
- ฝัง context/กฎทีมไว้ในตัว skill
- แชร์ผ่าน repo เหมือน context file

</div>
</div>

> skill = context engineering ระดับ “ขั้นตอนการทำงาน” — เขียนครั้งเดียว ทีมใช้ซ้ำได้ตลอด

---

<span class="mono">// RECOMMENDED SKILLS · ของทีม</span>

## Skill ที่แนะนำให้ติดไว้

<div class="cols">
<div class="card card-brand">

### `/gstack`
*ทีมวิศวกรเสมือน · ฟรี MIT*

ชุด skill โอเพนซอร์สของ Garry Tan (CEO, YC) เปลี่ยน Claude Code เป็นทีม 23+ บทบาท

- สปรินต์: Think → Plan → Build → Review → Test → Ship
- เด่น: `/office-hours /autoplan /review /qa /ship /cso`

**เหมาะกับ** อยากมี process + auto review/QA ทุก PR

</div>
<div class="card card-brand">

### `/ux-ui-pro-max`
*design intelligence · ฟรี MIT*

ฐานข้อมูลดีไซน์ให้ AI — 50+ styles · 161 palettes · 57 font pairings · 99 UX rules

- ขอ UI ปุ๊บ สร้าง design system + แนะนำ style/สี/ฟอนต์
- ครอบ React / Next / Vue / Svelte / SwiftUI / Flutter

**เหมาะกับ** ทำ UI สวยระดับโปร เลี่ยง “AI slop”

</div>
</div>

---

<span class="mono">// INSTALL · สแกนเพื่อเริ่ม</span>

## ติดตั้งแล้วเริ่มใช้ได้เลย

<div class="cols">
<div class="card" style="text-align:center">

### `/gstack`
![w:170](qr_gstack.png)
[github.com/garrytan/gstack](https://github.com/garrytan/gstack)
`install gstack`
*รันใน Claude Code หลังวางลิงก์ repo / เปิดหน้า repo*
<span class="muted">ต้องมี Claude Code + Bun · ฟรี MIT</span>

</div>
<div class="card" style="text-align:center">

### `/ux-ui-pro-max`
![w:170](qr_uiux.png)
[ui-ux-pro-max-skill.nextlevelbuilder.io](https://ui-ux-pro-max-skill.nextlevelbuilder.io/)
`npm i -g uipro-cli → uipro init --ai claude`
<span class="muted">Claude Code / Cursor / Windsurf · ฟรี MIT</span>

</div>
</div>

---

<!-- _class: divider -->

<span class="secnum">08</span>

SECTION · ลงมือทำ

# Workshop — สร้างของจริง

โปรเจกต์จริง: **CPMatch Care** — แอพดูแลพนักงานในองค์กร · วาง context + plan ทีละ feature ด้วย 4 ทักษะ

---

<span class="mono">// WORKSHOP · BRD ย่อ</span>

## โจทย์จริง: CPMatch Care — แอพดูแลพนักงาน

*แอพภายในองค์กร · ผู้ใช้: พนักงาน / หัวหน้า / admin · workshop นี้วาง context + plan ทีละ feature (ยังไม่ลงโค้ด)*

<div class="cols">
<div class="card brand">

### Core HR
- ทะเบียนพนักงานทั้งองค์กร
- ขาด · ลา · มาสาย
- จัดคนเข้า project (admin)

</div>
<div class="card">

### Engagement + Wellbeing
- ระบบแต้มเมื่อทำกิจกรรมสำเร็จ
- กล่องระบายความรู้สึก **ไม่ระบุตัวตน**
- AI สรุปให้หัวหน้าอ่าน

</div>
<div class="card green">

### Platform
- RBAC หลายระดับ · ตั้งสิทธิ์อิสระ
- หน้า admin จัดการระบบ
- Web + Mobile + API แยก service

</div>
</div>

`Web · Next.js + Prisma + Tailwind` · `App · Flutter` · `API · Go + GORM (clean arch)` · `DB · Postgres + Docker`

> **กติกา:** plan ก่อนทุก feature · สรุป tech stack + architecture ก่อนลงมือ · test coverage > 80% (API unit + Playwright) · โทนสีตาม design CPMatch Care

---

<span class="mono">// WORKSHOP · เตรียมเครื่อง (5 นาที)</span>

## ก่อนเริ่ม: เช็กให้พร้อม

*ทำให้ครบก่อน แล้วทั้ง session จะลื่น ไม่ติดเรื่อง setup กลางทาง*

<div class="cols">

- **1** Claude Code เปิดได้ + login แล้ว
- **2** git — repo หลัก + submodule `/api` `/web` `/app`
- **3** โฟลเดอร์ `/plans` สำหรับ plan ทุก feature

- **4** skills: `/gstack` · `/ux-ui-pro-max` · `/impeccable` — ตรวจ + install ก่อนเริ่ม
- **5** editor เปิด root ไว้ (เห็น context.md / claude.md)
- **6** ไฟล์ design โทนสี CPMatch Care ไว้อ้างอิง

</div>

> โครงสร้าง: root เก็บ `context.md` + `claude.md` · service แยก submodule `/api` `/web` `/app` · plan เป็น `/plans/001-<feature>.md` (ref context.md เสมอ)

---

<span class="mono">// WORKSHOP · pipeline — วันนี้หยุดที่ Plan</span>

## ตั้งระบบให้ดี ก่อนลงโค้ด

`1 Context (Layer 1-3) → 2 Roles (role.md) → 3 Plan/feature [หยุดที่นี่] → 4 Implement → 5 Review+QA (cov>80%) → 6 Ship`

- **1 Context** — ให้ AI ร่าง `context.md` (architecture) + `claude.md`/`agent.md` (Layer 1, ห้าม commit เอง) ตามโครง Layer 1-3
- **2 Roles** — `role.md` ทีมที่ปรึกษา: uxui 1 · dev lead 1 · po 2 · end-user 1 — เรียกใช้ตอนคิด feature ใหม่
- **3 Plan/feature** — เลือก feature → สรุป tech stack + architecture → `/plans/001-*.md` (สถานะ todo→done) *ก่อน*ลงโค้ด

> prompt บอกชัด: “ยังไม่ต้อง implement ให้แพลนให้เสร็จและทำทีละ feature” — workshop วันนี้จบที่ **plan ที่ review ได้**

---

<span class="mono">// WORKSHOP · prompt พร้อมใช้ — ก๊อปแล้วปรับ</span>

## prompt ประจำแต่ละก้าว

**① Context — kickoff (ตัวเต็มในคลัง Resources)**
“สร้างโปรเจกต์ใหม่ **CPMatch Care**: แอพพนักงานในองค์กร (Web Next.js · App Flutter · API Go · DB Postgres) — ภาพรวมฟีเจอร์ + โครง context Layer 1-3 + skills ที่ต้องมี · **ยังไม่ต้อง implement** เขียน `context.md` ให้เสร็จก่อน ไม่ชัดให้ถาม ห้ามเดา” → prompt เต็มในคลัง Resources

**② Roles — ทีมที่ปรึกษา**
“สร้าง `role.md` จำลอง persona: uxui 1 · dev lead 1 · po 2 · end-user 1 — ทุกครั้งที่ขึ้น plan feature ใหม่ ให้ถามก่อนว่าจะเรียกทีมนี้ปรึกษาไหม”

**③ Plan/feature — สรุป stack + arch ก่อน**
“เลือก feature ‘ขาด/ลา/มาสาย’: สรุป tech stack + architecture design ของแต่ละ service ให้ครบก่อน แล้วเขียน `/plans/001-*.md` (ref context.md · มีสถานะ todo→done) — ยังไม่ลงโค้ด”

**④ Implement → ปิดงาน (ทำต่อทีละ feature)**
“ลงมือตาม plan ทีละก้าว หยุดให้ review ก่อนไปต่อ · test cov > 80% (API unit + Playwright)” · จบ feature: `/review` → `/qa` → `/ship`

---

<span class="mono">// WORKSHOP · เกณฑ์เสร็จ</span>

## “เสร็จ” ของ workshop วันนี้

<div class="cols">
<div class="card green">

### Definition of Done
- ✓ `context.md` (Layer 2) + `claude.md`/`agent.md` (Layer 1) ครบ
- ✓ `role.md` ทีมที่ปรึกษาพร้อมใช้
- ✓ ≥ 1 plan ใน `/plans/001-*.md` (มีสถานะ · ref context)
- ✓ สรุป tech stack + architecture ครบทุก service
- ✓ ระบุกฎ test (cov > 80%) ใน context แล้ว

</div>
<div class="card amber">

### กับดักที่เจอบ่อย
- ▲ รีบ implement ก่อนวาง context → กลับมาแก้ยับ
- ▲ สั่ง mega-prompt ทีเดียว → ทำทีละ feature
- ▲ ปล่อย AI commit เอง → กฎ Layer 1: ห้าม commit ถ้าไม่สั่ง
- ▲ plan ไม่มีสถานะ → ใส่ todo→done ทุก feature

</div>
</div>

> มี context + plan ที่ review แล้ว → ลง implement ทีละ feature ด้วย pipeline เดิม (Implement → Review → /qa → /ship) ได้เลย

---

<span class="mono">// RECAP · สรุป + กับดักที่เลี่ยง</span>

## เปลี่ยน vibe → ใช้งานจริง

| ทักษะ | ✓ ทำ | ✗ เลี่ยง |
|---|---|---|
| **Context engineering** | ป้อนบริบทที่ใช่ + commit rule file | ไม่มี rule file ปล่อย AI เดาเอง |
| **Spec ไม่ใช่ vibe** | สั่งชัด + วางแผนก่อน + ก้าวเล็ก | mega-prompt สั่งทีเดียวใหญ่ |
| **วินัยการ review** | อ่าน diff ทุกบรรทัด เป็นเจ้าของโค้ด | รับโค้ดที่ไม่เข้าใจ · เชื่อ “รันผ่าน=ถูก” |
| **70% problem** | ปล่อย AI ที่ง่าย คุมเองที่สำคัญ | ปล่อย agent แตะ secret / คำสั่งอันตราย |

> **+ Git hygiene** เป็นตาข่ายนิรภัยตลอดทั้ง 4 ทักษะ

---

<!-- _class: divider -->
<!-- _paginate: false -->

# ขอบคุณครับ

### Thank you — ลองเอา vibe coding ไปใช้กับงานจริงดูนะครับ

<span class="mono">คำถาม / คุยต่อได้เลย · vibe coding workshop · CPMatch</span>
