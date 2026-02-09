# Educational SaaS Platform Requirements

## Project Overview
A multi-tenant SaaS platform for educational institutions (public and private schools). The platform provides separate interfaces and functionalities for Super Admins, School Admins, Teachers, and Students.

## User Roles
1. **Super Admin**: 
   - Manage all schools (tenants).
   - Subscription management.
   - Platform health monitoring.
2. **School Admin**:
   - Manage school-specific data (users, classes, settings).
   - Financial dashboard (Private schools only).
3. **Teacher**:
   - Class management.
   - Grading (Exams, Assignments).
   - Content upload.
   - Attendance tracking via QR Codes.
   - Communication with students.
4. **Student**:
   - Access course materials.
   - View grades and schedule.
   - Mark attendance via QR Scan.
   - Direct messaging with teachers.

## key Features

### Core Academic
- **Smart QR Attendance**:
  - Teacher generates unique QR per session.
  - Student scans -> Marked Present -> Content Unlocked/Downloaded.
- **Communication Hub**:
  - Real-time chat/messaging between Teacher and Student.
- **LMS (Learning Management System)**:
  - Grading system (Exams, Tutorials, Oral participation).
  - Assignments with due dates and submissions.
- **Calendar**:
  - Visual schedule.
  - Integration with attendance logs.

### Financial Module (Private Schools)
- **Tuition Management**:
  - Track payments, overdue flags, reminders.
- **Invoicing**:
  - Auto-generate receipts/invoices.
- **Payroll**:
  - Calculate teacher salary based on hours/sessions (verified by QR logs).
- **Financial Dashboard**:
  - Revenue, outstanding payments, expenses.

## Technical Architecture & Design
- **Frontend**: Next.js (React)
- **Styling**: Vanilla CSS (CSS Modules/Variables) with Premium Aesthetics (Glassmorphism, Dark Mode).
- **Database Strategy**: Multi-tenant architecture (SchoolID partitioning) - *Simulated in this prototype*.
- **Authentication**: Role-based access control (RBAC).

## Design Guidelines
- **Aesthetic**: Premium, Modern, Dynamic.
- **Theme**: Dark/Light mode support, vibrant accent colors.
- **Interactions**: Smooth transitions, hover effects. 
