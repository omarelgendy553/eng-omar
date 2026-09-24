# 🚀 Eng. Omar Elgendy - Portfolio

### بورتفوليو احترافي مستقبلي مع روبوت 3D تفاعلي

**Premium • Cinematic • Interactive • Futuristic**

هذا مشروع بورتفوليو شخصي باسم **Eng. Omar Elgendy** طالب ذكاء اصطناعي في جامعة المنوفية، مع روبوت 3D واقعي شبيه بالإنسان وتفاعل Scroll سينمائي.

---

## ✨ المميزات

- 🤖 **روبوت 3D واقعي** مبني بالكامل بالكود (Three.js) - ليس صورة
- 🎬 **تفاعل Scroll سينمائي** - الروبوت يفتح والكاميرا تدخل داخله
- 🖱️ **تفاعل الماوس** مع الروبوت والإضاءة
- 🌗 **ثيم مستقبلي فاخر** Dark Green / Blue
- 🗣️ **لغتين** عربي / إنجليزي مع RTL/LTR
- 🤖 **مساعد ذكي Omar AI** - Mock AI محلي بدون API
- 💬 **واتساب مباشر** للطلبات والشكاوى بدون Backend
- 📱 **متجاوب 100%** موبايل وتابلت وديسكتوب
- 🎯 **Custom Cursor** للديسكتوب
- ⚡ **Frontend فقط** - لا Backend لا Database

---

## 📁 هيكل المشروع

```
omar-portfolio/
├── public/
│   ├── models/
│   │   └── robot.glb (اختياري - لو عندك موديل جاهز)
│   ├── images/
│   │   └── profile.jpg (صورتك الشخصية)
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── RobotScene.jsx (الروبوت 3D)
│   │   ├── RobotIntro.jsx (مقدمة الروبوت)
│   │   ├── Navbar.jsx
│   │   ├── Hero.jsx
│   │   ├── About.jsx
│   │   ├── Skills.jsx
│   │   ├── Projects.jsx
│   │   ├── Services.jsx
│   │   ├── AIChat.jsx (المساعد الذكي)
│   │   ├── RequestForm.jsx
│   │   ├── ComplaintForm.jsx
│   │   ├── WhatsAppButton.jsx
│   │   ├── PrivacyConsent.jsx
│   │   ├── CustomCursor.jsx
│   │   ├── Footer.jsx
│   │   └── Contact.jsx
│   ├── data/
│   │   ├── profile.js (معلوماتك الشخصية - عدل هنا)
│   │   ├── projects.js (مشاريعك)
│   │   └── skills.js (مهاراتك)
│   ├── i18n/
│   │   ├── ar.json (النصوص العربية)
│   │   └── en.json (النصوص الإنجليزية)
│   ├── styles/
│   │   ├── global.css
│   │   └── animations.css
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

---

## 🛠️ طريقة التشغيل للمبتدئين (خطوة بخطوة)

### 1. تثبيت Node.js
- ادخل على https://nodejs.org
- حمل النسخة LTS (الخضراء)
- ثبته Next Next Next

### 2. فتح مجلد المشروع
- فك الضغط عن المشروع
- افتح المجلد `omar-portfolio`
- اضغط كليك يمين واختار `Open in Terminal` أو افتح `cmd` في المجلد
- أو افتح VS Code واسحب المجلد

### 3. تثبيت الحزم
في التيرمينال اكتب:
```bash
npm install
```
انتظر لحد ما يخلص (دقيقة أو اتنين)

### 4. تشغيل الموقع
```bash
npm run dev
```
هيظهر رابط مثل:
```
Local: http://localhost:5173/
```
افتحه في المتصفح

### 5. بناء المشروع للنشر
```bash
npm run build
```
هيتكون مجلد `dist` جاهز للنشر

---

## 🎨 التخصيص السهل

### أين أغير معلوماتي الشخصية؟
افتح ملف:
```
src/data/profile.js
```
غير:
- `name` اسمك
- `nameAr` اسمك بالعربي
- `phone` رقم واتساب
- `whatsappLink` رابط واتساب
- `telegramLink` رابط تيليجرام
- `description` وصفك
- الألوان

### أين أضع صورتي؟
ضع صورتك في:
```
public/images/profile.jpg
```
الموقع سيستخدمها تلقائياً في Hero والمشاريع. يمكنك استخدام `photo_2026-09-24_08-56-13.jpg` الموجودة.

### أين أضع robot.glb لو عندي؟
لو عندك موديل روبوت جاهز GLB:
```
public/models/robot.glb
```
الكود حالياً يبني روبوت procedural بالكود بدون الحاجة لملف خارجي، لكن لو وضعت الملف يمكنك تعديل `RobotScene.jsx` لاستخدامه.

### أين أغير رقم الواتساب؟
في ملف:
```
src/data/profile.js
```
غير:
```js
phone: "+201032853311",
phoneClean: "201032853311",
whatsappLink: "https://wa.me/201032853311",
```

### كيف أضيف مشروع جديد؟
افتح:
```
src/data/projects.js
```
انسخ مشروع موجود وعدل بياناته:
```js
{
  id: 4,
  title: "اسم المشروع",
  titleAr: "اسم المشروع عربي",
  description: "وصف انجليزي",
  descriptionAr: "وصف عربي",
  image: "/images/your-image.jpg",
  technologies: ["React", "AI"],
  github: "https://github.com/...",
  demo: "https://...",
  status: "real",
  category: "Web Development"
}
```

### كيف أغير الألوان؟
في ملف:
```
src/data/profile.js
```
أو في:
```
src/styles/global.css
```
في `:root` غير:
```css
--deep-green: #071A14
--green-accent: #1F8A70
--blue-accent: #3A607E
```

### كيف أغير النصوص؟
افتح:
```
src/i18n/ar.json
src/i18n/en.json
```
غير أي نص تريده، الموقع سيتغير تلقائياً.

---

## 🚀 النشر على GitHub Pages (مبسط جداً)

### الطريقة 1: GitHub Pages
1. أنشئ حساب على github.com
2. أنشئ Repository جديد باسم `omar-portfolio`
3. ارفع الملفات:
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/USERNAME/omar-portfolio.git
git push -u origin main
```
4. في GitHub، اذهب إلى Settings > Pages
5. اختر Source: GitHub Actions
6. استخدم Vite GitHub Pages Action

أو ببساطة:
```bash
npm run build
```
ثم ارفع محتويات `dist` إلى فرع `gh-pages`

### الطريقة 2: Vercel (أسهل)
1. ادخل vercel.com
2. سجل بـ GitHub
3. اضغط New Project
4. اختر مشروعك
5. اضغط Deploy - سيعمل مباشرة!

### الطريقة 3: Netlify
1. ادخل netlify.com
2. اسحب مجلد `dist` وأفلته في الموقع
3. سيعطيك رابط مباشر!

---

## 🤖 الروبوت 3D - شرح

الروبوت مبني بالكامل بـ Three.js procedural:

- **Head**: رأس مع Visor و Eyes متوهجة
- **Torso**: صدر يفتح (Chest panels) مع Core داخلي متوهج
- **Arms & Legs**: أذرع وأرجل مفصلة تشبه الإنسان
- **Materials**: Metallic مع reflections و emissive glow
- **Animation**:
  - 0% Scroll: مغلق Idle
  - 20%: حركة رأس
  - 35%: الصدر يبدأ يفتح
  - 50%: الألواح تتحرك
  - 65%: الإضاءة الداخلية تظهر
  - 80%: الكاميرا تقترب
  - 100%: مفتوح بالكامل والموقع يظهر من داخله

**Mouse Interaction**: حركة الماوس تؤثر على دوران الروبوت و Parallax

---

## 💬 نظام الطلبات والشكاوى

- لا Database
- لا Backend
- عند إرسال الطلب، يتم تجهيز رسالة واتساب تلقائياً
- يفتح واتساب على رقمك: `201032853311`
- العميل يضغط Send بنفسه

مثال رسالة الطلب:
```
مرحبًا عمر،

لدي طلب جديد:

الاسم: ...
رقم الهاتف: ...
نوع الطلب: ...
الموضوع: ...
التفاصيل: ...

تم الإرسال من موقعك الشخصي
```

---

## 🤖 Omar AI Assistant

- **لا API Key**
- **لا Backend**
- **Mock AI محلي ذكي** يرد بناءً على كلمات مفتاحية
- يعرف: اسمك، عمرك، عنوانك، جامعتك، مهاراتك
- يرد بشكل مختلف حسب السؤال (ليس رسالة ثابتة)
- واجهة Chat احترافية مع Typing Indicator

---

## 🔒 الخصوصية

- رسالة موافقة عند الدخول
- إذا وافق المستخدم: يمكن جمع معلومات يسمح بها المتصفح فقط:
  - Device Type, Browser, OS, Screen Size, Language, User Agent
  - Location فقط إذا سمح المستخدم عبر `navigator.geolocation`
- **لا يتم جمع**: Passwords, Files, Contacts, Camera, Microphone
- **لا يتم إرسال** البيانات تلقائياً لواتساب
- البيانات تبقى Local فقط (console.log للتوضيح)

---

## 📱 الموبايل

- يقلل جودة 3D تلقائياً
- يقلل Particles
- Custom Cursor معطل على الموبايل
- يحافظ على فكرة الروبوت

---

## ♿ تقليل الحركة

إذا المستخدم مفعل `prefers-reduced-motion`:
- تقل الأنيميشن الثقيلة
- الموقع يبقى قابل للاستخدام

---

## 🆘 حل المشاكل

**الروبوت لا يظهر؟**
- تأكد أنك شغلت `npm install`
- افتح Console في المتصفح (F12) وشوف الأخطاء
- الروبوت procedural لا يحتاج ملف glb

**الصورة لا تظهر؟**
- تأكد أن الصورة في `public/images/profile.jpg`
- اسم الملف يجب أن يكون بالضبط `profile.jpg`

**الموقع ثقيل؟**
- قلل `count` في `Particles` في `RobotScene.jsx`
- قلل `dpr` من `[1,2]` إلى `[1,1]`

**واتساب لا يفتح؟**
- تأكد من صيغة الرقم: `201032853311` بدون +
- جرب الرابط مباشرة: `https://wa.me/201032853311`

---

## 📞 معلومات الاتصال

- **Name**: Eng. Omar Elgendy / مهندس. عمر الجندي
- **Age**: 18
- **Address**: Sirs Ellyan, Elmonufia / سرس الليان، المنوفية
- **University**: Menoufia University - Faculty of AI
- **Phone**: +201032853311
- **WhatsApp**: https://wa.me/201032853311
- **Telegram**: https://t.me/omarelgendyy6

---

## 📄 الترخيص

هذا المشروع شخصي لـ Omar Elgendy. يمكنك استخدامه كقالب مع تغيير البيانات.

---

## 🙏 شكر

مبني بـ:
- React + Vite
- Three.js + React Three Fiber + Drei
- GSAP + ScrollTrigger
- Pure Frontend - No Backend!

**فكرة الموقع: ENTER OMAR'S DIGITAL WORLD - الروبوت هو بوابة الدخول!**

© 2026 Omar Elgendy - All Rights Reserved
