# 🎨 User Interface (UI/UX)

## Principles

- Mobile-first, responsive, card-based design.
- WCAG 2.1 compliance (contrast, keyboard nav, ARIA labels).
- 8px spacing grid, consistent buttons/icons.

## Core Pages

### Login (`/login`)

- SSO (Google OAuth), CoopBank logo.
- Input validation, error messages.

### Employee Dashboard (`/employee/dashboard`)

- Search + filters, mentor/resource cards, “My Mentorships.”
- Lazy loading, clickable cards.

### Employee Profile (`/employee/profile`)

- Editable personal info, skills (multi-select + proficiency), goals.
- Tabbed interface (Personal Info, Skills Offered, Skills Desired).

### Admin Dashboard (`/admin/dashboard`)

- KPI cards, Recharts charts, real-time updates.
- Export CSV/PDF.

### Admin Employees (`/admin/employees`)

- Searchable/sortable table, pagination.
- Role assignment, audit logs.

### Admin Resources (`/admin/resources`)

- Add/edit form, bulk import (drag-drop).
- Tag chips, URL validation.
