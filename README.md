# HouseIQ — ML House Price Predictor

A machine learning powered web app that predicts house prices in Delhi NCR using Linear Regression and Random Forest ensemble models.

## Features
- **Linear Regression** & **Random Forest** ensemble prediction
- Feature importance visualization (Radar + Bar charts)
- Model performance comparison (R², RMSE, MAE)
- 90% confidence interval display
- Training data distribution charts
- ML pipeline visualization
- Fully responsive

## Tech Stack
- **Next.js 14** (App Router)
- **TypeScript**
- **Recharts** for data visualization
- ML logic in `/src/app/api/predict/route.ts`

## Local Development

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## Deploy to Vercel

### Option 1 — Vercel CLI (Fastest)
```bash
npm install -g vercel
vercel
```
Follow the prompts. On first deploy it will ask you to log in.

### Option 2 — GitHub + Vercel Dashboard
1. Push this project to a GitHub repo
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Framework will be auto-detected as **Next.js**
5. Click **Deploy** — done!

No environment variables needed for this project.

## Project Structure
```
src/
  app/
    api/predict/route.ts   ← ML prediction API
    page.tsx               ← Main page
    globals.css
    layout.tsx
  components/
    Header.tsx
    PredictionForm.tsx     ← Input sliders & controls
    ResultPanel.tsx        ← Prediction results + charts
    CorrelationChart.tsx   ← Training data overview
```
