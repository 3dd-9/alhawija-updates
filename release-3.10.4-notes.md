# Alhawija 3.10.4

## Firebase Analytics

تم ربط تطبيق الحويجة بمشروع Firebase `aralhawija` وإضافة Firebase Analytics. يسجل التطبيق أحداثًا مجهولة فقط، من دون أسماء أو أرقام هواتف أو موقع دقيق.

يتم تسجيل فتح التطبيق مع رقم الإصدار، كما يمكن تسجيل استخدام مشاركة صورة المواقيت. تُعالج أحداث Analytics داخل SDK، وتبقى محفوظة محليًا عندما لا يتوفر الإنترنت، ثم تُرسل تلقائيًا إلى Firebase عند عودة الاتصال. لا تعتمد مواقيت الصلاة أو الأذان أو الودجات على Firebase، لذلك يبقى التطبيق يعمل دون اتصال.

| العنصر | القيمة |
|---|---|
| Firebase project | `aralhawija` |
| Android package | `com.ar.alhawija` |
| الأحداث الأساسية | `app_started` و`feature_used` |
| البيانات المسجلة | رقم الإصدار واسم ميزة عام فقط |
| توقيع APK | المفتاح الخاص نفسه المستخدم في الإصدارات السابقة |

## التحقق

تم تنفيذ `testDebugUnitTest` و`assembleRelease` بنجاح، وتحقق البناء من ملف `google-services.json` الخاص بالحزمة الصحيحة، كما تم التحقق من APK عبر APK Signature Scheme v2.

- Version code: 465
- Version name: 3.10.4
- SHA-256: `de968e646cf706056641c816cb77c723a7e500e722cc20ae55d4be2f8e15a067`
- شهادة التوقيع SHA-256: `2077b4e65ca5935e12a7f862f81cd8eee099c93d249f9578bcbcb73f9fafbfac`
- حجم APK: 13,749,652 بايت
