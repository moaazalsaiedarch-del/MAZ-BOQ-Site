<p align="center">
  <img src="icon.png" width="150" alt="Arch-Moaaz Aboualized Logo">
</p>

<h1 align="center">Arch-Moaaz Aboualized</h1>

<p align="center">
  تطبيق أندرويد لحصر التشطيبات، يعمل بدون إنترنت
</p>

<div dir="rtl">

## ✨ المميزات

- يعمل بالكامل بدون إنترنت.
- البيانات تُحفظ داخل التطبيق على الجهاز.
- تصدير Excel وPDF وJPG عبر قائمة المشاركة في أندرويد.

## 📥 تحميل التطبيق

حمّل أحدث ملف app-debug.apk من تبويب [Releases](../../releases) على الموبايل مباشرة، وثبّته واسمح بالتثبيت من هذا المصدر عند الطلب.

## 🛠️ المتطلبات (مرة واحدة على الكمبيوتر)

1. [Node.js](https://nodejs.org) (إصدار 18 أو أحدث)
2. [Android Studio](https://developer.android.com/studio) (يثبّت معه Java وأدوات أندرويد). افتحه مرة وسيحمّل المكونات المطلوبة.

## 🚀 بناء الـ APK

افتح الطرفية داخل المجلد ونفّذ بالترتيب:

npm install
npx cap add android
npm run sync
ثم اختر أحد الطريقين:

الطريقة 1: من Android Studio

npx cap open android
ثم: Build ← Build Bundle(s) / APK(s) ← Build APK(s)، وعند الانتهاء اضغط locate لفتح مكان الملف.

الطريقة 2: من الطرفية

cd android
./gradlew assembleDebug
على ويندوز: gradlew.bat assembleDebug

الملف الناتج: android/app/build/outputs/apk/debug/app-debug.apk

## ☁️ بناء APK على GitHub (بدون Android Studio)

1. أنشئ مستودعًا جديدًا (New repository).
2. ارفع كل محتويات المجلد بما فيها المجلد المخفي .github.
3. افتح تبويب Actions وانتظر انتهاء Build APK (5 إلى 10 دقائق).
4. افتح تبويب Releases وحمّل app-debug.apk.

## 📝 ملاحظات

- عند تعديل www/index.html نفّذ npm run sync ثم أعد البناء.
- هذا APK للتجربة والاستخدام الشخصي (debug). للنشر على Google Play يلزم توقيع ملف release.

</div>
