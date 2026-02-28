# AppraisePro

AppraisePro is a Faculty Performance Appraisal Web Application built using the **Frappe Framework**. It enables institutions to evaluate engineering faculty performance using structured KPI-based forms, automated scoring, reviewer workflows, and analytics dashboards.

---

## 📌 Overview

AppraisePro digitizes the faculty appraisal process by:

- Collecting structured KPI data across multiple performance categories
- Computing self-appraisal scores using predefined weightages
- Supporting reviewer scoring and approval workflows
- Providing analytics dashboards for institutional insights
- Generating PDF reports and sending email notifications

The system ensures transparency, efficiency, and role-based access control throughout the appraisal cycle.

---

## 🚀 Features

### 🗂 KPI-Based Evaluation
- 50 KPIs organized into 6 modules:
  - Academic Involvement
  - Student Development
  - Administrative Activities
  - Research
  - Consultancy & Corporate Training
  - Product Development

### 👥 Role-Based Access Control
- Administrator
- Performance Appraisal (PA) Team
- Faculty
- Department Executive / Reviewer
- External Viewer

### 📝 Workflow
1. Faculty fills appraisal forms.
2. Self-appraisal score is calculated automatically.
3. Reviewer reviews, approves, and assigns reviewer score.
4. Approved forms become read-only (can be revoked by reviewer).

### 📊 Analytics & Reporting
- Filter by department, semester, academic year, module
- Track KPI progress and performance summaries
- Export reports as PDF
- Email notifications

### ⚙️ Technical Features
- Built on Frappe Framework (Python + JavaScript)
- SQL database backend
- Redis caching
- Background job processing
- Evidence upload handling
- Light/Dark theme support

---

## 🏗 Architecture

- **Backend:** Python (Frappe Framework)
- **Frontend:** JavaScript (Frappe Desk UI)
- **Database:** MariaDB / PostgreSQL
- **Caching:** Redis
- **Background Jobs:** Frappe Worker & Scheduler
- **PDF Generation:** wkhtmltopdf (or Frappe-supported engine)

---

## 🛠 Installation

### Prerequisites

- Python (compatible with your Frappe version)
- Node.js
- Redis
- MariaDB / PostgreSQL
- wkhtmltopdf
- Frappe Bench CLI


### Installation

You can install this app using the [bench](https://github.com/frappe/bench) CLI:

```bash
cd $PATH_TO_YOUR_BENCH
bench get-app $URL_OF_THIS_REPO --branch develop
bench install-app appraise
```
