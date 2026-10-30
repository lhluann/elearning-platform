# 🎓 EduFlow — Enterprise Online Learning & Course Management Platform

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-16.2-black?style=for-the-badge&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Strapi_CMS-Headless-4945FF?style=for-the-badge&logo=strapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-Auth_&_Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Developer-lhluann-58A6FF?style=for-the-badge&logo=github&logoColor=white" />
</p>

<p align="center">
  A production-grade, full-stack Learning Management System (LMS) engineered with Next.js App Router, Strapi Headless CMS, and Firebase, developed by <strong>Lâm Hữu Luân (<a href="https://github.com/lhluann">@lhluann</a>)</strong>.
</p>

---

## 📸 Application Showcase & Screenshots

### 1. Course Discovery Catalog
<p align="center">
  <img src="docs/courses_preview.png" alt="EduFlow Course Discovery" width="95%" />
  <br/>
  <em>Figure 1: Course Catalog — Category taxonomy filters, sorting, instructor badges, ratings, student counts, and pricing tiers.</em>
</p>

### 2. Modern Hero Landing Page
<p align="center">
  <img src="docs/home_preview.png" alt="EduFlow Landing Page" width="95%" />
  <br/>
  <em>Figure 2: Homepage Hero — Modern design system, value proposition, and key learning statistics.</em>
</p>

---

## 🌟 Key Features

### 🎓 Student Experience
- **Modern Course Discovery:** Filter and search courses by category, difficulty level, and rating.
- **Interactive Learning Environment:** Structured lesson playback with video player, lesson transcripts, downloadable resources, and lesson completion checkmarks.
- **Quizzes & Assessments:** Multi-question timed quizzes with instant grading, score review, and retake policies.
- **Certificates of Completion:** Automated certificate generation upon 100% course completion.
- **Gamified Leaderboard:** Points and ranking system based on completed lessons, quiz achievements, and learning streaks.
- **Student Dashboard:** Track enrolled courses, active progress percentages, hours spent, and certificates earned.

### 👨‍🏫 Instructor Workspace
- **Course Studio:** Create, edit, and organize courses with modules, chapters, and rich media lessons.
- **Student Analytics:** Real-time visibility into enrollments, completion rates, and average quiz scores using interactive Recharts.
- **Q&A & Discussion Management:** Answer student questions, moderate comments, and engage with learners.

### 🛡️ Administrator Portal
- **Platform Overview:** High-level metrics on total active users, courses published, revenue trends, and platform engagement.
- **User Governance:** Manage student and instructor accounts, role assignments, and permissions.
- **Course Moderation:** Review submitted courses before public publication.

---

## 🏗️ System Architecture

```text
                               ┌────────────────────────┐
                               │   Next.js App Router   │
                               │   (Frontend & BFF)     │
                               └──────────┬─────────────┘
                                          │
                  ┌───────────────────────┴───────────────────────┐
                  ▼                                               ▼
     ┌────────────────────────┐                      ┌────────────────────────┐
     │   Strapi Headless CMS  │                      │   Firebase Ecosystem   │
     ├────────────────────────┤                      ├────────────────────────┤
     │ • Course Catalog       │                      │ • User Authentication  │
     │ • Curriculum Modules   │                      │ • Progress Data Store  │
     │ • Lessons & Media      │                      │ • Certificate Records  │
     │ • Category Taxonomy    │                      │ • Real-time Sync       │
     └────────────────────────┘                      └────────────────────────┘
