# 📊 StudyLens — Study Behavior Analytics

> **Most study apps track time. StudyLens analyzes the behavior behind it.**

StudyLens is a gamified study-tracking application that converts study-session activity into **behavioral metrics, patterns, streaks, and actionable insights**.

Instead of treating study time as a single number, StudyLens analyzes how consistently, frequently, and across which subjects a student studies.

**Core flow:**

```text
Study Sessions
      ↓
Behavioral Metrics
      ↓
Pattern Detection
      ↓
Visual Insights
      ↓
Gamification & Feedback
```

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open%20App-brightgreen)](https://studybehavioranalyticssystem.netlify.app/)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)](https://github.com/prasadk1628/study-buddy-app)

---

# 🎯 Problem

Most study trackers answer one question:

> **"How long did I study?"**

That number alone provides limited insight.

StudyLens attempts to answer more useful behavioral questions:

* Am I studying consistently?
* Which subjects receive most of my study time?
* Which days am I most active?
* Is my study activity increasing over time?
* Am I maintaining a study streak?
* Which behavioral milestones have I achieved?

The goal is to transform raw activity logs into **interpretable behavioral insights**.

---

# 📊 Behavioral Analytics

StudyLens calculates metrics from recorded study sessions.

### Consistency

Measures study consistency over time rather than focusing only on total hours.

### Subject Distribution

Shows how study time is distributed across subjects and identifies dominant study areas.

### Activity Trends

Tracks study activity over time to reveal changes in frequency and session patterns.

### Most Active Day

Identifies the day on which the user records the highest study activity.

### Session Analysis

Analyzes session duration and frequency to identify longer sessions and recurring study behavior.

---

# 🏆 Achievement Engine

StudyLens uses a **rule-based achievement engine** to convert behavioral milestones into rewards.

Achievements can be triggered by conditions such as:

* XP milestones
* study streaks
* session count
* long study sessions
* subject specialization

The achievement system evaluates multiple conditions against the user's current study data and unlocks relevant milestones dynamically.

---

# ⚡ Gamification Layer

The analytics layer is connected to a gamification system designed to make behavioral progress visible.

The system tracks:

* XP
* levels
* streaks
* achievement progress
* milestone completion

This creates a feedback loop:

```text
Study
  ↓
Record Session
  ↓
Analyze Behavior
  ↓
Earn XP / Achievements
  ↓
Visualize Progress
  ↓
Continue Studying
```

---

# 📈 Dashboard Visualizations

StudyLens provides real-time visual feedback through:

### Subject Analysis

Bar charts showing study time distribution across subjects.

### Progress Tracking

Line charts showing study activity progression over time.

### Behavioral Summary

Dashboard metrics highlighting:

* consistency
* session activity
* subject distribution
* streaks
* XP progression

---

# 🐍 Python Analytics Extension

The project also includes an offline Python analytics extension:

```text
analytics_dashboard.py
```

This provides a deeper analysis layer using **Pandas**.

The architecture therefore supports two complementary experiences:

| Layer                 | Purpose                                         |
| --------------------- | ----------------------------------------------- |
| **React Application** | Real-time tracking and behavioral visualization |
| **Python + Pandas**   | Offline deeper analytics                        |

This demonstrates how the same behavioral dataset can be consumed by both a user-facing analytics application and a Python analysis workflow.

---

# ⚙️ How It Works

```text
1. User logs a study session
          ↓
2. Session stored in localStorage
          ↓
3. React calculates behavioral metrics
          ↓
4. Achievement rules are evaluated
          ↓
5. XP / streak / achievement state is updated
          ↓
6. Charts and summaries are rendered
```

The application follows an **offline-first** approach, with session data persisted locally using browser `localStorage`.

---

# 📸 Application Preview

<p align="center">
  <img src="assets/index.jpg" width="300"/>
  <img src="assets/Session.jpg" width="300"/>
</p>
<p align="center"><em> Home Screen &nbsp;&nbsp;|&nbsp;&nbsp;  Session Screen </em></p>

<p align="center">
  <img src="assets/Acheivement.jpg" width="300"/>
  <img src="assets/Goal.jpg" width="300"/>
</p>
<p align="center"><em>Achievement Screen &nbsp;&nbsp;|&nbsp;&nbsp; Goal Screen</em></p>

<p align="center">
  <img src="assets/Setings.jpg" width="300"/>
</p>
<p align="center"><em>Settings Screen</em></p>

---

# 🛠️ Tech Stack

| Layer                   | Technology           |
| ----------------------- | -------------------- |
| **Frontend**            | React                |
| **Language**            | TypeScript           |
| **Visualization**       | Recharts             |
| **State / Logic**       | Custom React Hooks   |
| **Storage**             | Browser localStorage |
| **Styling**             | Tailwind CSS         |
| **Analytics Extension** | Python · Pandas      |
| **Deployment**          | Netlify              |

---

# 📁 Project Structure

```text
src/
├── components/
│   └── UI components
│
├── hooks/
│   └── Session, statistics and achievement logic
│
├── pages/
│   └── Main application views
│
├── utils/
│   └── Helper and analytical functions
│
└── types/
    └── TypeScript type definitions
```

---

# 💡 What This Project Demonstrates

### Behavioral Analytics

Converting raw user activity into meaningful behavioral metrics.

### Data Visualization

Presenting patterns through interactive charts and dashboards.

### Rule-Based Analytics

Building a multi-condition achievement engine that reacts to user behavior.

### Product Thinking

Connecting analytics with a feedback mechanism rather than presenting statistics in isolation.

### Full-Stack Analytics Delivery

Combining a user-facing React application with a Python/Pandas analytics extension.

---

# 🔮 Future Improvements

* Hour-level behavioral analysis using timestamps
* Cloud synchronization using Supabase
* Predictive study-behavior analysis
* Personalized study recommendations
* Multi-user support
* Historical behavioral comparisons

---

# 📄 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Vara Prasad K**

Data Analyst | Python · SQL · Tableau · Streamlit

[GitHub](https://github.com/prasadk1628) · [LinkedIn](https://www.linkedin.com/in/vara-prasad-kavali/)

---

> **Track the activity. Understand the behavior. Improve the system.**
