# 🌐 Caritas GRD Web Platform

> Full-stack web platform for disaster risk management, developed for **Cáritas Lima** as part of the Software Implementation Project at Pontificia Universidad Católica del Perú (PUCP).

The platform centralizes disaster risk management operations, allowing administrators and volunteers to manage disaster incidents, emergency resources, training activities, humanitarian aid distribution, and disaster preparedness through a unified web interface.

---

# 📖 Overview

The Caritas GRD Web Platform serves as the central management system for the Unified Disaster Risk Management (GRD) project.

It provides administrative tools for coordinating emergency response activities while integrating with the Android mobile application used by field volunteers. Data collected in the mobile application can be synchronized with the central platform, enabling both offline field operations and centralized information management.

---

# ✨ Key Features

- Secure authentication and authorization
- Disaster incident management
- Volunteer (brigadista) management
- Disaster drill administration
- Emergency kit management
- Training course administration
- Donation management
- Interactive dashboards and reports
- Geographic visualization of incidents
- Audit logging
- Integration with Android mobile application

---

# 🛠️ Technology Stack

## Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS

## Backend

- Next.js API Routes
- Prisma ORM
- PostgreSQL

## Authentication

- NextAuth

## Cloud Services

- AWS
- Amazon S3

## Data Visualization

- Leaflet
- Recharts

---

# 🏗️ System Architecture

```text
                    Browser
                       │
                       ▼
             Next.js Frontend (React)
                       │
                       ▼
          API Routes / Server Actions
                       │
                       ▼
                  Prisma ORM
                       │
                       ▼
                 PostgreSQL Database
                       ▲
                       │
         Android Mobile Application
```

---

# 📦 Main Modules

## Authentication

Secure user login and role-based authorization.

---

## Disaster Risk Management

Registration, monitoring, and management of disaster incidents.

---

## Volunteer Management

Administration of volunteers and emergency personnel.

---

## Disaster Drills

Planning and monitoring of disaster preparedness activities.

---

## Emergency Kits

Management of humanitarian aid distribution.

---

## Training

Management of training courses and educational material.

---

## Reports

Operational dashboards and statistical reports.

---

## Audit

Traceability of system activities.

---

# 📂 Project Structure

```text
app/
├── dashboard/
├── incidencias/
├── brigadistas/
├── simulacros/
├── cursos/
├── kits/
├── donaciones/
├── reportes/
├── auditoria/
└── usuarios/

components/

prisma/

services/

lib/
```

---

# 📱 Mobile Integration

The web platform integrates with the Caritas GRD Android application.

Field volunteers can collect information using the mobile application while working offline. Once connectivity becomes available, the synchronization service uploads local changes to the central platform, ensuring data consistency between both systems.

---

# 👨‍💻 My Contributions

My main contributions focused on backend development and mobile integration.

They included:

- Supporting the integration between the Android application and backend services.
- Extending the database schema for mobile synchronization.
- Implementing and maintaining backend endpoints consumed by the Android application.
- Contributing to database management using Prisma and PostgreSQL.
- Participating in testing and integration of synchronization workflows.

---

# 🚀 Running the Project

## Clone the repository

```bash
git clone <repository-url>
cd caritas-grd-web
```

## Install dependencies

```bash
npm install
```

## Configure environment variables

Create a `.env` file with the required configuration.

Example:

```env
DATABASE_URL=
NEXTAUTH_SECRET=
NEXTAUTH_URL=
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=
```

---

## Run the development server

```bash
npm run dev
```

The application will be available at:

```
http://localhost:3000
```

---

# 🔮 Future Improvements

- Real-time notifications
- GIS improvements
- Advanced analytics dashboards
- Performance optimization
- Enhanced synchronization monitoring

---

# 👥 Team

Developed by a multidisciplinary team as part of the Software Implementation Project at Pontificia Universidad Católica del Perú (PUCP).

---

# 📄 License

This repository is shared for educational and portfolio purposes.
