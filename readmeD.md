# 📚 مدرسہ مینجمنٹ سسٹم (Madrasa Management System)

[![Live Demo](https://img.shields.io/badge/Live-Demo-green?style=for-the-badge&logo=githubpages)](https://yasinullah.github.io/myMadrasaApp/)
[![Download APK](https://img.shields.io/badge/Download-APK-orange?style=for-the-badge&logo=android)](https://github.com/yasinullah/myMadrasaApp/raw/main/app-release.apk)
[![PWA](https://img.shields.io/badge/PWA-Installerable-blue?style=for-the-badge&logo=pwa)](https://yasinullah.github.io/myMadrasaApp/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

> **Bannu Software Solutions** – Developed by **Yasin Ullah**  
> WhatsApp: 03361593533 | Website: [www.yasinbss.com](https://www.yasinbss.com)

---

## 🌟 Overview (تعارف)

This is a **complete, offline‑first Progressive Web Application (PWA)** for managing all aspects of a Madrasa or Islamic school. It works entirely inside your browser using **IndexedDB** – no external server or internet required after installation. All data stays on the user’s device, and optional **Google Drive sync** provides cloud backup & restore.

یہ ایک **مکمل، آف لائن‑فرسٹ پروگریسو ویب ایپلیکیشن (PWA)** ہے جو مدرسہ یا اسلامی اسکول کے تمام شعبوں کو سنبھالنے کے لیے بنائی گئی ہے۔ یہ **IndexedDB** کا استعمال کرتے ہوئے براؤزر میں چلتی ہے – انسٹالیشن کے بعد کسی سرور یا انٹرنیٹ کی ضرورت نہیں۔ تمام ڈیٹا صارف کے آلے پر محفوظ رہتا ہے، اور **گوگل ڈرائیو سنک** بیک اپ اور بحالی کا اختیار فراہم کرتا ہے۔

**Key Features (اہم خصوصیات):**
- ✅ **Offline‑First** – Works without internet
- ✅ **PWA Installable** – Use like a native app on mobile/desktop
- ✅ **Android APK** – Also available as an installable APK
- ✅ **Multi‑Role** – Admin, Teacher, Accountant, Librarian
- ✅ **RTL Support** – Full Urdu interface with right‑to‑left layout
- ✅ **Complete Modules** – Students, Teachers, Classes, Fees, Hifz, Attendance, Exams, Library, Hostel, Inventory, Certificates, Promotions, Reports…
- ✅ **Google Drive Sync** – Backup & restore to/from cloud
- ✅ **Print & PDF** – Receipts, salary slips, result cards, ID cards, reports
- ✅ **Audit Log** – Tracks all user actions

---

## 📥 Installation (انسٹالیشن)

### 🌐 Web / PWA (Website)
1. Open [https://yasinullah.github.io/myMadrasaApp/](https://yasinullah.github.io/myMadrasaApp/) in Chrome / Edge / Firefox / Safari.
2. Click the **“Install”** or **“Add to Home Screen”** button in your browser (look for the download icon in the address bar).
3. The app will install like a native application and launch in its own window.

### 📱 Android APK
1. Download the APK from: [https://github.com/yasinullah/myMadrasaApp/raw/main/app-release.apk](https://github.com/yasinullah/myMadrasaApp/raw/main/app-release.apk)
2. Enable **“Install from unknown sources”** in your Android settings.
3. Open the APK and install it.

> 💡 **Note:** The APK is a wrapper of the same PWA – all data is stored locally on the device.

---

## 🔐 Demo Credentials (ڈیمو لاگ ان)

| Role (کردار)  | Username (صارف نام) | Password (پاس ورڈ)   |
|---------------|---------------------|----------------------|
| Admin (ایڈمن) | `admin`             | `admin@123`          |
| Teacher       | `teacher`           | `Teacher@123`        |

> After logging in, you can create more users from **Settings → Users**.

---

## 📖 Complete Feature Guide (مکمل فیچر گائیڈ)

Below is a detailed explanation of every module, button, and its effect on the system.

---

### 1️⃣ Dashboard (ڈیش بورڈ)

**What it shows:**  
- Statistical cards (total students, teachers, classes, today’s income/expenses, total profit/loss)
- Pie/bar charts: students per class, attendance trend (last 30 days), income vs expenses (6 months), fee status (paid vs due), exam averages, teacher salary distribution
- Recent fee collections and expense records
- Alert panel: fee defaulters, overdue books, low stock items
- **Profit/Loss & Admissions Calculator** – select month/year/custom range to see total income (fee+donations), total expenses (expenses+salary), net profit, and new admissions

**Effect on system:**  
- Charts and stats update automatically based on live data
- Alerts help you take action (e.g., remind defaulters, restock inventory)

---

### 2️⃣ Students (طلبا)

**Features:**
- **Add / Edit / Delete** student record  
  Fields: Enrollment No, Name, Father’s Name, Class, Enrollment Date, Contact, Address, Gender, DOB, Blood Group, Guardian Name, Emergency Contact, Status (Active/Withdrawn/Graduated/Suspended), Previous Education, Photo (upload & compress)
- **View Student Detail** – modal with tabs showing:  
  - Personal info + photo  
  - Fee history + total paid  
  - Attendance summary (present/absent/leave percentages)  
  - Exam results (all subjects)  
  - Fines/Arrears (paid/unpaid)  
  - Library books issued  
  - Hostel allocation (if any)
- **Bulk actions** – mass promotion, filter by class
- **Search & filter** via DataTable (global search, class filter)

**Effect:**  
- A student can be enrolled, updated, or removed. All linked records (fees, attendance, exams, fines, library, hostel) remain in the system (but are shown in detail view).

---

### 3️⃣ Teachers (اساتذہ)

**Features:**
- **Add / Edit / Delete** teacher  
  Fields: Name, Subjects, Mobile, Salary, Appointment Date, Qualification, Photo, “Hifz Teacher” checkbox
- **View Teacher Detail** – shows:  
  - Personal info + photo  
  - Assigned classes (list)  
  - Salary history (all payments, balance)  
  - Attendance summary (staff attendance)
- **Teacher Duty Roster** (under Timetable module) – displays which periods/classes the teacher is assigned
- **Salary slip** generation & print

**Effect:**  
- Teachers can be assigned to classes and Hifz students. Their salary is used in payroll, and attendance affects deductions.

---

### 4️⃣ Classes (جماعتیں)

**Features:**
- **Add / Edit / Delete** class  
  Fields: Class Name, Assigned Teacher, Subjects (comma‑separated), Monthly Fee
- List shows: class name, teacher, subjects, monthly fee, number of students
- **View Class Detail** – shows:  
  - Basic info  
  - List of students in that class  
  - Fee collection summary (total collected vs expected)  
  - Exam summary (average percentages, pass/fail per exam)  
  - Attendance summary

**Effect:**  
- Classes are the core grouping for students, fees, exams, and timetable. Deleting a class does **not** delete students – their `classId` becomes orphaned (you should re‑assign them).

---

### 5️⃣ Fee Structure (فیس ڈھانچہ)

**Features:**
- Define fee types per class: Monthly, Annual, Admission, Special
- Each entry: Class, Type, Amount, Description
- Used as default amount when collecting fees

**Effect:**  
- When you collect a fee for a student, the amount is auto‑filled from the structure. You can still override.

---

### 6️⃣ Fee Collection (فیس وصولی)

**Features:**
- **Collect fee** – select student, fee type, month, amount (auto from structure), discount, paid amount, method (cash/bank/cheque), date, note
- **Sibling discount** – if another active student has the same father name and contact, a discount % (default 10%) is applied automatically (can be changed in settings)
- **Auto receipt number** (`REC-XXXX`)
- **Print receipt** (modal with print button)
- **Edit / Delete** collection record
- **Fee summary** at top: total paid, total due, current month paid, last 6 months paid, current year paid
- **Filter** by student, date range
- **Student fee history** – when you select a student in the collection modal, a table below shows all previous payments
- **Late fee automation** – from Fines module: click “Apply Automated Late Fees” to add a penalty (default Rs 500) to all students who haven’t paid the current month

**Effect:**  
- Reduces the student’s due balance. Receipts can be printed for parents. All collection records appear in reports and dashboard.

---

### 7️⃣ Fines & Arrears (جرمانے و بقایا)

**Features:**
- Add fine/arrear: student, type (Fine / Arrear), amount, status (paid/unpaid), date, description
- Edit / delete
- **Apply Automated Late Fees** – adds a penalty to all students who missed monthly fee (amount from Settings → General → Late Fee Amount)
- **Defaulters Report** (under Reports) – lists students with unpaid monthly fees

**Effect:**  
- Unpaid fines appear in student detail view and can be collected later. They affect total due in fee summaries (if you mark them paid manually, they are considered income).

---

### 8️⃣ Donations & Zakat (عطیات و زکوٰۃ)

**Features:**
- Add donation: donor name, fund type (Zakat/Sadaqah/General/Construction), amount, mobile, date
- Auto receipt number (`DON-XXXX`)
- Print donation receipt
- Filter by fund type
- View all donations in a table

**Effect:**  
- Donations are added to total income (dashboard, reports, profit/loss calculator).

---

### 9️⃣ Salary & Payroll (تنخواہ)

**Features:**
- **Pay salary** – select teacher, month, fixed salary (auto from teacher record), absent days auto‑calculated from staff attendance, deduction, paid amount, balance, date, note
- Auto salary slip number (`SAL-XXXX`)
- Print salary slip
- View all salary payments (table with teacher, month, paid, balance)
- Salary distribution chart on dashboard

**Effect:**  
- Reduces balance owed to teacher. Salary expenses are included in total expenses (reports, profit/loss).

---

### 🔟 Expenses (اخراجات)

**Features:**
- Add expense: date, category (Electricity/Water/Gas/Salary/Repair/Other), amount, paid to, detail, receipt image (upload & compress)
- Edit / delete
- Filter by date range and category

**Effect:**  
- Expenses appear in reports and reduce net profit. Receipt images can be stored for audit.

---

### 1️⃣1️⃣ Hifz Department (حفظ ڈیپارٹمنٹ)

A complete subsystem for Quran memorization tracking.

**Tabs:**

#### a) Hifz Students
- **Enroll** a regular student into Hifz: select student, Hifz teacher, start date, target completion date, current juz (1‑30), status (Active/Completed/Paused/Withdrawn)
- **List** all Hifz students with current juz, progress percentage, status
- **Edit / delete** enrollment

#### b) Daily Progress (یومیہ پیشرفت)
- **Add progress entry** – date, student, attendance (Present/Absent/Leave)  
  Then enter three parts:
  1. **Sabaq (نیا سبق)** – juz, pages, from‑to ayah, quality (Excellent/Good/Average/Weak)
  2. **Sabqi (سبقی)** – revision of recent juz (comma‑separated list of juz numbers), quality
  3. **Manzil (منزل)** – old revision (comma‑separated juz), quality
- View progress table (date, student, sabaq details, sabqi, manzil, attendance)
- Edit/delete progress entries

#### c) Juz Tracker (جز ٹریکر)
- Select a Hifz student → displays a 30‑cell grid (juz 1‑30) with colour coding:
  - **Completed** (green)
  - **In Progress** (gold)
  - **Completed but pending review** (blue)
  - **Not Started** (grey)
- **Tracking mode** – switch between Juz mode and Surah mode (interface ready, Surah mode can be extended)
- Progress bar shows percentage completion

#### d) Evaluations (امتحانات و جائزہ)
- Add test/evaluation: student, juz number, evaluation type (Sabaq Test/Daura/Annual), mistakes count, quality, result (Pass/Fail), date, remarks
- View all evaluations in a table
- Used to assess student’s memorisation quality

**Effect:**  
- Hifz teachers can track daily progress, identify weak areas, and generate reports. The juz grid gives a visual overview of a student’s journey.

---

### 1️⃣2️⃣ Attendance (حاضری)

**Two modes:**

#### Daily Attendance (یومیہ)
- Select class, date
- Each student has three buttons: Present (ح), Absent (غ), Leave (ر)
- **“All Present” / “All Absent”** shortcuts
- Save – updates attendance records

#### Monthly Register (ماہانہ رجسٹر)
- Select class, month (YYYY‑MM)
- Table shows all days of the month with coloured cells for Present/ Absent/Leave
- Summary columns: total Present, Absent, Leave per student
- **Print register** – prints the monthly attendance sheet

**Effect:**  
- Attendance is used in:  
  - Student detail view (attendance percentage)  
  - Teacher salary deduction (absent days are counted from staff attendance)  
  - Reports

**Staff Attendance (عملہ حاضری)** – separate page:  
- Select date, mark each teacher Present/Absent/Leave, save.  
- Used for salary deduction.

---

### 1️⃣3️⃣ Exams & Results (امتحان و نتائج)

**Features:**
- Add exam result: exam name, class, student, subject, date, total marks, obtained marks  
  → Percentage, grade, pass/fail auto‑calculated (grading scheme customizable)
- Edit / delete exam records
- **Result Card** – prints a detailed card for a single exam (includes rank within exam)
- **Cumulative Result Card Generator** – select an exam name and a student → shows all subjects for that exam with total, percentage, grade, rank
- **Annual Cumulative Result Card** – for a student, shows all subjects across all exams of the year, with overall percentage and grade

**Effect:**  
- Exam data appears in student detail view, dashboard exam average chart, and reports.

---

### 1️⃣4️⃣ Timetable (ٹائم ٹیبل)

**Features:**
- Create timetable for a class: 6 periods × 6 days (Monday to Saturday)
- Click any cell → edit subject, teacher, start time, end time
- **Conflict detection** – warns if same teacher is already assigned at the same period in another class (but allows override)
- Save timetable to database
- **Print timetable** for a class
- **Teacher Duty Roster** – select a teacher → shows all periods/classes where they are assigned

**Effect:**  
- Helps organise daily schedule. Teachers’ duty roster helps manage workload.

---

### 1️⃣5️⃣ Library (کتب خانہ)

**Features:**
- **Issue book** – book name, student, issue date, due date, status (Issued/Returned)
- Edit / delete issue record
- **Overdue detection** – when returning a book past due date, system asks if you want to add a fine (configurable fine per day in settings)
- **Inventory stock adjustment** – when a book is issued, quantity in inventory decreases (if a matching inventory item exists); increases on return
- **Overdue books report** (under Reports) – lists all books not returned past due date

**Effect:**  
- Tracks who borrowed what and when. Overdue fines increase revenue.

---

### 1️⃣6️⃣ Hostel (دارالاقامہ)

**Features:**
- **Allocate room** – student, room number, resident status (Active/Left), monthly mess fee, fee status (Paid/Unpaid), check‑in date, check‑out date
- **Room capacity check** – when adding a new resident, system checks if room has reached capacity (default 4, can be changed in settings)
- Edit / delete hostel record
- **Hostel Report** – shows all residents, mess fee due status

**Effect:**  
- Manages boarding students, mess fee collection, and room occupancy.

---

### 1️⃣7️⃣ Inventory (انوینٹری)

**Features:**
- Add/edit inventory item: name, category, quantity, unit price, purchase date, description  
  → Total price auto‑calculated
- View all items in a table (stock levels)
- **Low stock alert** – on dashboard, items with quantity < 5 are highlighted
- When a library book is issued that matches an inventory item (by name), quantity decreases; increases on return (if status changed to Returned)

**Effect:**  
- Helps track assets, textbooks, stationery. Prevents over‑issuing.

---

### 1️⃣8️⃣ Certificates (اسناد و سرٹیفکیٹ)

**Features:**
- Generate three types:
  - **Leaving Certificate** (اسکول چھوڑنے کا سرٹیفکیٹ)
  - **Character Certificate** (کردار کا سرٹیفکیٹ)
  - **Sanad** (سند تکمیلِ تعلیم)
- Select student, add remarks (e.g., “Excellent behaviour”)
- Preview certificate in a styled template (includes madrasa name, student details, signatures)
- Print / save as PDF
- **Issued certificates list** – shows all generated certificates with date, type, remarks
- Delete certificate

**Effect:**  
- Automates the issuance of official documents to students.

---

### 1️⃣9️⃣ Promotions (سالانہ ترقی)

**Features:**
- **Mass promotion** – select source class, target class (or “Graduated / Archived”)
- Preview list of students in source class
- Click **“Apply Promotion”** – all students are moved to the target class (or status changed to Graduated)
- **Undo last promotion** – reverts the most recent promotion (only possible within 30 days)
- **Promotion history** – shows all past promotions (student, from class, to class, date)

**Effect:**  
- Saves time at the end of academic year. Graduated students no longer appear in active student lists but their records remain in the database.

---

### 2️⃣0️⃣ Reports (رپورٹس)

**Available report types:**
- Fee Collection (detailed, with date range)
- Due Fees (students with unpaid monthly fees)
- Expenses (by date range & category)
- Student List (all students with basic info)
- Salary Payments (all teacher salary records)
- Attendance Summary (per student: present/absent/leave counts & percentage)
- Donations & Zakat
- Inventory Report (all items with total value)
- Overdue Books (library books not returned on time)
- Hostel Report (current residents & mess fee due)
- Defaulters List (students who didn’t pay current month’s fee)

**Features:**
- Filter by date range
- **Export to CSV** (for fee, expenses, etc.)
- **Print** the report
- **Download as PDF** (using html2pdf)
- **Share via WhatsApp / SMS** – opens a pre‑filled message with report summary

**Effect:**  
- Provides printable/exportable data for accounting, auditing, and management.

---

### 2️⃣1️⃣ ID Cards (شناختی کارڈز)

**Features:**
- Choose type: Students or Teachers
- Filter by class (for students)
- Select a specific individual or “All”
- Click **“Generate ID Cards”** – preview all cards in a grid
- **Print** all cards at once (each card 240×360px, designed for printing on A4/ card stock)

**Effect:**  
- Quickly produce identity cards for students/staff.

---

### 2️⃣2️⃣ Settings (ترتیبات)

#### General Settings
- Madrasa / School Name
- Contact Number
- Address
- Print Header (custom text on receipts/reports)
- Late Fee Amount (for automated late fee)

#### Theme
- Choose from 5 colour schemes (Green, Blue, Purple, Gold, Red)
- Font size (Small / Medium / Large)
- Light / Dark mode

#### User Management
- Add new users (Full name, Username, Password, Role: Admin / Teacher / Accountant / Librarian)
- For Teacher role, optionally link to an existing teacher record (so the teacher can log in and see only their classes)
- Delete users (cannot delete own account)

#### Change Password
- For currently logged‑in user (requires old password, validates strength)

#### Data Backup & Restore
- **Export Data (ZIP)** – downloads all IndexedDB stores as a ZIP file containing `madrasa_database.json`
- **Import Data (ZIP)** – upload a previously exported ZIP to completely replace the database (warning: existing data is erased)
- **Clear All Data** – deletes everything (except users and settings) and re‑runs initial seed
- **Start Fresh (Clear Data & Reset)** – deletes all students, teachers, fees, attendance, exams, etc., but keeps users, settings, and default classes (8 classes created)
- **Load Sample Data** – inserts 14 sample records in each major module (students, teachers, classes, fees, expenses, salaries, attendance, exams, library, hostel, inventory, fines, donations, certificates) – useful for demonstration

#### Google Drive Sync (Cloud Backup)
- **Connect** – OAuth 2.0 login (requires a Google Cloud project with Drive API enabled – see notes below)
- **Backup** – uploads a ZIP backup to your Google Drive’s **appDataFolder** (hidden, only accessible by the app)
- **Restore** – downloads the latest backup from Drive and restores the entire database
- **Fresh Backup** – deletes the old backup file from Drive and uploads a new one
- **Disconnect** – revokes access token

> ⚠️ **Important:** To use Google Drive sync, you need to create your own OAuth 2.0 Client ID (Web application) in Google Cloud Console and replace `CLIENT_ID` in `index.html`. The current code includes a placeholder. Detailed instructions are shown when you click “Connect”.

#### Audit Log (آڈٹ لاگ)
- Records every user action (Add, Edit, Delete, Login, etc.) with timestamp, user, role, module, detail
- Filter by date range and module
- Export to CSV
- Clear log (admin only)

---

### 2️⃣3️⃣ Additional Utilities

- **Quick Receipt Generator** – for walk‑in payments (non‑student): enter name, category, amount → print receipt.
- **Profit/Loss Calculator** (on Dashboard) – dynamic range selection.
- **Idle & Absolute Session Timeout** – after 40 minutes of inactivity, you are logged out; after 8 hours total, session expires.
- **Responsive Mobile Layout** – bottom navigation bar appears on phones, sidebar collapses on tablets.
- **PWA** – can be installed as an app and used offline.

---

## 🛡️ Role‑Based Access Control

| Role (کردار)      | Allowed Sections (اجازت یافتہ صفحات)                                                                                           |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------|
| **Admin**         | Everything (full access)                                                                                                      |
| **Teacher**       | Dashboard, Students (own classes only), Attendance (own classes), Exams (own classes), Timetable, Certificates, Hifz           |
| **Accountant**    | Dashboard, Students (view only), Fee Structure, Fee Collection, Salary, Expenses, Fines, Donations, Reports                    |
| **Librarian**     | Dashboard, Library, Inventory, Reports (limited)                                                                              |

Teachers cannot delete or edit students/classes; they can only view and take attendance/enter results for their assigned classes.

---

## 💾 Data Management (ڈیٹا کا نظم)

| Action                          | Effect                                                                                                                                 |
|---------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| **Export (ZIP)**                | Saves a complete snapshot of all data (students, fees, attendance, etc.) as a ZIP file.                                               |
| **Import (ZIP)**                | Replaces the current database with the uploaded one. **Use with caution** – existing data is lost.                                    |
| **Clear All Data**              | Deletes everything and re‑initialises default users (admin, teacher) and empty database.                                              |
| **Start Fresh**                 | Deletes all operational data (students, teachers, fees, etc.) but keeps users, settings, and default classes (8 classes).             |
| **Load Sample Data**            | Inserts 14 demo records per module – useful for testing or showcasing the app.                                                        |
| **Google Drive Sync**           | Backup / restore to cloud. Files are stored in Google’s `appDataFolder` (not visible in user’s Drive root).                          |

---

## 🔒 Security & Session

- Passwords are hashed (simple non‑cryptographic hash, sufficient for local usage).
- Session idle timeout: **40 minutes** → automatic logout.
- Absolute session timeout: **8 hours** → logout even if active.
- After logout, all data remains in IndexedDB; user must log in again.

---

## ❓ Troubleshooting (مسائل کا حل)

| Issue                               | Solution                                                                                                                                      |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| App doesn’t load / blank screen     | Clear browser cache and reload. Ensure you are using a modern browser (Chrome, Edge, Firefox).                                                |
| Data lost after browser clear       | IndexedDB is cleared when user clears site data. **Backup regularly** using Export or Google Drive.                                           |
| Cannot log in                       | Use demo credentials: `admin` / `admin@123`. If you changed password and forgot, you must clear site data (which deletes all users) or re‑import a backup. |
| Google Drive sync not working       | You must create your own OAuth 2.0 Client ID in Google Cloud Console and replace `CLIENT_ID` in the HTML. See the popup when clicking “Connect”. |
| Print / PDF not working             | Some browsers block automatic print; use the print button in the print dialog. PDF generation requires `html2pdf` library (included).        |
| Teacher cannot see students         | Ensure the teacher is linked to a class in the class settings and that the teacher’s user account is linked to the correct teacher record.   |
| “Sibling discount” not applying     | Two students must have the same **father name** and **contact number**. The discount percentage can be changed in the database (default 10%). |

---

## 📞 Support & Contact

**Developed by:** Yasin Ullah – Bannu Software Solutions  
**Website:** [www.yasinbss.com](https://www.yasinbss.com)  
**WhatsApp:** 03361593533  
**GitHub Repository:** [https://github.com/yasinullah/myMadrasaApp](https://github.com/yasinullah/myMadrasaApp)

For customisation, deployment assistance, or feature requests, please reach out via WhatsApp or email.

---

## 📜 License

This project is open source under the **MIT License**. You are free to use, modify, and distribute it for personal or commercial use, provided you retain the original copyright notice.

---

---

## 🆕 Recently Added Features & Updates

### 📥 Pre‑Login Data Management
New options on the login page before signing in:
- **Restore from Google Drive** – download backup from Drive before login
- **Import from File** – upload ZIP export before logging in
- **Sync Before Login** – fetch latest Drive backup then log in

### 🧾 Quick Receipt Generator
Generate receipts for non‑student payments (walk‑in donations, book sales, etc.). Access from Fee Collection page.

### 👥 Active Users Panel
Sidebar displays real‑time active user count and user list (multi‑tab support).

### 🔄 Sync Status Bar
Status indicator at the bottom of the sidebar. Click to trigger manual sync.

### 📚 Library Enhanced
- **Books Catalog**: Separate book inventory (name, author, total, available)
- **Issue/Return**: Separate lending transaction tracking
- Stock auto‑updates from Inventory

### 🛏️ Hostel Enhanced
- **Rooms Catalog**: Separate room management (room number, capacity)
- **Capacity Validation** (configurable max)
- **Residents**: Separate allocation table

### 🏅 Donors Management
- Separate donors catalog with donation history
- Quick donation entry for existing donors

### 📚 Academic Year Management
- Create/manage academic years
- End‑of‑year promotion wizard
- Archive promotion records

### 🆔 Combined Documents Page
Unified page for: Student ID, Teacher ID, Leaving Certificate, Sanad/Completion, Character Certificate

---

**© 2026 Bannu Software Solutions – All Rights Reserved**  
*Made with ❤️ for the Ummah*