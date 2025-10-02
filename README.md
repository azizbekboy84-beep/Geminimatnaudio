# Gemini 2.5 Flash Ilovasi

Gemini AI modellari bilan ishlash uchun web ilova.

🌐 **Live Demo:** [Sizning Render URL'ingiz]

## Xususiyatlari

- ✍️ **Matn generatsiyalash** - Gemini 2.5 Flash
- ✨ **Matnni qisqartirish** - AI yordamida
- 🔊 **Ovozli javob** - Text-to-Speech (TTS)
- 🔍 **Google Search** - Manbalar bilan

## O'rnatish

1. Repozitoriyani klonlang:
   ```bash
   git clone <repo-url>
   cd geminisayt
   ```

2. `config.js` faylini yarating:
   ```bash
   cp config.example.js config.js
   ```

3. [Google AI Studio](https://aistudio.google.com/apikey) dan API kalit oling

4. `config.js` faylida API kalitni kiriting:
   ```javascript
   const CONFIG = {
       GEMINI_API_KEY: "SIZNING_API_KALITINGIZ"
   };
   ```

5. HTTP serverni ishga tushiring:
   ```bash
   python -m http.server 8000
   ```

6. Brauzerda oching: `http://localhost:8000/index.html`

## Muhim eslatma

⚠️ **`config.js` faylini GitHub'ga yuklaMang!** Bu fayl `.gitignore` da va sizning API kalitingizni saqlaydi.

## 🚀 Render.com'ga Deploy qilish

### 1. GitHub Repository yaratish

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin YOUR_GITHUB_REPO_URL
git push -u origin main
```

### 2. Render.com'da deploy

1. [Render.com](https://render.com)ga kiring
2. **New** → **Static Site** tanlang
3. GitHub repository'ni ulang
4. **Publish directory**: `.` (root)
5. **Deploy** tugmasini bosing

### 3. API Kalitni sozlash

Deploy qilingandan keyin:
1. Render.com dashboard'da **Environment** bo'limiga o'ting
2. `GEMINI_API_KEY` o'zgaruvchisini qo'shing
3. Qiymat: sizning API kalitingiz
4. Saqlang va redeploy qiling

**Muhim:** `config.js` faylini qo'lda Render'da tahrirlashingiz kerak bo'ladi yoki deployment script yozishingiz kerak.

## Fayllar tuzilishi

```
geminisayt/
├── index.html           # Asosiy HTML fayl
├── config.example.js    # Config namunasi
├── config.js           # API kalit (gitignore'da, local uchun)
├── .env                # Environment o'zgaruvchilar (gitignore'da)
├── .gitignore          # Git ignore qoidalari
└── README.md           # Loyiha hujjati
```

## Texnologiyalar

- **HTML5** - Asosiy struktura
- **Tailwind CSS** - Dizayn
- **Vanilla JavaScript** - Logika
- **Gemini API** - AI funksiyalari

## 🔐 Xavfsizlik

⚠️ **Muhim:** API kalitingizni hech qachon GitHub'ga yuklaMang! U `.gitignore` da va faqat local development uchun.
