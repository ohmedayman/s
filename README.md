# سوشيال فاست - منصة إدارة السوشيال ميديا (SaaS) 🚀

منصة متكاملة لإدارة السوشيال ميديا بأسلوب SaaS مع Landing Page و Firebase Authentication.

---

## الميزات

### 🏠 Landing Page
- تصميم احترافي جذاب
- قسم الميزات
- خطط الأسعار
- آراء العملاء
- CTA واضح

### 🔐 Firebase Authentication
- تسجيل الدخول بالبريد وكلمة المرور
- تسجيل الدخول بـ Google
- إعادة تعيين كلمة المرور
- حماية الصفحات

### 📊 Dashboard متكامل
- لوحة تحكم بالإحصائيات
- تقويم المحتوى
- مكتبة القوالب
- كاتب الكابشنات
- بحث الهاشتاجات
- إدارة الرسائل
- تحليل الأداء
- الإعدادات

---

## إعداد Firebase

### 1. إنشاء مشروع Firebase
1. اذهب إلى [Firebase Console](https://console.firebase.google.com)
2. أنشئ مشروع جديد
3. أضف تطبيق ويب

### 2. تفعيل Authentication
1. من Console، اذهب إلى **Authentication** > **Sign-in method**
2. فعّل **Email/Password**
3. فعّل **Google**

### 3. تحديث الكود
عثر على هذا الكود في `index.html` و استبدله ببيانات مشروعك:

```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
};
```

### 4. تفعيل Firestore (اختياري)
لتخزين بيانات المستخدمين:
1. أنشئ Firestore Database
2. اضبط قواعد الأمان حسب احتياجك

---

## التشغيل

1. افتح `index.html` في المتصفح
2. ستجد Landing Page أولاً
3. اضغط "ابدأ مجانًا" أو "تسجيل الدخول"
4. سجّل حساب جديد أو استخدم Google

---

## هيكل الصفحات

```
Landing Page
├── Hero Section
├── Features Section
├── Pricing Section
├── Testimonials Section
└── CTA Section

Auth Pages
├── Login (بريد + Google)
├── Register (بريد + Google)
└── Reset Password

Dashboard
├── لوحة التحكم
├── التقويم
├── القوالب
├── الكابشنات
├── الهاشتاجات
├── الرسائل
├── التحليل
└── الإعدادات
```

---

## ملاحظات مهمة

- **بيانات Firebase**: يجب استبدال بيانات التكوين ببيانات مشروعك الحقيقي
- **الأمان**: لا تضع مفاتيح Firebase في repos عامة
- **التطوير**: للإنتاج، يُنصح بإنشاء backend آمن للتعامل مع Firebase

---

## التقنيات

- React 18
- Tailwind CSS
- Firebase Auth
- Babel Standalone (للتطوير فقط)
