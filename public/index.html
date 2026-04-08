
import { useState, useEffect, useRef } from "react";

// ─── ICONS ────────────────────────────────────────────────────────────────────
const Icon = ({ d, size = 20, color = "currentColor", fill = "none", strokeWidth = 1.8 }) => (
  <svg width={size} height={size} viewBox="0 0 24 24" fill={fill} stroke={color} strokeWidth={strokeWidth} strokeLinecap="round" strokeLinejoin="round">
    {Array.isArray(d) ? d.map((path, i) => <path key={i} d={path} />) : <path d={d} />}
  </svg>
);

const Icons = {
  home: "M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z",
  growth: "M13 2L3 14h9l-1 8 10-12h-9l1-8z",
  thinking: "M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 1 1 7.072 0l-.548.547A3.374 3.374 0 0 0 14 18.469V19a2 2 0 1 1-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z",
  reflection: "M12 2a10 10 0 1 0 10 10A10 10 0 0 0 12 2zm0 3a3 3 0 1 1-3 3 3 3 0 0 1 3-3zm0 14.2a7.2 7.2 0 0 1-6-3.22c.03-1.99 4-3.08 6-3.08 1.99 0 5.97 1.09 6 3.08a7.2 7.2 0 0 1-6 3.22z",
  vision: "M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z M12 9a3 3 0 1 0 0 6 3 3 0 0 0 0-6z",
  menu: ["M3 12h18", "M3 6h18", "M3 18h18"],
  plus: "M12 5v14M5 12h14",
  bot: "M12 2a2 2 0 0 1 2 2v1h3a1 1 0 0 1 1 1v4a1 1 0 0 1-1 1h-1v2l-3-2H9l-3 2v-2H5a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h3V4a2 2 0 0 1 2-2z",
  close: "M18 6L6 18M6 6l12 12",
  send: "M22 2L11 13M22 2l-7 20-4-9-9-4 20-7z",
  fire: "M8.5 14.5A2.5 2.5 0 0 0 11 12c0-1.38-.5-2-1-3-1.072-2.143-.224-4.054 2-6 .5 2.5 2 4.9 4 6.5 2 1.6 3 3.5 3 5.5a7 7 0 1 1-14 0c0-1.153.433-2.294 1-3a2.5 2.5 0 0 0 2.5 2.5z",
  check: "M20 6L9 17l-5-5",
  target: "M12 22a10 10 0 1 0 0-20 10 10 0 0 0 0 20z M12 18a6 6 0 1 0 0-12 6 6 0 0 0 0 12z M12 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4z",
  brain: "M9.5 2A2.5 2.5 0 0 1 12 4.5v15a2.5 2.5 0 0 1-4.96-.44 2.5 2.5 0 0 1-2.96-3.08 3 3 0 0 1-.34-5.58 2.5 2.5 0 0 1 1.32-4.24 2.5 2.5 0 0 1 1.98-3A2.5 2.5 0 0 1 9.5 2z M14.5 2A2.5 2.5 0 0 0 12 4.5v15a2.5 2.5 0 0 0 4.96-.44 2.5 2.5 0 0 0 2.96-3.08 3 3 0 0 0 .34-5.58 2.5 2.5 0 0 0-1.32-4.24 2.5 2.5 0 0 0-1.98-3A2.5 2.5 0 0 0 14.5 2z",
  journal: "M4 19.5A2.5 2.5 0 0 1 6.5 17H20 M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z",
  star: "M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z",
  chart: "M18 20V10 M12 20V4 M6 20v-6",
  idea: "M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 1 1 7.072 0l-.548.547A3.374 3.374 0 0 0 14 18.469V19a2 2 0 1 1-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z",
  problem: "M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z M12 9v4 M12 17h.01",
  fear: "M8 14s1.5 2 4 2 4-2 4-2 M9 9h.01 M15 9h.01 M12 2a10 10 0 1 0 0 20 10 10 0 0 0 0-20z",
  experiment: "M9 3H5a2 2 0 0 0-2 2v4m6-6h10a2 2 0 0 1 2 2v4M9 3v11l4 2 4-2V3 M3 9l4 2 M21 9l-4 2",
  skill: "M18 20V10 M12 20V4 M6 20v-6",
  book: "M4 19.5A2.5 2.5 0 0 1 6.5 17H20 M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z",
  money: "M12 1v22 M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6",
  clock: "M12 22a10 10 0 1 0 0-20 10 10 0 0 0 0 20z M12 6v6l4 2",
  bell: "M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9 M13.73 21a2 2 0 0 1-3.46 0",
  eye: "M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z M12 9a3 3 0 1 0 0 6 3 3 0 0 0 0-6z",
  compass: "M12 22a10 10 0 1 0 0-20 10 10 0 0 0 0 20z M16.24 7.76l-2.12 6.36-6.36 2.12 2.12-6.36 6.36-2.12z",
  zap: "M13 2L3 14h9l-1 8 10-12h-9l1-8z",
  user: "M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2 M12 11a4 4 0 1 0 0-8 4 4 0 0 0 0 8z",
  settings: "M12 15a3 3 0 1 0 0-6 3 3 0 0 0 0 6z M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1-2.83 2.83l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-4 0v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83-2.83l.06-.06A1.65 1.65 0 0 0 4.68 15a1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1 0-4h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 2.83-2.83l.06.06A1.65 1.65 0 0 0 9 4.68a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 4 0v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 2.83l-.06.06A1.65 1.65 0 0 0 19.4 9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 0 4h-.09a1.65 1.65 0 0 0-1.51 1z",
  trophy: "M8 21h8 M12 17v4 M7 4H4a1 1 0 0 0-1 1v3c0 3.31 2.69 6 6 6h6c3.31 0 6-2.69 6-6V5a1 1 0 0 0-1-1h-3 M7 4h10v7a5 5 0 0 1-5 5 5 5 0 0 1-5-5V4z",
  arrow: "M5 12h14 M12 5l7 7-7 7",
  pin: "M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z M12 7a3 3 0 1 0 0 6 3 3 0 0 0 0-6z",
  tag: "M20.59 13.41l-7.17 7.17a2 2 0 0 1-2.83 0L2 12V2h10l8.59 8.59a2 2 0 0 1 0 2.82z M7 7h.01",
  heart: "M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z",
  search: "M11 17.25a6.25 6.25 0 1 1 0-12.5 6.25 6.25 0 0 1 0 12.5z M16 16l4.5 4.5",
};

// ─── DATA ─────────────────────────────────────────────────────────────────────
const initialData = {
  habits: [
    { id: 1, name: "Morning Meditation", streak: 14, done: false, icon: "🧘", category: "Mind" },
    { id: 2, name: "Cold Shower", streak: 7, done: true, icon: "🚿", category: "Body" },
    { id: 3, name: "Read 30 min", streak: 21, done: false, icon: "📖", category: "Knowledge" },
    { id: 4, name: "Exercise", streak: 5, done: true, icon: "💪", category: "Body" },
    { id: 5, name: "No Social Media AM", streak: 3, done: false, icon: "🔕", category: "Focus" },
  ],
  goals: [
    { id: 1, title: "Launch SaaS Product", deadline: "2025-12", progress: 35, type: "long", area: "Career" },
    { id: 2, title: "Read 24 books this year", deadline: "2025-12", progress: 62, type: "long", area: "Knowledge" },
    { id: 3, title: "Save $10,000", deadline: "2025-06", progress: 48, type: "short", area: "Money" },
    { id: 4, title: "Lose 10 lbs", deadline: "2025-04", progress: 80, type: "short", area: "Health" },
  ],
  ideas: [
    { id: 1, title: "AI-powered meal planner for gyms", tags: ["AI", "Health", "B2B"], date: "2025-01-10", status: "exploring" },
    { id: 2, title: "Micro-SaaS for freelancer invoicing", tags: ["SaaS", "Finance"], date: "2025-01-08", status: "validating" },
    { id: 3, title: "Newsletter about mental models", tags: ["Content", "Knowledge"], date: "2025-01-05", status: "idea" },
  ],
  problems: [
    { id: 1, industry: "Healthcare", problem: "Patients forget medications — no smart reminders", opportunity: "Smart pill box with ML predictions", date: "2025-01-09" },
    { id: 2, industry: "Education", problem: "Students can't find quality tutors quickly", opportunity: "Uber for tutors — instant booking", date: "2025-01-07" },
  ],
  experiments: [
    { id: 1, title: "Wake up at 5AM for 7 days", duration: 7, day: 4, status: "active", hypothesis: "Early rising will double productive hours" },
    { id: 2, title: "No caffeine for 14 days", duration: 14, day: 14, status: "complete", result: "Sleep improved significantly, energy more stable" },
  ],
  skills: [
    { id: 1, name: "Python Programming", level: 65, category: "Tech", hoursLogged: 120 },
    { id: 2, name: "Public Speaking", level: 40, category: "Communication", hoursLogged: 45 },
    { id: 3, name: "Sales & Negotiation", level: 55, category: "Business", hoursLogged: 80 },
    { id: 4, name: "Financial Modeling", level: 30, category: "Finance", hoursLogged: 25 },
  ],
  journal: [
    { id: 1, date: "2025-01-10", mood: 8, entry: "Had a breakthrough on the product roadmap today. Started with meditation and the ideas just flowed.", tags: ["productivity", "clarity"] },
    { id: 2, date: "2025-01-09", mood: 6, entry: "Felt distracted. Need to redesign my environment. Social media crept in during deep work hours.", tags: ["focus", "lessons"] },
  ],
  fears: [
    { id: 1, fear: "Public speaking to 100+ people", facing: false, plan: "Join a Toastmasters club" },
    { id: 2, fear: "Launching something publicly and failing", facing: true, plan: "Build in public on Twitter" },
    { id: 3, fear: "Cold outreach to CEOs", facing: false, plan: "Send 1 cold email per day for 30 days" },
  ],
  notes: [
    { id: 1, title: "Mental Models Worth Knowing", content: "First principles, Inversion, Second-order thinking, Map is not the territory...", tags: ["thinking", "models"], pinned: true, date: "2025-01-10" },
    { id: 2, title: "Book Notes: Atomic Habits", content: "Identity-based habits. 1% better every day. Systems > Goals. Environment design.", tags: ["habits", "books"], pinned: false, date: "2025-01-08" },
  ],
  lifeAreas: [
    { area: "Health", score: 7.2, color: "#10b981" },
    { area: "Career", score: 8.1, color: "#3b82f6" },
    { area: "Money", score: 5.8, color: "#f59e0b" },
    { area: "Relationships", score: 6.5, color: "#ec4899" },
    { area: "Knowledge", score: 8.8, color: "#8b5cf6" },
    { area: "Mindset", score: 7.5, color: "#06b6d4" },
  ],
  money: { income: 5800, savings: 12400, investments: 8200, business: 1200 },
  decisions: [
    { id: 1, decision: "Quit agency job to go freelance", date: "2024-10-01", outcome: "Income dropped 30% first month but tripled by month 4", rating: 9 },
    { id: 2, decision: "Invest in online course creation tools", date: "2024-11-15", outcome: "Still pending — course launch in Feb", rating: null },
  ],
  opportunities: [
    { id: 1, title: "Partner with local gym for app pilot", source: "Networking event", status: "pursuing", potential: "High" },
    { id: 2, title: "Guest post on ProductHunt blog", source: "Cold outreach", status: "pending", potential: "Medium" },
  ],
  challenges: [
    { id: 1, title: "7-Day Digital Detox", days: 7, completed: 7, status: "done" },
    { id: 2, title: "30-Day Writing Challenge", days: 30, completed: 12, status: "active" },
    { id: 3, title: "21-Day No Complaining", days: 21, completed: 3, status: "active" },
  ],
  comfortBreakers: [
    { id: 1, action: "Talk to a stranger today", done: false },
    { id: 2, action: "Share your work publicly", done: true },
    { id: 3, action: "Ask for feedback from a mentor", done: false },
  ],
  books: [
    { id: 1, title: "Zero to One", author: "Peter Thiel", progress: 100, notes: "Monopolies > competition. Create new markets." },
    { id: 2, title: "The Almanack of Naval Ravikant", author: "Eric Jorgenson", progress: 75, notes: "Wealth = assets working for you." },
    { id: 3, title: "Deep Work", author: "Cal Newport", progress: 40, notes: "Distraction is the enemy of mastery." },
  ],
};

// ─── STYLES ───────────────────────────────────────────────────────────────────
const styles = `
  @import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=DM+Sans:wght@300;400;500;600&display=swap');

  * { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #080c14;
    --surface: #0d1420;
    --surface2: #111827;
    --surface3: #1a2234;
    --border: rgba(255,255,255,0.07);
    --border2: rgba(255,255,255,0.12);
    --accent: #4f6ef7;
    --accent2: #7c3aed;
    --accent3: #06b6d4;
    --gold: #f59e0b;
    --green: #10b981;
    --red: #ef4444;
    --pink: #ec4899;
    --text: #e2e8f0;
    --text2: #94a3b8;
    --text3: #64748b;
    --radius: 16px;
    --radius-sm: 10px;
    --font-display: 'Syne', sans-serif;
    --font-body: 'DM Sans', sans-serif;
  }

  body { background: var(--bg); color: var(--text); font-family: var(--font-body); }

  .app {
    max-width: 430px;
    margin: 0 auto;
    min-height: 100vh;
    background: var(--bg);
    position: relative;
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }

  .scroll-area {
    flex: 1;
    overflow-y: auto;
    padding: 0 16px 100px;
    scrollbar-width: none;
  }
  .scroll-area::-webkit-scrollbar { display: none; }

  .topbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 16px 20px 12px;
    position: sticky;
    top: 0;
    z-index: 50;
    background: linear-gradient(to bottom, var(--bg) 80%, transparent);
  }

  .topbar-title {
    font-family: var(--font-display);
    font-size: 18px;
    font-weight: 700;
    letter-spacing: -0.5px;
    color: var(--text);
  }
  .topbar-title span { color: var(--accent); }

  .icon-btn {
    width: 38px; height: 38px;
    display: flex; align-items: center; justify-content: center;
    border-radius: 10px;
    background: var(--surface2);
    border: 1px solid var(--border);
    cursor: pointer;
    color: var(--text2);
    transition: all 0.2s;
  }
  .icon-btn:hover { background: var(--surface3); color: var(--text); }

  /* Bottom Nav */
  .bottom-nav {
    position: fixed;
    bottom: 0; left: 50%; transform: translateX(-50%);
    width: 100%; max-width: 430px;
    display: flex;
    background: rgba(13,20,32,0.95);
    backdrop-filter: blur(20px);
    border-top: 1px solid var(--border);
    padding: 8px 0 20px;
    z-index: 100;
  }

  .nav-item {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 4px;
    cursor: pointer;
    padding: 4px 0;
    color: var(--text3);
    transition: all 0.2s;
  }
  .nav-item.active { color: var(--accent); }
  .nav-item span {
    font-size: 10px;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    font-family: var(--font-display);
  }

  /* Sidebar */
  .sidebar-overlay {
    position: fixed; inset: 0;
    background: rgba(0,0,0,0.6);
    z-index: 200;
    backdrop-filter: blur(4px);
    animation: fadeIn 0.2s ease;
  }

  .sidebar {
    position: fixed;
    top: 0; left: 0; bottom: 0;
    width: 280px;
    background: var(--surface);
    border-right: 1px solid var(--border2);
    z-index: 201;
    overflow-y: auto;
    padding: 0 0 40px;
    animation: slideInLeft 0.25s ease;
  }

  .sidebar-header {
    padding: 50px 20px 20px;
    border-bottom: 1px solid var(--border);
  }

  .sidebar-logo {
    font-family: var(--font-display);
    font-size: 22px;
    font-weight: 800;
    letter-spacing: -1px;
  }
  .sidebar-logo .os { color: var(--accent); }

  .sidebar-tagline {
    font-size: 12px;
    color: var(--text3);
    margin-top: 4px;
    font-style: italic;
  }

  .sidebar-section {
    padding: 16px 12px 8px;
  }
  .sidebar-label {
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 1.5px;
    color: var(--text3);
    text-transform: uppercase;
    padding: 0 8px;
    margin-bottom: 6px;
    font-family: var(--font-display);
  }

  .sidebar-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 12px;
    border-radius: 10px;
    cursor: pointer;
    color: var(--text2);
    font-size: 14px;
    font-weight: 500;
    transition: all 0.15s;
  }
  .sidebar-item:hover { background: var(--surface2); color: var(--text); }
  .sidebar-item .icon-wrap {
    width: 32px; height: 32px;
    border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0;
  }

  /* Cards */
  .card {
    background: var(--surface2);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 16px;
    margin-bottom: 12px;
  }
  .card-accent {
    border-color: rgba(79,110,247,0.3);
    background: linear-gradient(135deg, rgba(79,110,247,0.08), var(--surface2));
  }

  .card-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 14px;
  }

  .card-title {
    font-family: var(--font-display);
    font-size: 14px;
    font-weight: 700;
    letter-spacing: -0.3px;
    color: var(--text);
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    padding: 2px 8px;
    border-radius: 20px;
    font-size: 11px;
    font-weight: 600;
    font-family: var(--font-display);
  }
  .badge-blue { background: rgba(79,110,247,0.15); color: #7fa7ff; }
  .badge-green { background: rgba(16,185,129,0.15); color: #34d399; }
  .badge-gold { background: rgba(245,158,11,0.15); color: #fcd34d; }
  .badge-red { background: rgba(239,68,68,0.15); color: #fca5a5; }
  .badge-purple { background: rgba(124,58,237,0.15); color: #a78bfa; }
  .badge-cyan { background: rgba(6,182,212,0.15); color: #67e8f9; }

  /* Progress */
  .progress-bar {
    height: 4px;
    background: var(--surface3);
    border-radius: 4px;
    overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    border-radius: 4px;
    transition: width 0.5s ease;
  }

  /* Habit item */
  .habit-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 12px;
    border-radius: 10px;
    background: var(--surface3);
    margin-bottom: 8px;
    cursor: pointer;
    transition: all 0.2s;
  }
  .habit-item:hover { background: rgba(255,255,255,0.07); }
  .habit-check {
    width: 24px; height: 24px;
    border-radius: 8px;
    border: 2px solid var(--border2);
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0;
    transition: all 0.2s;
  }
  .habit-check.done {
    background: var(--accent);
    border-color: var(--accent);
  }

  /* Timer */
  .timer-ring {
    width: 140px; height: 140px;
    margin: 16px auto;
    position: relative;
    display: flex; align-items: center; justify-content: center;
  }
  .timer-svg { transform: rotate(-90deg); }
  .timer-text {
    position: absolute;
    text-align: center;
  }
  .timer-number {
    font-family: var(--font-display);
    font-size: 28px;
    font-weight: 800;
    letter-spacing: -1px;
  }
  .timer-label { font-size: 11px; color: var(--text3); }

  /* Floating buttons */
  .fab-container {
    position: fixed;
    bottom: 90px;
    right: calc(50% - 215px + 16px);
    display: flex;
    flex-direction: column-reverse;
    align-items: flex-end;
    gap: 10px;
    z-index: 90;
  }

  .fab {
    width: 52px; height: 52px;
    border-radius: 16px;
    display: flex; align-items: center; justify-content: center;
    cursor: pointer;
    box-shadow: 0 8px 32px rgba(0,0,0,0.4);
    transition: all 0.2s;
    border: none;
  }
  .fab:hover { transform: scale(1.05); }
  .fab-main {
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    color: white;
  }
  .fab-ai {
    background: linear-gradient(135deg, #06b6d4, #3b82f6);
    color: white;
  }

  .fab-menu {
    position: absolute;
    bottom: 64px;
    right: 0;
    background: var(--surface);
    border: 1px solid var(--border2);
    border-radius: var(--radius);
    padding: 8px;
    min-width: 200px;
    animation: scaleIn 0.15s ease;
    box-shadow: 0 20px 60px rgba(0,0,0,0.5);
  }

  .fab-option {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 10px 12px;
    border-radius: 10px;
    cursor: pointer;
    font-size: 14px;
    font-weight: 500;
    color: var(--text2);
    transition: all 0.15s;
  }
  .fab-option:hover { background: var(--surface2); color: var(--text); }

  /* AI Chat */
  .chat-overlay {
    position: fixed; inset: 0;
    background: rgba(0,0,0,0.7);
    z-index: 300;
    display: flex;
    align-items: flex-end;
    animation: fadeIn 0.2s ease;
  }

  .chat-panel {
    width: 100%;
    max-width: 430px;
    margin: 0 auto;
    height: 80vh;
    background: var(--surface);
    border-radius: 24px 24px 0 0;
    border-top: 1px solid var(--border2);
    display: flex;
    flex-direction: column;
    animation: slideUp 0.3s ease;
  }

  .chat-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 16px 20px;
    border-bottom: 1px solid var(--border);
  }

  .chat-ai-info {
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .ai-avatar {
    width: 36px; height: 36px;
    border-radius: 12px;
    background: linear-gradient(135deg, #06b6d4, #3b82f6);
    display: flex; align-items: center; justify-content: center;
    font-size: 18px;
  }

  .ai-name {
    font-family: var(--font-display);
    font-size: 15px;
    font-weight: 700;
  }
  .ai-status { font-size: 11px; color: var(--green); display: flex; align-items: center; gap: 4px; }
  .ai-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--green); }

  .chat-messages {
    flex: 1;
    overflow-y: auto;
    padding: 16px;
    display: flex;
    flex-direction: column;
    gap: 12px;
    scrollbar-width: none;
  }

  .msg {
    max-width: 85%;
    padding: 12px 14px;
    border-radius: 14px;
    font-size: 14px;
    line-height: 1.5;
    animation: fadeIn 0.2s ease;
  }
  .msg-ai {
    align-self: flex-start;
    background: var(--surface2);
    border: 1px solid var(--border);
    border-bottom-left-radius: 4px;
    color: var(--text);
  }
  .msg-user {
    align-self: flex-end;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    border-bottom-right-radius: 4px;
    color: white;
  }

  .chat-input-row {
    display: flex;
    gap: 10px;
    padding: 12px 16px 24px;
    border-top: 1px solid var(--border);
  }
  .chat-input {
    flex: 1;
    background: var(--surface2);
    border: 1px solid var(--border2);
    border-radius: 12px;
    padding: 10px 14px;
    color: var(--text);
    font-family: var(--font-body);
    font-size: 14px;
    outline: none;
  }
  .chat-input::placeholder { color: var(--text3); }
  .send-btn {
    width: 42px; height: 42px;
    border-radius: 12px;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    border: none;
    cursor: pointer;
    display: flex; align-items: center; justify-content: center;
    color: white;
    flex-shrink: 0;
    transition: all 0.2s;
  }
  .send-btn:hover { transform: scale(1.05); }

  /* Section headers */
  .section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 20px 0 12px;
  }
  .section-title {
    font-family: var(--font-display);
    font-size: 16px;
    font-weight: 700;
    letter-spacing: -0.5px;
    color: var(--text);
  }
  .section-action {
    font-size: 12px;
    color: var(--accent);
    cursor: pointer;
    font-weight: 600;
  }

  /* Stat cards */
  .stats-row {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
    margin-bottom: 12px;
  }
  .stat-card {
    background: var(--surface2);
    border: 1px solid var(--border);
    border-radius: var(--radius-sm);
    padding: 14px;
  }
  .stat-value {
    font-family: var(--font-display);
    font-size: 24px;
    font-weight: 800;
    letter-spacing: -1px;
  }
  .stat-label { font-size: 11px; color: var(--text3); margin-top: 2px; font-weight: 500; }
  .stat-change { font-size: 11px; margin-top: 6px; font-weight: 600; }

  /* Life areas */
  .life-area-item {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 12px;
  }
  .area-name { width: 100px; font-size: 13px; font-weight: 600; }
  .area-bar { flex: 1; }
  .area-score { width: 30px; text-align: right; font-size: 13px; font-weight: 700; font-family: var(--font-display); }

  /* Modal */
  .modal-overlay {
    position: fixed; inset: 0;
    background: rgba(0,0,0,0.7);
    z-index: 400;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    animation: fadeIn 0.2s ease;
  }
  .modal {
    width: 100%;
    max-width: 380px;
    background: var(--surface);
    border: 1px solid var(--border2);
    border-radius: 20px;
    padding: 24px;
    animation: scaleIn 0.2s ease;
  }
  .modal-title {
    font-family: var(--font-display);
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 16px;
  }
  .modal-input {
    width: 100%;
    background: var(--surface2);
    border: 1px solid var(--border2);
    border-radius: 10px;
    padding: 10px 14px;
    color: var(--text);
    font-family: var(--font-body);
    font-size: 14px;
    outline: none;
    margin-bottom: 10px;
  }
  .modal-input::placeholder { color: var(--text3); }
  .modal-textarea {
    resize: none;
    height: 100px;
  }
  .modal-btn {
    width: 100%;
    padding: 12px;
    border-radius: 12px;
    border: none;
    font-family: var(--font-display);
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.2s;
    margin-top: 4px;
  }
  .modal-btn-primary { background: linear-gradient(135deg, var(--accent), var(--accent2)); color: white; }
  .modal-btn-secondary { background: var(--surface2); color: var(--text2); margin-top: 8px; }

  /* Horizontal scroll pills */
  .pill-row {
    display: flex;
    gap: 8px;
    overflow-x: auto;
    padding-bottom: 4px;
    scrollbar-width: none;
    margin-bottom: 14px;
  }
  .pill-row::-webkit-scrollbar { display: none; }
  .pill {
    padding: 6px 14px;
    border-radius: 20px;
    border: 1px solid var(--border2);
    font-size: 12px;
    font-weight: 600;
    cursor: pointer;
    white-space: nowrap;
    transition: all 0.15s;
    color: var(--text3);
    background: var(--surface2);
  }
  .pill.active { background: var(--accent); border-color: var(--accent); color: white; }

  /* Streak badge */
  .streak-badge {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    background: rgba(245,158,11,0.15);
    border: 1px solid rgba(245,158,11,0.2);
    border-radius: 20px;
    padding: 2px 8px;
    font-size: 12px;
    font-weight: 700;
    color: var(--gold);
  }

  /* Mood selector */
  .mood-row {
    display: flex;
    gap: 8px;
    margin-bottom: 12px;
  }
  .mood-btn {
    flex: 1;
    aspect-ratio: 1;
    border-radius: 12px;
    background: var(--surface3);
    border: 2px solid transparent;
    cursor: pointer;
    font-size: 20px;
    display: flex; align-items: center; justify-content: center;
    transition: all 0.2s;
  }
  .mood-btn.selected { border-color: var(--accent); background: rgba(79,110,247,0.1); }

  /* Animations */
  @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
  @keyframes slideUp { from { transform: translateY(100%); } to { transform: translateY(0); } }
  @keyframes slideInLeft { from { transform: translateX(-100%); } to { transform: translateX(0); } }
  @keyframes scaleIn { from { transform: scale(0.95); opacity: 0; } to { transform: scale(1); opacity: 1; } }
  @keyframes pulse { 0%, 100% { opacity: 1; } 50% { opacity: 0.5; } }

  .dot-pulse { animation: pulse 2s infinite; }

  /* Gradient text */
  .gradient-text {
    background: linear-gradient(135deg, var(--accent), var(--accent3));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  /* Welcome banner */
  .welcome-banner {
    background: linear-gradient(135deg, rgba(79,110,247,0.15), rgba(124,58,237,0.1));
    border: 1px solid rgba(79,110,247,0.2);
    border-radius: var(--radius);
    padding: 20px;
    margin-bottom: 16px;
    position: relative;
    overflow: hidden;
  }
  .welcome-banner::before {
    content: '';
    position: absolute;
    top: -30px; right: -30px;
    width: 120px; height: 120px;
    background: radial-gradient(circle, rgba(79,110,247,0.2), transparent 70%);
  }

  .greeting { font-size: 13px; color: var(--text3); margin-bottom: 4px; font-weight: 500; }
  .greeting-name {
    font-family: var(--font-display);
    font-size: 22px;
    font-weight: 800;
    letter-spacing: -0.5px;
    margin-bottom: 12px;
  }

  .day-stats {
    display: flex;
    gap: 20px;
  }
  .day-stat { text-align: center; }
  .day-stat-value {
    font-family: var(--font-display);
    font-size: 20px;
    font-weight: 800;
  }
  .day-stat-label { font-size: 10px; color: var(--text3); font-weight: 600; text-transform: uppercase; letter-spacing: 0.5px; }

  /* Decision rating */
  .rating-stars {
    display: flex;
    gap: 4px;
    margin-top: 6px;
  }
  .rating-star { color: var(--text3); font-size: 12px; cursor: pointer; }
  .rating-star.filled { color: var(--gold); }

  /* Energy chart simple */
  .energy-bars {
    display: flex;
    align-items: flex-end;
    gap: 6px;
    height: 60px;
    margin-top: 12px;
  }
  .energy-bar {
    flex: 1;
    border-radius: 4px;
    opacity: 0.8;
  }
  .energy-label {
    display: flex;
    gap: 6px;
    margin-top: 6px;
  }
  .energy-label span { flex: 1; text-align: center; font-size: 10px; color: var(--text3); }

  /* Vision board */
  .vision-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
    margin-bottom: 12px;
  }
  .vision-item {
    border-radius: 12px;
    padding: 16px;
    min-height: 90px;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    cursor: pointer;
    transition: all 0.2s;
    position: relative;
    overflow: hidden;
  }
  .vision-item:hover { transform: scale(1.02); }
  .vision-item-title {
    font-family: var(--font-display);
    font-size: 13px;
    font-weight: 700;
    color: white;
    z-index: 1;
  }
  .vision-item-emoji {
    font-size: 28px;
    margin-bottom: 6px;
    z-index: 1;
  }

  .input-row { display: flex; gap: 8px; margin-bottom: 10px; }

  .toggle-btn {
    position: relative;
    width: 40px; height: 22px;
    background: var(--surface3);
    border-radius: 20px;
    cursor: pointer;
    transition: all 0.2s;
    border: none;
  }
  .toggle-btn.on { background: var(--accent); }
  .toggle-knob {
    position: absolute;
    top: 3px; left: 3px;
    width: 16px; height: 16px;
    background: white;
    border-radius: 50%;
    transition: all 0.2s;
  }
  .toggle-btn.on .toggle-knob { transform: translateX(18px); }

  .opportunity-item {
    padding: 14px;
    background: var(--surface3);
    border-radius: 12px;
    margin-bottom: 8px;
  }
  .opportunity-title { font-size: 14px; font-weight: 600; margin-bottom: 4px; }
  .opportunity-meta { font-size: 12px; color: var(--text3); display: flex; gap: 10px; }

  .future-letter {
    background: linear-gradient(135deg, rgba(124,58,237,0.1), rgba(79,110,247,0.08));
    border: 1px solid rgba(124,58,237,0.2);
    border-radius: var(--radius);
    padding: 20px;
    font-size: 14px;
    line-height: 1.8;
    color: var(--text2);
    font-style: italic;
    margin-bottom: 12px;
  }
`;

// ─── TIMER COMPONENT ──────────────────────────────────────────────────────────
function FocusTimer() {
  const [seconds, setSeconds] = useState(25 * 60);
  const [running, setRunning] = useState(false);
  const [mode, setMode] = useState("focus");
  const ref = useRef();

  useEffect(() => {
    if (running) {
      ref.current = setInterval(() => setSeconds(s => s > 0 ? s - 1 : 0), 1000);
    } else clearInterval(ref.current);
    return () => clearInterval(ref.current);
  }, [running]);

  const total = mode === "focus" ? 25 * 60 : 5 * 60;
  const progress = ((total - seconds) / total) * 100;
  const mm = String(Math.floor(seconds / 60)).padStart(2, "0");
  const ss = String(seconds % 60).padStart(2, "0");
  const r = 54;
  const circ = 2 * Math.PI * r;

  return (
    <div className="card card-accent">
      <div className="card-header">
        <span className="card-title">⚡ Focus Timer</span>
        <div style={{ display: "flex", gap: 6 }}>
          <span className={`pill ${mode === "focus" ? "active" : ""}`} onClick={() => { setMode("focus"); setSeconds(25 * 60); setRunning(false); }}>Focus</span>
          <span className={`pill ${mode === "break" ? "active" : ""}`} onClick={() => { setMode("break"); setSeconds(5 * 60); setRunning(false); }}>Break</span>
        </div>
      </div>
      <div className="timer-ring">
        <svg className="timer-svg" width="140" height="140" viewBox="0 0 140 140">
          <circle cx="70" cy="70" r={r} fill="none" stroke="rgba(255,255,255,0.05)" strokeWidth="8" />
          <circle cx="70" cy="70" r={r} fill="none" stroke={mode === "focus" ? "#4f6ef7" : "#10b981"} strokeWidth="8"
            strokeDasharray={circ} strokeDashoffset={circ - (circ * progress / 100)}
            strokeLinecap="round" style={{ transition: "stroke-dashoffset 1s ease" }} />
        </svg>
        <div className="timer-text">
          <div className="timer-number">{mm}:{ss}</div>
          <div className="timer-label">{mode === "focus" ? "DEEP WORK" : "BREAK"}</div>
        </div>
      </div>
      <div style={{ display: "flex", gap: 8, justifyContent: "center" }}>
        <button className="modal-btn modal-btn-primary" style={{ maxWidth: 140, padding: "10px" }} onClick={() => setRunning(r => !r)}>
          {running ? "⏸ Pause" : "▶ Start"}
        </button>
        <button className="modal-btn modal-btn-secondary" style={{ maxWidth: 80, padding: "10px" }} onClick={() => { setRunning(false); setSeconds(mode === "focus" ? 25 * 60 : 5 * 60); }}>
          ↺ Reset
        </button>
      </div>
    </div>
  );
}

// ─── HOME DASHBOARD ───────────────────────────────────────────────────────────
function HomeDashboard({ data, setData }) {
  const completedHabits = data.habits.filter(h => h.done).length;
  const totalHabits = data.habits.length;

  const toggleHabit = (id) => {
    setData(d => ({ ...d, habits: d.habits.map(h => h.id === id ? { ...h, done: !h.done, streak: !h.done ? h.streak + 1 : h.streak } : h) }));
  };

  const energyData = [
    { h: "6AM", val: 40 }, { h: "8AM", val: 75 }, { h: "10AM", val: 95 },
    { h: "12PM", val: 70 }, { h: "2PM", val: 45 }, { h: "4PM", val: 65 },
    { h: "6PM", val: 80 }, { h: "8PM", val: 50 },
  ];
  const maxE = Math.max(...energyData.map(e => e.val));

  return (
    <div>
      <div className="welcome-banner">
        <div className="greeting">Good morning ☀️</div>
        <div className="greeting-name">Welcome back, <span className="gradient-text">Alex.</span></div>
        <div className="day-stats">
          <div className="day-stat">
            <div className="day-stat-value" style={{ color: "#4f6ef7" }}>{completedHabits}/{totalHabits}</div>
            <div className="day-stat-label">Habits</div>
          </div>
          <div className="day-stat">
            <div className="day-stat-value" style={{ color: "#10b981" }}>3</div>
            <div className="day-stat-label">Exp. Active</div>
          </div>
          <div className="day-stat">
            <div className="day-stat-value" style={{ color: "#f59e0b" }}>21</div>
            <div className="day-stat-label">Day Streak</div>
          </div>
          <div className="day-stat">
            <div className="day-stat-value" style={{ color: "#ec4899" }}>4</div>
            <div className="day-stat-label">Goals</div>
          </div>
        </div>
      </div>

      <div className="stats-row">
        <div className="stat-card">
          <div className="stat-value gradient-text">87%</div>
          <div className="stat-label">Weekly Discipline</div>
          <div className="stat-change" style={{ color: "#10b981" }}>↑ +12% this week</div>
        </div>
        <div className="stat-card">
          <div className="stat-value" style={{ color: "#f59e0b" }}>🔥 21</div>
          <div className="stat-label">Day Streak</div>
          <div className="stat-change" style={{ color: "#f59e0b" }}>Personal best!</div>
        </div>
      </div>

      <FocusTimer />

      <div className="section-header">
        <span className="section-title">Today's Habits</span>
        <span className="section-action">{completedHabits}/{totalHabits} done</span>
      </div>
      <div className="card">
        <div className="progress-bar" style={{ marginBottom: 14 }}>
          <div className="progress-fill" style={{ width: `${(completedHabits / totalHabits) * 100}%`, background: "linear-gradient(90deg, #4f6ef7, #7c3aed)" }} />
        </div>
        {data.habits.map(h => (
          <div key={h.id} className="habit-item" onClick={() => toggleHabit(h.id)}>
            <div className={`habit-check ${h.done ? "done" : ""}`}>
              {h.done && <Icon d={Icons.check} size={14} color="white" />}
            </div>
            <span style={{ fontSize: 18 }}>{h.icon}</span>
            <div style={{ flex: 1 }}>
              <div style={{ fontSize: 14, fontWeight: 600, textDecoration: h.done ? "line-through" : "none", color: h.done ? "var(--text3)" : "var(--text)" }}>{h.name}</div>
              <div style={{ fontSize: 11, color: "var(--text3)" }}>{h.category}</div>
            </div>
            <span className="streak-badge">🔥 {h.streak}</span>
          </div>
        ))}
      </div>

      <div className="section-header">
        <span className="section-title">Energy Pattern</span>
        <span className="badge badge-cyan">Today</span>
      </div>
      <div className="card">
        <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 8 }}>Peak productivity: <span style={{ color: "#4f6ef7", fontWeight: 600 }}>10AM–12PM</span></div>
        <div className="energy-bars">
          {energyData.map((e, i) => (
            <div key={i} className="energy-bar" style={{ height: `${(e.val / maxE) * 100}%`, background: e.val > 80 ? "#4f6ef7" : e.val > 60 ? "#7c3aed" : "var(--surface3)" }} />
          ))}
        </div>
        <div className="energy-label">
          {energyData.map((e, i) => <span key={i}>{e.h.replace("M", "")}</span>)}
        </div>
      </div>

      <div className="section-header">
        <span className="section-title">Upcoming</span>
      </div>
      <div className="card">
        {[
          { time: "7:00 PM", label: "Evening Reflection", icon: "📓", color: "#8b5cf6" },
          { time: "9:00 PM", label: "Deep Work Session #2", icon: "⚡", color: "#4f6ef7" },
          { time: "Sun", label: "Weekly Review", icon: "📊", color: "#10b981" },
        ].map((item, i) => (
          <div key={i} style={{ display: "flex", alignItems: "center", gap: 12, padding: "10px 0", borderBottom: i < 2 ? "1px solid var(--border)" : "none" }}>
            <div style={{ width: 36, height: 36, borderRadius: 10, background: `${item.color}20`, display: "flex", alignItems: "center", justifyContent: "center", fontSize: 18 }}>
              {item.icon}
            </div>
            <div style={{ flex: 1 }}>
              <div style={{ fontSize: 14, fontWeight: 600 }}>{item.label}</div>
              <div style={{ fontSize: 11, color: "var(--text3)" }}>{item.time}</div>
            </div>
            <Icon d={Icons.bell} size={16} color="var(--text3)" />
          </div>
        ))}
      </div>

      <div className="section-header">
        <span className="section-title">Active Experiments</span>
      </div>
      {data.experiments.filter(e => e.status === "active").map(exp => (
        <div key={exp.id} className="card">
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 10 }}>
            <div>
              <div style={{ fontSize: 14, fontWeight: 700, marginBottom: 4 }}>🧪 {exp.title}</div>
              <div style={{ fontSize: 12, color: "var(--text3)" }}>Day {exp.day} of {exp.duration}</div>
            </div>
            <span className="badge badge-blue">Active</span>
          </div>
          <div className="progress-bar">
            <div className="progress-fill" style={{ width: `${(exp.day / exp.duration) * 100}%`, background: "#06b6d4" }} />
          </div>
        </div>
      ))}
    </div>
  );
}

// ─── GROWTH DASHBOARD ─────────────────────────────────────────────────────────
function GrowthDashboard({ data, setData }) {
  const [tab, setTab] = useState("habits");

  return (
    <div>
      <div className="pill-row">
        {["habits", "skills", "learning", "challenges", "experiments", "comfort"].map(t => (
          <span key={t} className={`pill ${tab === t ? "active" : ""}`} onClick={() => setTab(t)}>
            {t.charAt(0).toUpperCase() + t.slice(1)}
          </span>
        ))}
      </div>

      {tab === "habits" && (
        <>
          <div className="stats-row">
            <div className="stat-card">
              <div className="stat-value gradient-text">{data.habits.filter(h => h.done).length}/{data.habits.length}</div>
              <div className="stat-label">Today Complete</div>
            </div>
            <div className="stat-card">
              <div className="stat-value" style={{ color: "#f59e0b" }}>🔥 21</div>
              <div className="stat-label">Best Streak</div>
            </div>
          </div>
          <div className="card">
            <div className="card-header">
              <span className="card-title">🎯 Habit Tracker</span>
              <button className="modal-btn modal-btn-primary" style={{ width: "auto", padding: "6px 12px", fontSize: 12, marginTop: 0 }}
                onClick={() => setData(d => ({ ...d, habits: [...d.habits, { id: Date.now(), name: "New Habit", streak: 0, done: false, icon: "⭐", category: "General" }] }))}>
                + Add
              </button>
            </div>
            {data.habits.map(h => (
              <div key={h.id} className="habit-item" onClick={() => setData(d => ({ ...d, habits: d.habits.map(hab => hab.id === h.id ? { ...hab, done: !hab.done } : hab) }))}>
                <div className={`habit-check ${h.done ? "done" : ""}`}>
                  {h.done && <Icon d={Icons.check} size={14} color="white" />}
                </div>
                <span style={{ fontSize: 20 }}>{h.icon}</span>
                <div style={{ flex: 1 }}>
                  <div style={{ fontSize: 14, fontWeight: 600 }}>{h.name}</div>
                  <div style={{ fontSize: 11, color: "var(--text3)" }}>{h.category}</div>
                </div>
                <span className="streak-badge">🔥 {h.streak}</span>
              </div>
            ))}
          </div>
        </>
      )}

      {tab === "skills" && (
        <div className="card">
          <div className="card-header">
            <span className="card-title">🚀 Skill Development</span>
          </div>
          {data.skills.map(s => (
            <div key={s.id} style={{ marginBottom: 16 }}>
              <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 6 }}>
                <div>
                  <div style={{ fontSize: 14, fontWeight: 600 }}>{s.name}</div>
                  <div style={{ fontSize: 11, color: "var(--text3)" }}>{s.category} · {s.hoursLogged}h logged</div>
                </div>
                <span style={{ fontFamily: "var(--font-display)", fontWeight: 800, fontSize: 18 }}>{s.level}%</span>
              </div>
              <div className="progress-bar">
                <div className="progress-fill" style={{ width: `${s.level}%`, background: s.level > 70 ? "#10b981" : s.level > 40 ? "#4f6ef7" : "#f59e0b" }} />
              </div>
            </div>
          ))}
        </div>
      )}

      {tab === "learning" && (
        <div className="card">
          <div className="card-header">
            <span className="card-title">📚 Books & Learning</span>
          </div>
          {data.books.map(b => (
            <div key={b.id} style={{ marginBottom: 16 }}>
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 8 }}>
                <div>
                  <div style={{ fontSize: 14, fontWeight: 700 }}>{b.title}</div>
                  <div style={{ fontSize: 12, color: "var(--text3)" }}>{b.author}</div>
                </div>
                <span className={`badge ${b.progress === 100 ? "badge-green" : "badge-blue"}`}>{b.progress}%</span>
              </div>
              <div className="progress-bar" style={{ marginBottom: 6 }}>
                <div className="progress-fill" style={{ width: `${b.progress}%`, background: b.progress === 100 ? "#10b981" : "#4f6ef7" }} />
              </div>
              <div style={{ fontSize: 12, color: "var(--text3)", fontStyle: "italic" }}>"{b.notes}"</div>
            </div>
          ))}
        </div>
      )}

      {tab === "challenges" && (
        <div>
          {data.challenges.map(c => (
            <div key={c.id} className="card">
              <div className="card-header">
                <span className="card-title">🏆 {c.title}</span>
                <span className={`badge ${c.status === "done" ? "badge-green" : "badge-blue"}`}>{c.status === "done" ? "Complete" : "Active"}</span>
              </div>
              <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 8, fontSize: 12, color: "var(--text3)" }}>
                <span>Day {c.completed} of {c.days}</span>
                <span>{Math.round((c.completed / c.days) * 100)}%</span>
              </div>
              <div className="progress-bar">
                <div className="progress-fill" style={{ width: `${(c.completed / c.days) * 100}%`, background: c.status === "done" ? "#10b981" : "#4f6ef7" }} />
              </div>
            </div>
          ))}
          <button className="modal-btn modal-btn-primary" style={{ marginTop: 8 }}
            onClick={() => setData(d => ({ ...d, challenges: [...d.challenges, { id: Date.now(), title: "New Challenge", days: 30, completed: 0, status: "active" }] }))}>
            + New Challenge
          </button>
        </div>
      )}

      {tab === "experiments" && (
        <div>
          {data.experiments.map(e => (
            <div key={e.id} className="card">
              <div className="card-header">
                <span className="card-title">🧪 {e.title}</span>
                <span className={`badge ${e.status === "complete" ? "badge-green" : "badge-blue"}`}>{e.status}</span>
              </div>
              <div style={{ fontSize: 13, color: "var(--text3)", marginBottom: 10, fontStyle: "italic" }}>Hypothesis: {e.hypothesis || e.result}</div>
              {e.status === "active" && (
                <div className="progress-bar">
                  <div className="progress-fill" style={{ width: `${(e.day / e.duration) * 100}%`, background: "#06b6d4" }} />
                </div>
              )}
              {e.status === "complete" && <div style={{ fontSize: 12, background: "rgba(16,185,129,0.1)", border: "1px solid rgba(16,185,129,0.2)", borderRadius: 8, padding: "8px 10px", color: "#34d399" }}>✓ Result: {e.result}</div>}
            </div>
          ))}
        </div>
      )}

      {tab === "comfort" && (
        <div>
          <div className="card">
            <div className="card-header">
              <span className="card-title">💪 Comfort Zone Breakers</span>
            </div>
            <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12 }}>Small daily actions that push your limits</div>
            {data.comfortBreakers.map(b => (
              <div key={b.id} className="habit-item" onClick={() => setData(d => ({ ...d, comfortBreakers: d.comfortBreakers.map(cb => cb.id === b.id ? { ...cb, done: !cb.done } : cb) }))}>
                <div className={`habit-check ${b.done ? "done" : ""}`}>
                  {b.done && <Icon d={Icons.check} size={14} color="white" />}
                </div>
                <div style={{ flex: 1, fontSize: 14, fontWeight: 500 }}>{b.action}</div>
              </div>
            ))}
          </div>
        </div>
      )}
    </div>
  );
}

// ─── THINKING DASHBOARD ───────────────────────────────────────────────────────
function ThinkingDashboard({ data, setData }) {
  const [tab, setTab] = useState("ideas");
  const [newIdea, setNewIdea] = useState("");

  return (
    <div>
      <div className="pill-row">
        {["ideas", "problems", "decisions", "opportunities"].map(t => (
          <span key={t} className={`pill ${tab === t ? "active" : ""}`} onClick={() => setTab(t)}>
            {t.charAt(0).toUpperCase() + t.slice(1)}
          </span>
        ))}
      </div>

      {tab === "ideas" && (
        <>
          <div className="card">
            <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 8 }}>Quick capture</div>
            <div className="input-row">
              <input className="modal-input" style={{ marginBottom: 0, flex: 1 }} placeholder="New idea..." value={newIdea} onChange={e => setNewIdea(e.target.value)} />
              <button className="modal-btn modal-btn-primary" style={{ width: "auto", padding: "10px 16px", marginTop: 0 }}
                onClick={() => { if (newIdea.trim()) { setData(d => ({ ...d, ideas: [{ id: Date.now(), title: newIdea, tags: [], date: new Date().toLocaleDateString(), status: "idea" }, ...d.ideas] })); setNewIdea(""); } }}>
                Add
              </button>
            </div>
          </div>
          {data.ideas.map(idea => (
            <div key={idea.id} className="card">
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 8 }}>
                <div style={{ fontSize: 15, fontWeight: 700 }}>💡 {idea.title}</div>
                <span className={`badge ${idea.status === "validating" ? "badge-gold" : idea.status === "exploring" ? "badge-blue" : "badge-purple"}`}>{idea.status}</span>
              </div>
              <div style={{ display: "flex", gap: 6, flexWrap: "wrap" }}>
                {idea.tags.map((tag, i) => <span key={i} className="badge badge-cyan">{tag}</span>)}
              </div>
              <div style={{ fontSize: 11, color: "var(--text3)", marginTop: 8 }}>{idea.date}</div>
            </div>
          ))}
        </>
      )}

      {tab === "problems" && (
        <div>
          <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12, background: "rgba(245,158,11,0.1)", border: "1px solid rgba(245,158,11,0.2)", borderRadius: 10, padding: "10px 12px" }}>
            🔍 Great entrepreneurs are problem hunters. Log every problem you observe.
          </div>
          {data.problems.map(p => (
            <div key={p.id} className="card">
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 8 }}>
                <span className="badge badge-red">{p.industry}</span>
                <span style={{ fontSize: 11, color: "var(--text3)" }}>{p.date}</span>
              </div>
              <div style={{ fontSize: 14, fontWeight: 600, marginBottom: 8 }}>⚠️ {p.problem}</div>
              <div style={{ fontSize: 13, color: "var(--accent3)", background: "rgba(6,182,212,0.08)", borderRadius: 8, padding: "8px 10px" }}>
                💡 Opportunity: {p.opportunity}
              </div>
            </div>
          ))}
          <button className="modal-btn modal-btn-primary" onClick={() => setData(d => ({ ...d, problems: [{ id: Date.now(), industry: "Unknown", problem: "New problem observed", opportunity: "TBD", date: new Date().toLocaleDateString() }, ...d.problems] }))}>
            + Log Problem
          </button>
        </div>
      )}

      {tab === "decisions" && (
        <div>
          <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12 }}>Track important decisions and learn from outcomes</div>
          {data.decisions.map(d => (
            <div key={d.id} className="card">
              <div style={{ fontSize: 14, fontWeight: 700, marginBottom: 6 }}>🎯 {d.decision}</div>
              <div style={{ fontSize: 11, color: "var(--text3)", marginBottom: 10 }}>{d.date}</div>
              {d.outcome && <div style={{ fontSize: 13, color: "var(--text2)", marginBottom: 8, fontStyle: "italic" }}>Outcome: {d.outcome}</div>}
              {d.rating && (
                <div className="rating-stars">
                  {Array.from({ length: 10 }, (_, i) => (
                    <span key={i} className={`rating-star ${i < d.rating ? "filled" : ""}`}>★</span>
                  ))}
                </div>
              )}
              {!d.outcome && <span className="badge badge-gold">Pending outcome</span>}
            </div>
          ))}
        </div>
      )}

      {tab === "opportunities" && (
        <div>
          {data.opportunities.map(o => (
            <div key={o.id} className="opportunity-item">
              <div className="opportunity-title">{o.title}</div>
              <div className="opportunity-meta">
                <span>📍 {o.source}</span>
                <span className={`badge ${o.potential === "High" ? "badge-green" : "badge-gold"}`}>{o.potential}</span>
                <span className={`badge ${o.status === "pursuing" ? "badge-blue" : "badge-purple"}`}>{o.status}</span>
              </div>
            </div>
          ))}
          <button className="modal-btn modal-btn-primary" style={{ marginTop: 8 }}
            onClick={() => setData(d => ({ ...d, opportunities: [{ id: Date.now(), title: "New opportunity", source: "Unknown", status: "pending", potential: "Medium" }, ...d.opportunities] }))}>
            + Add Opportunity
          </button>
        </div>
      )}
    </div>
  );
}

// ─── REFLECTION DASHBOARD ─────────────────────────────────────────────────────
function ReflectionDashboard({ data, setData }) {
  const [tab, setTab] = useState("journal");
  const [newEntry, setNewEntry] = useState("");
  const [selectedMood, setSelectedMood] = useState(null);

  const moods = ["😞", "😕", "😐", "🙂", "😊", "😄", "🤩"];

  return (
    <div>
      <div className="pill-row">
        {["journal", "fears", "lessons", "mood", "minddump", "weekly"].map(t => (
          <span key={t} className={`pill ${tab === t ? "active" : ""}`} onClick={() => setTab(t)}>
            {t === "minddump" ? "Mind Dump" : t === "weekly" ? "Weekly" : t.charAt(0).toUpperCase() + t.slice(1)}
          </span>
        ))}
      </div>

      {tab === "journal" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">✍️ Today's Entry</span></div>
            <div style={{ marginBottom: 10 }}>
              <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 8 }}>How's your energy today?</div>
              <div className="mood-row">
                {moods.map((m, i) => (
                  <button key={i} className={`mood-btn ${selectedMood === i ? "selected" : ""}`} onClick={() => setSelectedMood(i)}>{m}</button>
                ))}
              </div>
            </div>
            <textarea className="modal-input modal-textarea" placeholder="What happened today? What did you learn? How do you feel?"
              value={newEntry} onChange={e => setNewEntry(e.target.value)} />
            <button className="modal-btn modal-btn-primary" onClick={() => {
              if (newEntry.trim()) {
                setData(d => ({ ...d, journal: [{ id: Date.now(), date: new Date().toLocaleDateString(), mood: selectedMood || 5, entry: newEntry, tags: [] }, ...d.journal] }));
                setNewEntry(""); setSelectedMood(null);
              }
            }}>Save Entry</button>
          </div>
          {data.journal.map(j => (
            <div key={j.id} className="card">
              <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 8 }}>
                <span style={{ fontSize: 11, color: "var(--text3)" }}>{j.date}</span>
                <span style={{ fontSize: 20 }}>{moods[j.mood - 1] || "🙂"}</span>
              </div>
              <div style={{ fontSize: 14, color: "var(--text2)", lineHeight: 1.6 }}>{j.entry}</div>
            </div>
          ))}
        </div>
      )}

      {tab === "fears" && (
        <div>
          <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12, background: "rgba(124,58,237,0.1)", border: "1px solid rgba(124,58,237,0.2)", borderRadius: 10, padding: "10px 12px" }}>
            🦁 Courage is not the absence of fear. Face each one deliberately.
          </div>
          {data.fears.map(f => (
            <div key={f.id} className="card">
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 8 }}>
                <div style={{ fontSize: 15, fontWeight: 600 }}>😰 {f.fear}</div>
                <span className={`badge ${f.facing ? "badge-green" : "badge-red"}`}>{f.facing ? "Facing" : "Avoiding"}</span>
              </div>
              <div style={{ fontSize: 13, color: "var(--accent)", marginTop: 8 }}>📋 Plan: {f.plan}</div>
            </div>
          ))}
          <button className="modal-btn modal-btn-primary" onClick={() => setData(d => ({ ...d, fears: [...d.fears, { id: Date.now(), fear: "New fear to face", facing: false, plan: "Create an action plan" }] }))}>
            + Add Fear
          </button>
        </div>
      )}

      {tab === "lessons" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">📖 Failure & Lessons Log</span></div>
            {[
              { lesson: "Launched too late — spent too long perfecting, lost market window", date: "2024-12", type: "Business" },
              { lesson: "Ignored early user feedback signals about pricing", date: "2024-11", type: "Product" },
              { lesson: "Burned out from working 14h days for 3 weeks straight", date: "2024-10", type: "Health" },
            ].map((l, i) => (
              <div key={i} style={{ padding: "12px 0", borderBottom: i < 2 ? "1px solid var(--border)" : "none" }}>
                <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 6 }}>
                  <span className="badge badge-purple">{l.type}</span>
                  <span style={{ fontSize: 11, color: "var(--text3)" }}>{l.date}</span>
                </div>
                <div style={{ fontSize: 14, color: "var(--text2)", lineHeight: 1.5 }}>💡 {l.lesson}</div>
              </div>
            ))}
          </div>
        </div>
      )}

      {tab === "mood" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">🌡️ Mood & Energy Tracker</span></div>
            <div style={{ marginBottom: 16 }}>
              <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12 }}>This week's mood pattern</div>
              {["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"].map((day, i) => {
                const val = [6, 8, 5, 9, 7, 8, 7][i];
                return (
                  <div key={i} style={{ display: "flex", alignItems: "center", gap: 12, marginBottom: 8 }}>
                    <span style={{ width: 30, fontSize: 12, color: "var(--text3)" }}>{day}</span>
                    <div style={{ flex: 1, height: 8, borderRadius: 4, background: "var(--surface3)", overflow: "hidden" }}>
                      <div style={{ width: `${val * 10}%`, height: "100%", borderRadius: 4, background: val > 7 ? "#10b981" : val > 5 ? "#4f6ef7" : "#f59e0b" }} />
                    </div>
                    <span style={{ fontSize: 12, fontWeight: 700, width: 20 }}>{val}</span>
                  </div>
                );
              })}
            </div>
          </div>
        </div>
      )}

      {tab === "minddump" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">🌊 Mind Dump</span></div>
            <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 10 }}>Empty your head. No filters. Just write.</div>
            <textarea className="modal-input modal-textarea" style={{ height: 200 }} placeholder="Dump everything on your mind right now..." />
            <button className="modal-btn modal-btn-primary">Save Dump</button>
          </div>
        </div>
      )}

      {tab === "weekly" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">📊 Weekly Review</span></div>
            {[
              { q: "Top 3 wins this week?", a: "Launched landing page, booked 3 sales calls, hit 5-day streak" },
              { q: "Biggest obstacle?", a: "Time management — got pulled into too many meetings" },
              { q: "What would you do differently?", a: "Block calendar earlier, say no more often" },
              { q: "Next week's #1 priority?", a: "Close first paying customer" },
            ].map((item, i) => (
              <div key={i} style={{ marginBottom: 14 }}>
                <div style={{ fontSize: 12, color: "var(--text3)", fontWeight: 600, marginBottom: 4 }}>{item.q}</div>
                <div style={{ fontSize: 14, color: "var(--text2)", lineHeight: 1.5 }}>{item.a}</div>
              </div>
            ))}
            <button className="modal-btn modal-btn-primary" style={{ marginTop: 8 }}>Start Fresh Review</button>
          </div>
        </div>
      )}
    </div>
  );
}

// ─── VISION DASHBOARD ─────────────────────────────────────────────────────────
function VisionDashboard({ data, setData }) {
  const [tab, setTab] = useState("goals");

  return (
    <div>
      <div className="pill-row">
        {["goals", "vision", "letter", "lifescore", "money"].map(t => (
          <span key={t} className={`pill ${tab === t ? "active" : ""}`} onClick={() => setTab(t)}>
            {t === "lifescore" ? "Life Score" : t === "letter" ? "Future Me" : t.charAt(0).toUpperCase() + t.slice(1)}
          </span>
        ))}
      </div>

      {tab === "goals" && (
        <div>
          <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12 }}>Short-term and long-term goals tracking</div>
          {["short", "long"].map(type => (
            <div key={type}>
              <div className="section-header" style={{ marginTop: 4 }}>
                <span className="section-title">{type === "short" ? "🏃 Short-term" : "🎯 Long-term"}</span>
              </div>
              {data.goals.filter(g => g.type === type).map(g => (
                <div key={g.id} className="card">
                  <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 8 }}>
                    <div>
                      <div style={{ fontSize: 15, fontWeight: 700 }}>{g.title}</div>
                      <div style={{ fontSize: 12, color: "var(--text3)", marginTop: 2 }}>📅 {g.deadline} · {g.area}</div>
                    </div>
                    <span style={{ fontFamily: "var(--font-display)", fontWeight: 800, fontSize: 18, color: g.progress > 75 ? "#10b981" : g.progress > 40 ? "#4f6ef7" : "#f59e0b" }}>{g.progress}%</span>
                  </div>
                  <div className="progress-bar">
                    <div className="progress-fill" style={{ width: `${g.progress}%`, background: g.progress > 75 ? "#10b981" : g.progress > 40 ? "linear-gradient(90deg, #4f6ef7, #7c3aed)" : "#f59e0b" }} />
                  </div>
                </div>
              ))}
            </div>
          ))}
          <button className="modal-btn modal-btn-primary" onClick={() => setData(d => ({ ...d, goals: [...d.goals, { id: Date.now(), title: "New Goal", deadline: "2025-12", progress: 0, type: "short", area: "General" }] }))}>
            + Add Goal
          </button>
        </div>
      )}

      {tab === "vision" && (
        <div>
          <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 12 }}>Design your ideal future across every dimension</div>
          <div className="vision-grid">
            {[
              { label: "Dream Home", emoji: "🏡", bg: "linear-gradient(135deg, #1e3a5f, #2563eb)" },
              { label: "Business Empire", emoji: "🏢", bg: "linear-gradient(135deg, #1a1a2e, #7c3aed)" },
              { label: "Health & Fitness", emoji: "💪", bg: "linear-gradient(135deg, #064e3b, #10b981)" },
              { label: "Travel & Freedom", emoji: "✈️", bg: "linear-gradient(135deg, #1c1917, #d97706)" },
              { label: "Relationships", emoji: "❤️", bg: "linear-gradient(135deg, #4c0519, #ec4899)" },
              { label: "Knowledge & Skills", emoji: "🧠", bg: "linear-gradient(135deg, #0f172a, #06b6d4)" },
            ].map((v, i) => (
              <div key={i} className="vision-item" style={{ background: v.bg }}>
                <div className="vision-item-emoji">{v.emoji}</div>
                <div className="vision-item-title">{v.label}</div>
              </div>
            ))}
          </div>
        </div>
      )}

      {tab === "letter" && (
        <div>
          <div style={{ fontSize: 13, color: "var(--text3)", marginBottom: 12 }}>Write a letter to your future self. Be specific.</div>
          <div className="future-letter">
            Dear Future Alex,
            <br /><br />
            It's January 2025. By the time you read this — December 2025 — I hope you've launched the SaaS, generated your first $10K month, and proven to yourself that the vision was always possible.
            <br /><br />
            Remember: the person you're becoming is built one decision at a time. Stay consistent. Trust the process.
            <br /><br />
            — Past You
          </div>
          <button className="modal-btn modal-btn-primary">✏️ Write New Letter</button>
        </div>
      )}

      {tab === "lifescore" && (
        <div>
          <div className="card">
            <div className="card-header"><span className="card-title">⚡ Life Balance Score</span></div>
            <div style={{ fontSize: 12, color: "var(--text3)", marginBottom: 16 }}>Rate your current satisfaction in each life area</div>
            {data.lifeAreas.map((a, i) => (
              <div key={i} className="life-area-item">
                <div className="area-name" style={{ color: a.color }}>{a.area}</div>
                <div className="area-bar">
                  <div className="progress-bar">
                    <div className="progress-fill" style={{ width: `${a.score * 10}%`, background: a.color }} />
                  </div>
                </div>
                <div className="area-score" style={{ color: a.color }}>{a.score}</div>
              </div>
            ))}
            <div style={{ marginTop: 12, padding: 12, background: "var(--surface3)", borderRadius: 10, fontSize: 13, color: "var(--text2)", textAlign: "center" }}>
              Overall Life Score: <span style={{ fontFamily: "var(--font-display)", fontWeight: 800, color: "#4f6ef7" }}>{(data.lifeAreas.reduce((s, a) => s + a.score, 0) / data.lifeAreas.length).toFixed(1)}/10</span>
            </div>
          </div>
        </div>
      )}

      {tab === "money" && (
        <div>
          <div className="stats-row">
            <div className="stat-card">
              <div className="stat-value" style={{ color: "#10b981" }}>${data.money.income.toLocaleString()}</div>
              <div className="stat-label">Monthly Income</div>
              <div className="stat-change" style={{ color: "#10b981" }}>↑ +8% MoM</div>
            </div>
            <div className="stat-card">
              <div className="stat-value" style={{ color: "#4f6ef7" }}>${data.money.savings.toLocaleString()}</div>
              <div className="stat-label">Savings</div>
              <div className="stat-change" style={{ color: "#10b981" }}>↑ On track</div>
            </div>
          </div>
          <div className="stats-row">
            <div className="stat-card">
              <div className="stat-value" style={{ color: "#8b5cf6" }}>${data.money.investments.toLocaleString()}</div>
              <div className="stat-label">Investments</div>
              <div className="stat-change" style={{ color: "#10b981" }}>↑ +12.4%</div>
            </div>
            <div className="stat-card">
              <div className="stat-value" style={{ color: "#f59e0b" }}>${data.money.business.toLocaleString()}</div>
              <div className="stat-label">Business Rev.</div>
              <div className="stat-change" style={{ color: "#f59e0b" }}>↑ Growing</div>
            </div>
          </div>
          <div className="card">
            <div className="card-header"><span className="card-title">💰 Net Worth Trajectory</span></div>
            <div style={{ display: "flex", alignItems: "flex-end", gap: 8, height: 80 }}>
              {[35, 48, 52, 61, 70, 82, 100].map((v, i) => (
                <div key={i} style={{ flex: 1, height: `${v}%`, background: `rgba(79,110,247,${0.3 + i * 0.1})`, borderRadius: "4px 4px 0 0" }} />
              ))}
            </div>
            <div style={{ display: "flex", gap: 8, marginTop: 6 }}>
              {["Jul", "Aug", "Sep", "Oct", "Nov", "Dec", "Jan"].map((m, i) => (
                <span key={i} style={{ flex: 1, textAlign: "center", fontSize: 10, color: "var(--text3)" }}>{m}</span>
              ))}
            </div>
          </div>
        </div>
      )}
    </div>
  );
}

// ─── AI CHAT ──────────────────────────────────────────────────────────────────
function AIChat({ onClose }) {
  const [messages, setMessages] = useState([
    { role: "ai", text: "Hey! I'm your AI mentor. I can analyze your habits, help design experiments, review journal reflections, evaluate ideas, or help with goal planning. What would you like to work on?" }
  ]);
  const [input, setInput] = useState("");
  const [loading, setLoading] = useState(false);
  const bottomRef = useRef();

  useEffect(() => { bottomRef.current?.scrollIntoView({ behavior: "smooth" }); }, [messages]);

  const send = async () => {
    if (!input.trim() || loading) return;
    const userMsg = input.trim();
    setInput("");
    setMessages(m => [...m, { role: "user", text: userMsg }]);
    setLoading(true);

    try {
      const sysPrompt = `You are LifeOS AI — a world-class personal development mentor and strategic advisor. You help ambitious individuals grow their career, build businesses, develop discipline, and design their ideal future.

Your personality:
- Direct, insightful, and strategic
- You ask powerful questions that provoke deep thinking
- You provide specific, actionable advice
- You're like a combination of a Navy SEAL commander, a successful entrepreneur, and a Stoic philosopher
- Keep responses concise but high-value (2-4 paragraphs max)
- Reference frameworks like: First principles, Inversion, 80/20, Compounding, Systems thinking

When relevant, you can analyze the user's habits (morning meditation 14-day streak, reading 21-day streak), their goal to launch a SaaS, their skills (Python 65%, Public Speaking 40%), and their life scores.`;

      const res = await fetch("https://api.anthropic.com/v1/messages", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          model: "claude-sonnet-4-20250514",
          max_tokens: 1000,
          system: sysPrompt,
          messages: [
            ...messages.filter(m => m.role !== "ai" || messages.indexOf(m) > 0).map(m => ({
              role: m.role === "ai" ? "assistant" : "user",
              content: m.text
            })),
            { role: "user", content: userMsg }
          ]
        })
      });
      const data = await res.json();
      const reply = data.content?.[0]?.text || "Let me think on that and get back to you.";
      setMessages(m => [...m, { role: "ai", text: reply }]);
    } catch {
      setMessages(m => [...m, { role: "ai", text: "Connection issue. Please try again." }]);
    }
    setLoading(false);
  };

  const suggestions = ["Analyze my habits", "Help me design an experiment", "What's my biggest leverage point?", "Review my goals"];

  return (
    <div className="chat-overlay" onClick={e => e.target === e.currentTarget && onClose()}>
      <div className="chat-panel">
        <div className="chat-header">
          <div className="chat-ai-info">
            <div className="ai-avatar">🤖</div>
            <div>
              <div className="ai-name">LifeOS AI Mentor</div>
              <div className="ai-status"><span className="ai-dot dot-pulse" />Online — Ready to advise</div>
            </div>
          </div>
          <button className="icon-btn" onClick={onClose}><Icon d={Icons.close} size={18} /></button>
        </div>
        <div className="chat-messages">
          {messages.map((m, i) => (
            <div key={i} className={`msg msg-${m.role}`}>{m.text}</div>
          ))}
          {loading && (
            <div className="msg msg-ai">
              <span className="dot-pulse">Thinking</span>
              <span style={{ marginLeft: 4 }}>...</span>
            </div>
          )}
          <div ref={bottomRef} />
        </div>
        {messages.length === 1 && (
          <div style={{ padding: "0 16px 8px", display: "flex", flexWrap: "wrap", gap: 6 }}>
            {suggestions.map((s, i) => (
              <span key={i} className="pill" onClick={() => { setInput(s); }} style={{ cursor: "pointer" }}>{s}</span>
            ))}
          </div>
        )}
        <div className="chat-input-row">
          <input className="chat-input" placeholder="Ask your AI mentor..." value={input}
            onChange={e => setInput(e.target.value)}
            onKeyDown={e => e.key === "Enter" && send()} />
          <button className="send-btn" onClick={send}>
            <Icon d={Icons.send} size={18} color="white" />
          </button>
        </div>
      </div>
    </div>
  );
}

// ─── QUICK CAPTURE ────────────────────────────────────────────────────────────
function QuickCapture({ onClose, onSave }) {
  const [type, setType] = useState("idea");
  const [text, setText] = useState("");

  const types = [
    { id: "idea", label: "💡 Idea", color: "#f59e0b" },
    { id: "problem", label: "⚠️ Problem", color: "#ef4444" },
    { id: "note", label: "📝 Note", color: "#4f6ef7" },
    { id: "journal", label: "📓 Journal", color: "#8b5cf6" },
    { id: "fear", label: "😰 Fear", color: "#ec4899" },
    { id: "goal", label: "🎯 Goal", color: "#10b981" },
    { id: "experiment", label: "🧪 Experiment", color: "#06b6d4" },
    { id: "lesson", label: "📖 Lesson", color: "#7c3aed" },
  ];

  const selected = types.find(t => t.id === type);

  return (
    <div className="modal-overlay" onClick={e => e.target === e.currentTarget && onClose()}>
      <div className="modal">
        <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 16 }}>
          <div className="modal-title">⚡ Quick Capture</div>
          <button className="icon-btn" onClick={onClose}><Icon d={Icons.close} size={18} /></button>
        </div>
        <div style={{ display: "flex", flexWrap: "wrap", gap: 6, marginBottom: 14 }}>
          {types.map(t => (
            <span key={t.id} onClick={() => setType(t.id)}
              style={{ padding: "5px 10px", borderRadius: 20, fontSize: 12, fontWeight: 600, cursor: "pointer", transition: "all 0.15s",
                background: type === t.id ? `${t.color}20` : "var(--surface2)",
                border: `1px solid ${type === t.id ? t.color : "var(--border2)"}`,
                color: type === t.id ? t.color : "var(--text3)" }}>
              {t.label}
            </span>
          ))}
        </div>
        <textarea className="modal-input modal-textarea" placeholder={`Capture your ${type}...`} value={text} onChange={e => setText(e.target.value)} />
        <button className="modal-btn modal-btn-primary" onClick={() => { if (text.trim()) { onSave(type, text); onClose(); } }}>
          Save {selected?.label}
        </button>
        <button className="modal-btn modal-btn-secondary" onClick={onClose}>Cancel</button>
      </div>
    </div>
  );
}

// ─── SIDEBAR ──────────────────────────────────────────────────────────────────
function Sidebar({ onClose, onNavigate }) {
  const tools = [
    { icon: "📝", label: "Notes", color: "#4f6ef7", nav: "thinking" },
    { icon: "✅", label: "Habits", color: "#10b981", nav: "growth" },
    { icon: "💡", label: "Ideas", color: "#f59e0b", nav: "thinking" },
    { icon: "⚠️", label: "Problems", color: "#ef4444", nav: "thinking" },
    { icon: "🧪", label: "Experiments", color: "#06b6d4", nav: "growth" },
    { icon: "🏆", label: "Challenges", color: "#8b5cf6", nav: "growth" },
    { icon: "🚀", label: "Skills", color: "#7c3aed", nav: "growth" },
    { icon: "🎯", label: "Goals", color: "#10b981", nav: "vision" },
    { icon: "📓", label: "Journal", color: "#ec4899", nav: "reflection" },
    { icon: "😰", label: "Fear List", color: "#f59e0b", nav: "reflection" },
    { icon: "🔭", label: "Opportunities", color: "#4f6ef7", nav: "thinking" },
    { icon: "📚", label: "Learning / Books", color: "#06b6d4", nav: "growth" },
  ];

  return (
    <>
      <div className="sidebar-overlay" onClick={onClose} />
      <div className="sidebar">
        <div className="sidebar-header">
          <div className="sidebar-logo">Life<span className="os">OS</span></div>
          <div className="sidebar-tagline">Your Personal Operating System</div>
          <div style={{ marginTop: 12, display: "flex", gap: 8 }}>
            <div style={{ flex: 1, textAlign: "center", padding: "8px", background: "var(--surface2)", borderRadius: 8 }}>
              <div style={{ fontFamily: "var(--font-display)", fontWeight: 800, fontSize: 18, color: "#f59e0b" }}>🔥 21</div>
              <div style={{ fontSize: 10, color: "var(--text3)" }}>STREAK</div>
            </div>
            <div style={{ flex: 1, textAlign: "center", padding: "8px", background: "var(--surface2)", borderRadius: 8 }}>
              <div style={{ fontFamily: "var(--font-display)", fontWeight: 800, fontSize: 18, color: "#4f6ef7" }}>87%</div>
              <div style={{ fontSize: 10, color: "var(--text3)" }}>DISCIPLINE</div>
            </div>
            <div style={{ flex: 1, textAlign: "center", padding: "8px", background: "var(--surface2)", borderRadius: 8 }}>
              <div style={{ fontFamily: "var(--font-display)", fontWeight: 800, fontSize: 18, color: "#10b981" }}>7.5</div>
              <div style={{ fontSize: 10, color: "var(--text3)" }}>LIFE SCORE</div>
            </div>
          </div>
        </div>

        <div className="sidebar-section">
          <div className="sidebar-label">Tool Library</div>
          {tools.map((t, i) => (
            <div key={i} className="sidebar-item" onClick={() => { onNavigate(t.nav); onClose(); }}>
              <div className="icon-wrap" style={{ background: `${t.color}18` }}>
                <span style={{ fontSize: 16 }}>{t.icon}</span>
              </div>
              <span>{t.label}</span>
            </div>
          ))}
        </div>

        <div className="sidebar-section">
          <div className="sidebar-label">Account</div>
          <div className="sidebar-item"><div className="icon-wrap" style={{ background: "#4f6ef720" }}><Icon d={Icons.user} size={14} color="#4f6ef7" /></div>Profile</div>
          <div className="sidebar-item"><div className="icon-wrap" style={{ background: "#64748b20" }}><Icon d={Icons.settings} size={14} color="#94a3b8" /></div>Settings</div>
        </div>
      </div>
    </>
  );
}

// ─── MAIN APP ─────────────────────────────────────────────────────────────────
export default function LifeOS() {
  const [tab, setTab] = useState("home");
  const [sidebarOpen, setSidebarOpen] = useState(false);
  const [chatOpen, setChatOpen] = useState(false);
  const [captureOpen, setCaptureOpen] = useState(false);
  const [data, setData] = useState(initialData);

  const navItems = [
    { id: "home", label: "HOME", icon: Icons.home },
    { id: "growth", label: "GROWTH", icon: Icons.growth },
    { id: "thinking", label: "THINKING", icon: Icons.brain },
    { id: "reflection", label: "REFLECT", icon: Icons.reflection },
    { id: "vision", label: "VISION", icon: Icons.vision },
  ];

  const tabTitles = {
    home: <><span style={{ color: "var(--accent)" }}>Life</span>OS</>,
    growth: "Growth",
    thinking: "Thinking",
    reflection: "Reflection",
    vision: "Vision",
  };

  const handleSave = (type, text) => {
    setData(d => {
      switch (type) {
        case "idea": return { ...d, ideas: [{ id: Date.now(), title: text, tags: [], date: new Date().toLocaleDateString(), status: "idea" }, ...d.ideas] };
        case "problem": return { ...d, problems: [{ id: Date.now(), industry: "General", problem: text, opportunity: "TBD", date: new Date().toLocaleDateString() }, ...d.problems] };
        case "goal": return { ...d, goals: [{ id: Date.now(), title: text, deadline: "2025-12", progress: 0, type: "short", area: "General" }, ...d.goals] };
        case "fear": return { ...d, fears: [{ id: Date.now(), fear: text, facing: false, plan: "Create a plan" }, ...d.fears] };
        case "journal": return { ...d, journal: [{ id: Date.now(), date: new Date().toLocaleDateString(), mood: 7, entry: text, tags: [] }, ...d.journal] };
        case "note": return { ...d, notes: [{ id: Date.now(), title: text.slice(0, 40), content: text, tags: [], pinned: false, date: new Date().toLocaleDateString() }, ...d.notes] };
        case "experiment": return { ...d, experiments: [{ id: Date.now(), title: text, duration: 7, day: 0, status: "active", hypothesis: "TBD" }, ...d.experiments] };
        default: return d;
      }
    });
  };

  return (
    <>
      <style>{styles}</style>
      <div className="app">
        <div className="topbar">
          <button className="icon-btn" onClick={() => setSidebarOpen(true)}>
            <Icon d={Icons.menu} size={18} />
          </button>
          <div className="topbar-title">{tabTitles[tab]}</div>
          <button className="icon-btn">
            <Icon d={Icons.search} size={18} />
          </button>
        </div>

        <div className="scroll-area">
          {tab === "home" && <HomeDashboard data={data} setData={setData} />}
          {tab === "growth" && <GrowthDashboard data={data} setData={setData} />}
          {tab === "thinking" && <ThinkingDashboard data={data} setData={setData} />}
          {tab === "reflection" && <ReflectionDashboard data={data} setData={setData} />}
          {tab === "vision" && <VisionDashboard data={data} setData={setData} />}
        </div>

        {/* Floating Buttons */}
        <div className="fab-container">
          <button className="fab fab-ai" onClick={() => setChatOpen(true)} title="AI Mentor">
            <span style={{ fontSize: 22 }}>🤖</span>
          </button>
          <button className="fab fab-main" onClick={() => setCaptureOpen(true)} title="Quick Capture">
            <Icon d={Icons.plus} size={24} color="white" strokeWidth={2.5} />
          </button>
        </div>

        {/* Bottom Nav */}
        <div className="bottom-nav">
          {navItems.map(n => (
            <div key={n.id} className={`nav-item ${tab === n.id ? "active" : ""}`} onClick={() => setTab(n.id)}>
              <Icon d={n.icon} size={20} color={tab === n.id ? "var(--accent)" : "var(--text3)"} />
              <span>{n.label}</span>
            </div>
          ))}
        </div>

        {/* Overlays */}
        {sidebarOpen && <Sidebar onClose={() => setSidebarOpen(false)} onNavigate={setTab} />}
        {chatOpen && <AIChat onClose={() => setChatOpen(false)} />}
        {captureOpen && <QuickCapture onClose={() => setCaptureOpen(false)} onSave={handleSave} />}
      </div>
    </>
  );
}
