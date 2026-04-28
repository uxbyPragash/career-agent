# ⚡ Career AI Agent

A 3-in-1 AI-powered career tool built with Claude AI:
- 📄 **Resume Builder** — ATS-optimized resume generator
- 🎤 **Interview Practice Bot** — Live mock interviews with feedback
- 🗺️ **Skill Roadmap Generator** — Personalized learning paths

---

## 🚀 Deploy to Vercel (5 Steps)

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "initial commit"
git remote add origin https://github.com/YOUR_USERNAME/career-agent.git
git branch -M main
git push -u origin main
```

### Step 2 — Import to Vercel
1. Go to https://vercel.com
2. Sign in with GitHub
3. Click **"Add New Project"**
4. Select your `career-agent` repo
5. Click **Deploy**

### Step 3 — Add API Key
1. Go to your project on Vercel dashboard
2. Click **Settings → Environment Variables**
3. Add:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** `sk-ant-xxxxxxxxxxxxxxxxx`
4. Click **Save**

### Step 4 — Redeploy
Go to **Deployments** tab → click **Redeploy**

### Step 5 — Done! 🎉
Your app is live at: `https://career-agent-xxx.vercel.app`

---

## 📁 Project Structure
```
career-agent/
├── public/
│   └── index.html      ← Frontend UI
├── api/
│   └── chat.js         ← Vercel serverless function (proxies Anthropic API)
├── vercel.json         ← Vercel routing config
├── package.json
└── .gitignore
```

---

## 🔑 Get Anthropic API Key
1. Go to https://console.anthropic.com
2. Sign up / Log in
3. Go to **API Keys** → **Create Key**
4. Copy the key (starts with `sk-ant-...`)

---

## 🛠️ Local Development
```bash
npm install -g vercel
vercel dev
# App runs at http://localhost:3000
```
