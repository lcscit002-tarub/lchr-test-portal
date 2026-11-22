# LC Employee + HR Portal v2 — Design-First Build

This version intentionally focuses on UI/UX and workflow validation before Supabase deployment.

## Role entry flow
- Welcome page first shows EMPLOYEE / MANAGER / HR.
- Each selection opens its own role-specific login route/state.
- Demo buttons are included for testing without a backend.
- Production authentication will be connected to Supabase later.

## Design direction
The portal uses the supplied Luo City Spa Club login artwork as the visual foundation and follows the supplied portal design language: dark wood/brown, cream panels, rounded/soft cards, serif headings, top search, welcome/profile area, date/time, and aligned modals.

## Requirements reflected
- Employee Schedule Request is only for Change Work Hours / Change Rest Day.
- Employee Leave and Offset Request contains Vacation Leave, Sick Leave, Holiday Offset and other leave types.
- HR salary page supports editing Salary Pay and attaching a payslip. No payroll calculation.
- Attendance page has employee search and separates records by employee ID.
- Import UI accepts CSV/XLSX and is designed for validation before Supabase writes.
- CR: 10 minutes per session, multiple sessions, separate overbreak calculation.
- Meal: 60 minutes OR 30-minute x2 configuration, separate overbreak per session.
- Schedules support dated assignments, OFF days and overnight shifts.
- Manager is first reviewer; HR has final authority and may intervene if manager is unresponsive. Overall request expiry remains 48 hours. Urgent requests are highlighted.
- Profile modal follows the supplied reference: split form/preview, full name read-only, email/contact editable, title/department read-only, cancel/save actions.

## Next phase
After visual/workflow approval, connect Supabase Auth, PostgreSQL/RLS, Storage and realtime subscriptions. Do not place confidential production employee data into this design demo yet.
