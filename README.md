# INQUISITTORS
An offline-first telehealth platform designed for patients in rural communities with limited internet connectivity (2G/3G networks). The platform enables patients to directly access healthcare services, submit health information, receive medical guidance, and manage prescriptions through asynchronous communication
#Application Overview
# Healify

## Overview
Healify is an **offline-first telehealth platform** designed for patients in rural communities with limited internet connectivity (2G/3G networks). It enables patients, doctors, nurses, pharmacy holders, and guardians to access healthcare services, submit health information, receive medical guidance, and manage prescriptions through **asynchronous communication**, optimized for low-bandwidth environments.

### Key Features
- AI-powered prescription and diagnosis
- Real-time online counseling
- Multi-language accessibility (English + all 22 official Indian languages)
- Voice assistance and screen reader compatibility
- Comprehensive health tracking
- Guardian portal for patient monitoring
- SMS-based communication (zero data requirement)
- Offline medical knowledge library

---

## User Roles & Access
- **Patient**: Consultations, health tracking, prescriptions  
- **Doctor**: Review consultations, issue prescriptions, communicate with patients  
- **Nurse**: Assist consultations, monitor patient records  
- **Pharmacy Holder**: Fulfill prescriptions, manage inventory  
- **Guardian**: Monitor linked patient accounts, receive alerts  

 **Certification Requirement**: Doctors, Nurses, and Pharmacy Holders must upload valid professional certifications. Accounts remain pending until verified.
## Page Structure
- **Onboarding & Authentication**
  - Language selection (supports RTL scripts like Urdu)
  - Role selection
  - Registration (role-specific)
  - Login with role-based redirect
- **Patient Dashboard**
  - Home / Overview
  - AI Counseling (Chat)
  - Consultation Management
  - Health Tracker & Heart Rate Calculator
  - Prescriptions & Pharmacy Services
  - Medical Knowledge Library
  - Guardian Portal
  - Settings
- **Doctor Dashboard**
  - Pending Consultations, Patient Records, Prescription Management
- **Nurse Dashboard**
  - Assigned Patients, Health Records
- **Pharmacy Dashboard**
  - Prescription Queue, Medication Inventory

---

## Core Features
- **Multi-Language Accessibility**: Real-time translation, localized medical terminology, RTL layout support  
- **Voice Assistant**: Text-to-speech, voice commands, audio playback, haptic feedback  
- **AI Counseling (Chat)**: Symptom assessment, triage, diagnosis, prescriptions, mental health support  
- **AI-Powered Prescription System**: Allergy checks, dosage recommendations, alternative suggestions, audit trail  
- **Disease Diagnosis & Management**: Reports, lifestyle recommendations, emergency warnings, progression tracking  
- **Health Tracker**: Vitals logging, charts, medication reminders, PDF export  
- **Consultation Management**: Offline submission, sync on reconnection, follow-ups  
- **Pharmacy Services**: Digital prescriptions, availability checks, refill reminders  
- **SMS Communication**: Encrypted prescriptions, reminders, diet planning, health updates  
- **Medical Knowledge Library**: Offline-accessible, audio versions, searchable interface  
- **Guardian Portal**: Linked patient monitoring, alerts, communication with providers  

---

## Business Rules & Logic
- **Certification Verification**: Role-specific features locked until verified  
- **Offline-First Sync**: Local encrypted storage, auto-sync, conflict resolution  
- **AI Prescription Rules**: Cross-references patient profile, multi-layer validation, safety alerts  
- **Language & RTL Rules**: Instant language change, mirrored UI for RTL scripts  
- **Session Management**: Timeout notifications, secure logout  
- **Guardian Access**: Read-only access, patient approval required  
- **Data Compression**: Images compressed up to 80%, max 500KB per upload  
## Exceptions & Edge Cases
- No internet → Full offline mode with local AI  
- Upload failure → Automatic retry & resume  
- AI unable to generate prescription → Escalation to human provider  
- Language change mid-session → Immediate re-render  
- Guardian not linked → Patient approval required  
- Abnormal health metrics → Alerts + audio warnings  
- SMS delivery failure → In-app notification fallback  

---

## Acceptance Criteria
- Language selection on first launch  
- Voice assistant reads all content accurately  
- Certification upload required for Doctors/Nurses/Pharmacy Holders  
- Offline consultation submission with sync  
- AI generates validated prescriptions with alternatives  
- Heart rate calculator with history tracking  
- Health tracker with charts and PDF export  
- Guardian portal with linked patient records  
- Prescriptions delivered via encrypted SMS  
- Dark mode + high contrast mode support  
- Image compression and incremental upload  

---

## Out of Scope (This Release)
- Video/audio call consultations  
- External EHR integration  
- Insurance claim processing  
- Wearable device integration  
- Admin panel for certification verification  
- In-app payments/e-commerce  
- Push notifications beyond SMS  
- Multi-patient management under one doctor  
- Calendar integration with external apps  
