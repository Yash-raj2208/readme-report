# 🩺 HealthLens AI — Health Report Analyzer

Analyze blood reports in plain language. Upload a lab report image or enter values manually to get instant, easy-to-understand health advice.

---

## 🚀 Quick Start (3 steps)

### 1. Install dependencies
```bash
npm install
```

### 2. Start the server
```bash
npm start
```

### 3. Open the app
Go to: **http://localhost:3000**

---

## 📁 File Structure

```
health-analyzer/
├── server.js              ← Node.js + Express backend (POST /analyze)
├── package.json           ← Dependencies
├── public/
│   ├── index.html         ← Main UI
│   ├── style.css          ← Styles
│   ├── script.js          ← OCR, chart, API logic
│   └── sample_report.png  ← Test image (upload this to try OCR)
└── README.md
```

---

## 🧪 Testing

### Manual entry
1. Click **Manual Entry**
2. Enter: Hemoglobin=11.2, Glucose=158, Cholesterol=242
3. Click **Analyze My Report**

### OCR Upload
1. Click **Upload Report**
2. Upload `sample_report.png` from the `public/` folder
3. Wait for OCR to extract values (~10–20 seconds)
4. Click **Analyze My Report**

---

## 📊 What it analyzes

| Parameter | Low | Normal | High |
|-----------|-----|--------|------|
| Hemoglobin | < 12 g/dL | 12–17.5 | > 17.5 |
| Glucose | < 70 mg/dL | 70–100 | > 100 |
| Cholesterol | < 150 mg/dL | < 200 | > 200 |

---

## ⚠️ Disclaimer
This tool is for **educational purposes only**. Always consult a qualified doctor for medical diagnosis and treatment.