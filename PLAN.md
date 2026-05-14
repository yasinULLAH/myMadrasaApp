# Implementation Plan for Madrasa Management System

## Phase 1: Foundation & Dependencies
- Add CDNs for PDF generation (`html2pdf.js` or `jspdf`) and charting (`Chart.js`).
- Expand IndexedDB stores to support new modules: `academicYears`, `libraryBooks`, `libraryIssues`, `hostelRooms`, `hostelAllocations`, `fines`, `donations`, `certificates`.

## Phase 2: RBAC & Media Handling
- **RBAC**: Restrict Teacher role to only view data (students, attendance, results) for classes they are assigned to.
- **Media**: Add file input for base64 image conversion to support student/staff profile pictures and expense receipts.

## Phase 3: Academic Year & Promotions
- Add "Academic Year" settings module.
- Implement "Promote Students" feature to batch update student classes.
- Tag relevant historical records (fees, attendance, results) with the academic year for archiving.

## Phase 4: Missing & Partial Modules Implementation
- **Library (Kutub Khana)**: Complete the book inventory, issue, and return tracking logic.
- **Hostel (Dar-ul-Iqama)**: Complete room management, student allocation, and specific hostel fee tracking.
- **Fines & Arrears**: Add fine/arrears recording modal and late-fee penalties integration into fee collection.
- **Zakat / Donations**: Complete donor tracking, fund categorization, and separate donation receipts.

## Phase 5: ID Cards & Certificates
- **ID Cards**: Create a printable template/view for generating Student and Teacher ID cards (incorporating their photos).
- **Leaving Certificate / Sanad**: Create a template and generation form for graduating/leaving students.

## Phase 6: Enhancements (Dashboard to Settings)
- **Dashboard**: Add Quick stat cards (Profit/Loss, New Admissions), Exam Average Chart, and Salary Distribution Chart.
- **Fee & Salary**:
  - Add student fee history table within the fee collection view.
  - Split action buttons: 'Collect Fee' and 'Generate Receipt'.
  - Add dynamic duration filters (total, this month, last 6 months, this year).
- **Attendance**:
  - Add toggle for marks (ح/غ/ر vs ✓/✗/—).
  - Add specific Month filter and a dedicated 'Print Register' button.
  - Enable simultaneous Date/Month filtering.
- **Timetable**:
  - Add specific start/end time inputs for periods.
  - Add "Teacher Duty Roster" view.
- **Results**:
  - Build a dedicated Result Card viewer/filter with print capabilities.
  - Add auto-calculating grade/percent column in the result entry table.
- **Reports**:
  - Add multi-month/year filters and separate fee breakdowns.
  - Add native PDF generation and CSV export capabilities.
  - Add a "Send Message" (WhatsApp/SMS link) button post-generation.
- **Settings**:
  - Enhance Print Settings section.
  - Add explicit data import warning note.
  - Add class filter in the fee structure view.
