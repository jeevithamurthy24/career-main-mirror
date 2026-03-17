<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=39FF14&height=120&section=header&text=AI%20Career%20Mentor&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Your%20AI-Powered%20Career%20Co-Pilot&descAlignY=60&descColor=39FF14" width="100%"/>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=39FF14&background=0A0A0A00&center=true&vCenter=true&width=600&lines=Know+your+gaps.;Fix+your+resume.;Build+your+future.)](https://git.io/typing-svg)

<br/>

![](https://img.shields.io/badge/Groq-LPU%20Inference-FF6B35?style=for-the-badge&labelColor=0A0A0A)
![](https://img.shields.io/badge/Llama%203.3-70B%20Parameters-39FF14?style=for-the-badge&labelColor=0A0A0A)
![](https://img.shields.io/badge/Firebase-Auth%20%2B%20Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=FFCA28&labelColor=0A0A0A)
![](https://img.shields.io/badge/Vanilla-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=F7DF1E&labelColor=0A0A0A)
![](https://img.shields.io/badge/License-MIT-white?style=for-the-badge&labelColor=0A0A0A)

<br/>

> **Built by a Engineering students, for every fresher who ever sent 100 applications and heard nothing back.**

</div>

---

## 🧩 The Problem

Every year, **1.5 million engineering graduates** in India enter the job market.

Most of them apply to dozens of jobs. Most of them get rejected — not because they're unqualified, but because:

- ❌ They don't know **which specific skills** their target role actually needs
- ❌ Their resume gets **filtered out by ATS software** before any human reads it
- ❌ They get **generic advice** — not guidance built around their actual background

No tool told them: *"You have Python. You want cybersecurity. You're missing network security, cryptography, and threat analysis — and here's how to close that in 6 months."*

**AI Career Mentor does exactly that.**

---

## 💡 What It Does

In **under 10 seconds**, AI Career Mentor:

1. **Analyzes your profile** — your skills, target role, education, and experience
2. **Gives you a match score** — an exact percentage showing how ready you are
3. **Lists your critical gaps** — ranked by how much they matter for your role
4. **Scores your resume** — simulates how ATS hiring software rates it
5. **Builds your roadmap** — a personalized 6-month learning plan

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎯 Skill Gap Analyzer
Enter your skills + target role → get an exact match score and a ranked list of what you're missing, specific to your background.

### 📄 ATS Resume Scorer
Upload your resume (PDF/TXT/DOC) → get an ATS compatibility score + actionable fix list. Because **75% of resumes never reach a human.**

### 🔁 What-If Simulator
Thinking of learning Python? SQL? See your match score change **in real-time** before committing to a learning path.

### 🗺️ 6-Month Learning Roadmap
Not just "learn this skill" — a week-by-week personalized plan built around your actual gaps and timeline.

</td>
<td width="50%">

### 🤖 AI Chat Mentor
Ask anything. Career questions, resume feedback, interview prep — powered by Llama 3.3 70B, free, always on.

### 🔥 Brutal Honesty Mode
Toggle on raw, unfiltered AI feedback. No fluff, no encouragement — just exactly what's wrong and how to fix it.

### 📈 Live Skill Market Ticker
See which skills are trending in real job postings right now — so you know what to learn before recruiters start asking.

### 🕐 Analysis History Dashboard
Every analysis you've ever run — tracked, saved, and comparable. Watch your score grow over time.

</td>
</tr>
</table>

---

## 🏗️ Architecture
```
┌─────────────────────────────────────────────────────────┐
│                     USER BROWSER                        │
│          HTML5 · CSS3 · Vanilla JavaScript              │
│         Canvas Animations · Responsive Design           │
└───────────────────────┬─────────────────────────────────┘
                        │  API calls (fetch)
                        ▼
┌─────────────────────────────────────────────────────────┐
│                    GROQ API                             │
│             Meta Llama 3.3 70B (70B params)            │
│                                                         │
│  • Skill Gap Analysis      • ATS Resume Scoring        │
│  • What-If Re-Scoring      • Roadmap Generation        │
│  • Conversational Chat     • Job Role Matching         │
└───────────────────────┬─────────────────────────────────┘
                        │  save / read
                        ▼
┌─────────────────────────────────────────────────────────┐
│                   FIREBASE                              │
│                                                         │
│  Authentication (Google OAuth)                          │
│  Firestore Database (analyses, profiles, history)       │
│  Hosting (global CDN deployment)                        │
└─────────────────────────────────────────────────────────┘
```

### How data flows
```
You enter your skills + target role
           ↓
Prompt Engineering Layer
(adds your education, experience, role context
 so AI reasons about YOU — not a generic student)
           ↓
Groq → Llama 3.3 70B
(70 billion parameters reasoning about
 your specific situation in ~2 seconds)
           ↓
Structured response: score + gaps + summary
           ↓
Saved to Firestore under your account
           ↓
Displayed on your dashboard
```

> **The What-If Simulator** re-runs this entire flow with a hypothetical skill added. That's why Groq's speed is critical — each simulation is a full AI inference call.

---

## 🛠️ Tech Stack — What, Why & What It Does

| Technology | What It Is | What It Does In This App | Why We Chose It |
|-----------|-----------|--------------------------|----------------|
| **HTML5 + CSS3** | Web structure & styling language | Builds every screen, card, form, and layout. Dark theme + neon green UI | Zero framework overhead. Full control. Fast on slow internet |
| **Vanilla JavaScript** | Programming language of the web, no framework | Handles all logic — API calls, routing, skill tags, real-time updates | No build tools needed. Faster load. Stronger fundamentals than hiding behind React |
| **Canvas API** | Browser's built-in graphics engine | Powers the custom glowing cursor and background particle ripple animations | Makes the first impression unforgettable. Shows UI craftsmanship |
| **CSS Grid & Flexbox** | Modern CSS layout systems | Dashboard card grid, navbar alignment, responsive mobile layout | Industry standard. No layout library needed |
| **Groq API** | LLM inference infrastructure (custom LPU hardware) | Routes every AI request — analysis, scoring, chat, roadmap | **10–100× faster** than OpenAI. The What-If Simulator needs near-instant responses |
| **Meta Llama 3.3 70B** | Open-source AI model with 70 billion parameters | The brain — understands your skills, reasons about gaps, generates roadmaps | Near GPT-4 quality. Free on Groq. 70B = nuanced reasoning, not shallow keyword matching |
| **Firebase Auth** | Google's authentication service | Manages all user accounts, sessions, and login state | Enterprise-grade security with zero backend code |
| **Google OAuth 2.0** | Secure login protocol | One-click "Sign in with Google" — no new passwords | Every student has Gmail. Removes the #1 drop-off point |
| **Firebase Firestore** | NoSQL cloud database | Stores every analysis, profile, gap list, score, and history entry | Serverless. Real-time. Free tier. Scales automatically |

---

## 📊 Why This Beats Every Existing Tool

| What you actually need | LinkedIn | Coursera | Naukri | **AI Career Mentor** |
|------------------------|:-------:|:-------:|:------:|:-------------------:|
| Your exact skill gap for a specific role | ❌ | ❌ | ❌ | ✅ |
| ATS resume score for that role | ❌ | ❌ | ⚠️ Generic | ✅ |
| Personalized 6-month learning roadmap | ❌ | ⚠️ Generic paths | ❌ | ✅ |
| What-If skill simulator | ❌ | ❌ | ❌ | ✅ |
| Free AI career coaching | ⚠️ Paid | ❌ | ❌ | ✅ |
| Analysis history & score tracking | ❌ | ⚠️ Courses only | ❌ | ✅ |
| Built specifically for Indian BE/BTech freshers | ❌ | ❌ | ⚠️ Job listings only | ✅ |

**LinkedIn** shows you jobs. **Coursera** shows you courses. **Naukri** shows you listings.
None of them tell you the exact gap between *you* and *that role*, right now, with your specific background.

**We do.**

---

## 🚀 Getting Started

### What you need
- Any modern browser — Chrome recommended
- A [Groq API key](https://console.groq.com) — free to create
- A [Firebase project](https://console.firebase.google.com) — free Spark plan

### Step 1 — Clone the repo
```bash
git clone https://github.com/jeevithamurthy24/ai-career-mentor.git
cd ai-career-mentor
```

### Step 2 — Set up Firebase

1. Go to [Firebase Console](https://console.firebase.google.com) → **Add project**
2. **Authentication** → Sign-in method → Enable **Google**
3. **Firestore Database** → Create database → **Test mode**
4. **Project Settings** → Your apps → Web `</>` → Copy your config object

### Step 3 — Add your API keys

Create a file called `config.js` in the root folder:
```javascript
// config.js — DO NOT commit this file to GitHub
const firebaseConfig = {
  apiKey: "YOUR_FIREBASE_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const GROQ_API_KEY = "YOUR_GROQ_API_KEY";
```

Then add to `.gitignore`:
```
config.js
```

> ⚠️ Never push your API keys to GitHub. For production, move the Groq key to a Firebase Cloud Function.

### Step 4 — Run it

No npm install. No build step. Just:
```bash
# Open directly in browser
open index.html

# Or use a local server (recommended)
npx serve .
# visit http://localhost:3000
```

### Step 5 — Deploy (optional)
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

---

## 📁 Project Structure
```
ai-career-mentor/
│
├── index.html          ← Landing page + login
├── profile.html        ← Build your profile (Step 1)
├── analysis.html       ← Skill gap results + score
├── resume.html         ← ATS resume scorer
├── chat.html           ← AI chat mentor
├── dashboard.html      ← All your past analyses
├── roadmap.html        ← Your 6-month plan
│
├── css/
│   ├── main.css        ← Dark theme, CSS variables, global styles
│   ├── components.css  ← Cards, buttons, skill tags, forms
│   └── animations.css  ← Canvas ripple, cursor glow, transitions
│
├── js/
│   ├── auth.js         ← Firebase login / logout
│   ├── firestore.js    ← Save and read from database
│   ├── groq.js         ← All Groq API calls + prompt templates
│   ├── analyzer.js     ← Skill gap analysis logic
│   ├── ats.js          ← ATS resume scoring logic
│   ├── simulator.js    ← What-If simulator
│   ├── roadmap.js      ← Roadmap generation
│   └── canvas.js       ← Cursor + particle animations
│
├── config.js           ← 🔒 API keys — NEVER commit this
├── .gitignore
└── README.md
```

---

## 🔌 Code Samples

### Calling Groq for skill gap analysis
```javascript
const response = await fetch("https://api.groq.com/openai/v1/chat/completions", {
  method: "POST",
  headers: {
    "Authorization": `Bearer ${GROQ_API_KEY}`,
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    model: "llama-3.3-70b-versatile",
    messages: [
      {
        role: "system",
        content: "You are an expert career analyst specializing in tech roles..."
      },
      {
        role: "user",
        content: `Analyze skill gap for:
          Skills: ${skills}
          Target Role: ${role}
          Education: ${education}
          Experience: ${experience}`
      }
    ],
    temperature: 0.3,
    max_tokens: 1000
  })
});
```

### Saving an analysis to Firestore
```javascript
import { collection, addDoc, serverTimestamp } from "firebase/firestore";

await addDoc(collection(db, "analyses"), {
  userId: auth.currentUser.uid,
  targetRole: role,
  skills: skills,
  matchScore: score,
  criticalGaps: gaps,
  summary: summary,
  createdAt: serverTimestamp()
});
```

---

## 🗺️ Roadmap

**v1.0 — Live ✅**
- [x] Profile builder with smart skill tags
- [x] AI skill gap analyzer (Llama 3.3 70B)
- [x] ATS resume scorer
- [x] What-If skill simulator
- [x] 6-month personalized roadmap
- [x] AI chat mentor
- [x] Brutal Honesty Mode
- [x] Live skill market ticker
- [x] Analysis history dashboard

**v2.0 — Coming Soon**
- [ ] Job board integration (LinkedIn, Naukri)
- [ ] Mock interview simulator
- [ ] Peer score benchmarking
- [ ] Company-specific prep packs

**v3.0 — Vision**
- [ ] Mobile app (React Native)
- [ ] Recruiter-side talent analytics
- [ ] Regional language support

---

## 👩‍💻 About the Developer

Built by **Jeevitha Murthy** **Gangothri C L** **Rahul Nittur B P** - Engineering students

This isn't a class assignment. It's a tool I built because I needed it. I was targeting cybersecurity roles, I had Python, and I had no idea what I was missing. No tool gave me a straight answer. So I built one.

Every single feature in this app solves a real problem I personally faced.

[![GitHub](https://img.shields.io/badge/GitHub-jeevithamurthy24-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/jeevithamurthy24)

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=39FF14&height=80&section=footer" width="100%"/>

**⭐ Star this repo if it helped you — it takes 2 seconds and means everything.**

*Know your gaps. Fix your resume. Build your future.*

![](https://img.shields.io/badge/Built%20with-Groq%20%2B%20Llama%203.3%2070B%20%2B%20Firebase-39FF14?style=flat-square&labelColor=0A0A0A)

</div>
