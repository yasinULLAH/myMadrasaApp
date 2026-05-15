# 🕌 Madrasa Management System | مدرسہ مینجمنٹ سسٹم
**Developed by:** Yasin Ullah – Bannu Software Solutions  
**Website:** [www.yasinbss.com](https://www.yasinbss.com) | **WhatsApp:** `03361593533`  
**Demo Credentials:** `admin / admin@123` | `teacher / Teacher@123`

---

## 📖 Overview | تعارف
**English:**  
A complete, all-in-one digital management platform designed specifically for Madrasas, Islamic schools, and modern educational institutes. It integrates academics, finance, HR, hostel, library, Hifz tracking, and administrative controls into a single secure interface. The system is built for scalability, offline/online flexibility, and client-friendly reporting.

**اردو:**  
یہ ایک مکمل ڈیجیٹل انتظامی پلیٹ فارم ہے جو خاص طور پر مدارس، اسلامی اسکولوں اور جدید تعلیمی اداروں کے لیے ڈیزائن کیا گیا ہے۔ یہ تعلیم، فنانشل، ایچ آر، ہاسٹل، لائبریری، حفظ ٹریکنگ اور انتظامی کنٹرول کو ایک محفوظ انٹرفیس میں مربوط کرتا ہے۔ یہ سسٹم اسکیل ایبلٹی، آف لائن/آن لائن لچک، اور کلائنٹ فرینڈلی رپورٹنگ کے لیے بنایا گیا ہے۔

---

## 👥 User Roles & Access | صارفین کے کردار اور رسائی
| Role / کردار | Permissions / اجازتیں |
|---|---|
| **Admin / ایڈمن** | Full access to all modules, settings, backups, user management, financial overrides, and audit logs. |
| **Teacher / استاد** | Attendance, Hifz tracking, exam entry, timetable view, duty roster, limited student records. |
| **Accountant / اکاؤنٹنٹ** | Fee collection, expenses, salaries, donations, fines, financial reports, receipt generation. |
| **Librarian / لائبریرین** | Book issuing/returns, overdue tracking, library reports. |
| **Teacher Record / منسلک استاد** | Read-only or restricted academic entry, Hifz progress, attendance marking. |

**اردو نوٹ:** ہر صارف کا کردار سسٹم کی سیکیورٹی اور ڈیٹا کی درستگی کو یقینی بناتا ہے۔ غیر مجاز تبدیلیوں سے بچنے کے لیے ہر عمل آڈٹ لاگ میں محفوظ ہوتا ہے۔

---

## 📊 Dashboard & Analytics | ڈیش بورڈ اور تجزیات
**English:**  
The central hub provides real-time visual and tabular summaries:
- 📊 Class-wise student distribution
- 📅 30-day attendance summary
- 💰 6-month income vs expenses trend
- 📉 Fee status breakdown (Collected vs Arrears)
- 📜 Recent fee & expense tables (Student/Description, Amount, Date)
- 🎓 Exam averages & teacher salary distribution
- 🧮 Profit/Loss & New Admissions calculator (Current Month/Year/Custom Dates)
- 📈 Total Income (Fees + Donations) vs Total Expenses & Salaries

**اردو:**  
ڈیش بورڈ ادارے کی فوری مالی اور تعلیمی صورتحال دکھاتا ہے۔ آپ موجودہ ماہ، سال یا مخصوص تاریخوں کے منافع/نقصان، نئے داخلوں، کل آمدنی اور اخراجات کا فوری جائزہ لے سکتے ہیں۔ تمام گرافس اور ٹیبلز خودکار طور پر ڈیٹا ماڈیولز سے اپ ڈیٹ ہوتے ہیں۔

---

## 🧩 Comprehensive Module Breakdown | مکمل ماڈیولز کی تفصیل

### 1. 🧑‍🎓 Students Management | طلبا کا انتظام
**Fields / فیلڈز:** Admission #, Name, Father’s Name, Class, Admission Date, Contact, Gender, DOB, Blood Group, Guardian/Emergency Contact, Status (Active/Withdrawn/Graduated/Suspended), Previous Education, Address, Photo.  
**System Impact / سسٹم پر اثر:**  
- Drives fee collection, attendance, exams, library, hostel, and certificate modules.
- Status changes auto-update financial liabilities and academic eligibility.
- Links to promotions, ID cards, and Hifz enrollment.

### 2. 👨‍🏫 Teachers Management | اساتذہ کا انتظام
**Fields / فیلڈز:** Name, Subjects, Mobile, Salary, Appointment Date, Qualification, Photo, `Hifz Teacher` toggle.  
**System Impact:**  
- Assigns to classes, timetable, duty roster, and Hifz tracking.
- Salary module pulls fixed amount; attendance deductions apply automatically.
- Hifz toggle restricts/extends access to Quran memorization tracking.

### 3. 🏫 Classes | جماعتیں
**Fields / فیلڈز:** Class Name, Assigned Teacher, Subjects (comma-separated), Monthly Fee.  
**System Impact:**  
- Determines fee structure, timetable periods, attendance registers, and exam grouping.
- Student count auto-calculates. Promotions move students between classes.

### 4. 💳 Fee Structure | فیس ڈھانچہ
**Fields / فیلڈز:** Class, Fee Type (Monthly/Annual/Admission/Special), Amount, Description.  
**System Impact:**  
- Defines payable amounts per student class.
- Auto-calculates dues for fee collection & defaulter reports.
- Late fee amount (from settings) applies automatically to overdue payments.

### 5. 💰 Fee Collection & Quick Receipts | فیس وصولی اور فوری رسیدیں
**Fields / فیلڈز:** Student, Fee Type, Month, Due Amount, Discount, Paid Amount, Net Due, Payment Method (Cash/Bank/Cheque), Date, Note.  
**Features:** Receipt generation/print, selected student history, status summary (Total Collected, Arrears, Current Month/6 Months/Year), Quick Receipt Generator.  
**System Impact:**  
- Updates income dashboard & profit/loss calculator.
- Marks students as cleared/defaulters.
- Syncs with financial reports, audit logs, and donation adjustments.

### 6. 💵 Salaries & Payroll | تنخواہ اور پے رول
**Fields / فیلڈز:** Teacher, Month, Fixed Salary, Absence Days, Deduction, Payable Amount, Remaining, Date, Note.  
**Features:** Auto deduction based on staff attendance, salary slip print, payment tracking.  
**System Impact:**  
- Records as expenses. Affects profit/loss.
- Unpaid amounts roll over to next cycle.
- Links to teacher attendance & appointment dates.

### 7. 📉 Expenses | اخراجات
**Fields / فیلڈز:** Date, Type (Electricity/Water/Gas/Salary/Maintenance/Other), Amount, Paid By, Description, Receipt Image.  
**System Impact:**  
- Directly reduces monthly profit.
- Filters into financial reports & budget planning.
- Image attachment ensures audit transparency.

### 8. 📖 Hifz Department | حفظ ڈیپارٹمنٹ
**Sub-Modules / ذیلی ماڈیولز:**
- **Enrollment / داخلہ:** Student, Hifz Teacher, Start Date, Expected Completion, Current Juz (1-30), Status (Active/Completed/Paused/Withdrawn), Note.
- **Daily Progress / یومیہ پیشرفت:** Date, Attendance (ح/غ/ر), New Lesson (Juz, Pages, Ayah Range, Quality: Excellent/Good/Average/Weak), Previous Revision (Juz list, Quality), Old Revision (Juz list, Quality), Remarks.
- **Review & Exams / جائزہ و امتحان:** Student, Juz, Test Type (New/Revival/Annual), Mistakes, Quality, Result (Pass/Fail), Date, Remarks.  
**System Impact:**  
- Tracks Quran memorization accuracy & consistency.
- Quality/mistake data influences parent reports & teacher evaluations.
- Status updates reflect in student records & certificates (Sanad).

### 9. 📋 Attendance (Students & Staff) | حاضری (طلبا و عملہ)
**Features:** Daily/Monthly registers, Class selection, Marks: Present (ح), Absent (غ), Leave (ر), Save All, Print Register.  
**System Impact:**  
- Student attendance affects academic standing & parent notifications.
- Staff attendance auto-calculates salary deductions.
- Feeds into monthly summaries & defaulters/promotion eligibility.

### 10. 📝 Exams & Results | امتحانات و نتائج
**Fields / فیلڈز:** Exam Name, Class, Subject, Date, Student, Total Marks, Obtained Marks, Percentage, Grade, Result.  
**Features:** Cumulative Result Card Generator, Print/View.  
**System Impact:**  
- Academic performance tracking.
- Results auto-calculate percentages & grades.
- Links to certificates, promotions, and academic reports.

### 11. 🗓️ Timetable & Duty Roster | ٹائم ٹیبل اور ڈیوٹی روسٹر
**Features:** Class selection, Periods 1-6 daily assignment, Save, Print. Teacher Duty Roster view.  
**System Impact:**  
- Prevents teacher overlap & manages workload.
- Syncs with attendance & Hifz scheduling.
- Printable for classroom display.

### 12. 📦 Inventory | انوینٹری
**Fields / فیلڈز:** Name, Type, Quantity, Unit Price, Total Price, Purchase Date, Description.  
**System Impact:**  
- Asset tracking & depreciation awareness.
- Links to expenses if purchased internally.
- Generates inventory reports for audits.

### 13. 📊 Reports | رپورٹس
**Types / اقسام:** Fee Collection, Outstanding Fees, Expenses, Student List, Salary Payments, Attendance Summary, Donations & Zakat, Inventory, Overdue Books, Hostel Report, Defaulters List.  
**Features:** CSV Export, Date/Month Filters, Send Message option.  
**System Impact:**  
- Centralized decision-making data.
- Exportable for accounting software or government submissions.
- Filters isolate specific timeframes or categories.

### 14. 🪪 ID Cards Generator | شناختی کارڈز جنریٹر
**Features:** Print for Students/Teachers, Select Class/Individual/All, Preview, Print.  
**System Impact:**  
- Official identification for exams, events, security.
- Pulls photo, name, class/role, and institute branding.

### 15. ⚠️ Fines & Arrears | جرمانے اور بقایا جات
**Fields / فیلڈز:** Student, Type (Fine/Arrear), Amount, Status (Unpaid/Paid), Date, Description.  
**Features:** Auto late fee apply, manual fine entry, payment tracking.  
**System Impact:**  
- Recovers overdue fees & penalizes repeated delays.
- Updates income dashboard once paid.
- Flags students in defaulter reports.

### 16. 🤲 Donations & Zakat | عطیات اور زکوٰۃ
**Fields / فیلڈز:** Donor Name, Fund Type (Zakat/Sadaqah/Atiyya/Construction), Amount, Mobile, Date.  
**System Impact:**  
- Tracks non-fee income transparently.
- Segregates funds for Shariah compliance.
- Appears in total income & financial reports.

### 17. 📚 Library Management | کتب خانہ مینجمنٹ
**Fields / فیلڈز:** Book Name, Student, Issue Date, Due Return Date, Status (Issued/Returned).  
**System Impact:**  
- Tracks book circulation & overdue penalties.
- Links to student records & defaulters list.
- Generates library reports.

### 18. 🏨 Boarding & Hostel | دارالاقامہ / ہاسٹل
**Fields / فیلڈز:** Student, Room #, Residential Status (Active/Left), Mess Fee, Payment Status (Paid/Unpaid), Check-in, Check-out.  
**System Impact:**  
- Manages accommodation & mess billing.
- Unpaid mess fees roll into arrears.
- Status updates reflect in student records & reports.

### 19. 📜 Certificates & Sanad | اسناد اور سرٹیفکیٹ
**Fields / فیلڈز:** Student, Type (Leaving/Character/Completion Sanad), Grade/Remarks.  
**Features:** Generate, Issued Certificates History Table.  
**System Impact:**  
- Official documentation for transfers, employment, or graduation.
- Auto-logs issuance date & remarks for audit.
- Ties into student status (Graduated/Withdrawn).

### 20. 🎓 Mass Promotions / Year End | سالانہ ترقی
**Fields / فیلڈز:** Source Class, Target Class or Graduated/Archived, Apply Promotion, Undo.  
**Features:** Promotion History Table, Affected Students List.  
**System Impact:**  
- Bulk updates student class assignments or archives graduates.
- Preserves historical records while clearing active sessions.
- Undo feature prevents accidental data loss.

---

## 🔄 Cross-Module Data Flow & System Effects | ماڈیولز کا باہمی تعلق اور ڈیٹا فلو

| Action / عمل | Affected Modules / متاثرہ ماڈیولز | System-Wide Effect / سسٹم پر اثر |
|---|---|---|
| **New Admission** | Students, Fee Structure, Classes, ID Cards, Library, Hostel | Creates financial liability, enables fee collection, generates ID, allocates resources. |
| **Fee Payment** | Dashboard, Profit/Loss, Fines/Arrears, Reports | Updates income, clears defaulter status, recalculates monthly summaries. |
| **Staff Absence** | Attendance, Salaries, Timetable | Triggers automatic salary deduction, affects duty roster, updates payroll reports. |
| **Hifz Progress Entry** | Hifz Module, Student Records, Certificates | Tracks memorization quality, influences Sanad eligibility, updates academic standing. |
| **Class Promotion** | Students, Classes, Exams, Certificates, Dashboard | Moves students academically, archives old records, resets session tracking. |
| **Expense Entry** | Expenses, Profit/Loss, Reports, Inventory (if asset) | Reduces net profit, updates financial summaries, aids budgeting. |
| **Donation Receipt** | Donations, Profit/Loss, Reports | Adds to non-fee income, segregates funds, updates financial transparency. |

**اردو خلاصہ:** سسٹم کے تمام ماڈیولز آپس میں جڑے ہوئے ہیں۔ ایک ماڈیول میں ڈیٹا درج کرنے سے متعلقہ فنانس، رپورٹس، ڈیش بورڈ اور دیگر شعبے خودکار طریقے سے اپ ڈیٹ ہو جاتے ہیں۔ اس سے ڈپلیکیشن، انسانی غلطی، اور ڈیٹا تضاد کا خاتمہ ہوتا ہے۔

---

## ⚙️ Settings & Administration | ترتیبات اور انتظامیہ
### 🔧 General Settings
- Institute Name, Contact, Address
- Report Header / Custom Print Text
- Auto Late Fee Amount (Rs)

### 🎨 Theme & UI
- Color Theme, Font Size (Small/Medium/Large)
- Light/Dark Mode toggle

### 👤 User Management
- Add New User: Full Name, Username, Password, Role (Admin/Teacher/Accountant/Librarian/Teacher Record)
- Password Policy: Min 8 chars, 1 special character required
- Change Password interface

**System Impact:** Controls access levels, enforces security, customizes branding, and standardizes late fee calculations across the platform.

---

## 💾 Backup, Sync & Data Management | بیک اپ، سنک اور ڈیٹا مینجمنٹ
| Feature / خصوصیت | Description / تفصیل |
|---|---|
| **Data Export (ZIP)** | Downloads complete database backup in encrypted ZIP format. |
| **Data Import (ZIP)** | Restores system state. ⚠️ Warning: Overwrites existing data. |
| **Google Drive Sync** | Online/Offline toggle. Auto-syncs backups to cloud. Shows last backup time & size. |
| **Clear Data & Start Fresh** | Deletes all academic/financial records. Preserves Users, Settings, Default Classes. |
| **Load Sample Data** | Inserts 14 demo records per module for testing/training. |
| **Audit Log** | Tracks: User, Role, Action, Module, Details, Timestamp. Export CSV, Clear Log. |

**Security Note / سیکیورٹی نوٹ:** Always export before import. Session auto-logs out after 40 mins of inactivity. Audit logs ensure full accountability.

---

## 🚀 Quick Start & Usage Guide | فوری آغاز اور استعمال کا طریقہ
1. **Login / لاگ ان:** Enter credentials. Demo: `admin/admin@123`.
2. **Setup Institute / ادارہ سیٹ اپ:** Go to Settings → Add Name, Address, Late Fee, Print Header.
3. **Create Classes & Fee Structure / جماعتیں اور فیس:** Define classes, assign teachers, set monthly/annual fees.
4. **Add Students & Staff / طلبا و اساتذہ:** Fill forms, upload photos, assign classes/status.
5. **Record Daily Operations / روزانہ کا کام:** Mark attendance, collect fees, log expenses, track Hifz progress.
6. **Generate Reports & Certificates / رپورٹس اور اسناد:** Use filters → Export CSV or Print ID/Result/Sanad.
7. **Backup Regularly / باقاعدہ بیک اپ:** Use ZIP export or Google Drive sync weekly/monthly.

---

## 📞 Support & Contact | معاونت اور رابطہ
- **Developer:** Yasin Ullah – Bannu Software Solutions  
- **Website:** [www.yasinbss.com](https://www.yasinbss.com)  
- **WhatsApp:** `03361593533`  
- **Support Hours:** Mon–Sat, 9 AM – 6 PM (PKT)  
- **Training & Customization:** Available on request for modules, reports, or UI branding.

---

## ✅ Feature Coverage Checklist | مکمل خصوصیات کی فہرست
- [x] Authentication & Role-Based Access  
- [x] 40-min Session Timeout & Password Security  
- [x] Real-Time Dashboard & Profit/Loss Calculator  
- [x] Student & Teacher Management (Full Forms)  
- [x] Classes, Fee Structure & Collection  
- [x] Quick Receipts & Salary Payroll (Auto Deductions)  
- [x] Expense Tracking with Receipt Upload  
- [x] Hifz Enrollment, Daily Progress (New/Prev/Old), Reviews & Exams  
- [x] Student & Staff Attendance (ح/غ/ر)  
- [x] Exams, Results & Cumulative Report Cards  
- [x] Timetable & Teacher Duty Roster  
- [x] Inventory & Asset Tracking  
- [x] 12+ Report Types + CSV Export  
- [x] ID Card Generator (Students/Teachers)  
- [x] Fines, Arrears & Auto Late Fee  
- [x] Donations & Zakat (Fund Segregation)  
- [x] Library Issuing & Overdue Tracking  
- [x] Hostel/Boarding & Mess Fee Management  
- [x] Certificates & Sanad Generation  
- [x] Mass Promotions & Year-End Archiving  
- [x] General/Theme/User Settings  
- [x] ZIP Backup/Restore, Google Drive Sync  
- [x] Clear Data & Sample Data Loader  
- [x] Complete Audit Log with CSV Export  

---

> 📜 **License & Disclaimer:** This system is proprietary software developed by Bannu Software Solutions. Unauthorized reproduction, redistribution, or reverse engineering is prohibited. All data remains the property of the licensed institute. Regular backups are the responsibility of the administrator.  
> ⚖️ **Disclaimer:** The system is designed for operational efficiency. Financial/academic decisions should be verified by authorized personnel. Data integrity depends on accurate daily entry and routine backups.

---
🖨️ **Ready for Client Handover | کلائنٹ کے حوالے کے لیے تیار**  
📦 **Version:** 1.0 | 🌐 **Bilingual Documentation (EN/UR)** | 🔒 **Secure & Audited**