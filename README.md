# Alhawija Android Updates

هذا المستودع مخصص لتوزيع إصدارات تطبيق الحويجة عبر GitHub Releases.

يقرأ التطبيق الملف `latest.json` عبر رابط raw، ثم يتحقق من رقم الإصدار ورابط HTTPS وبصمة SHA-256 قبل تنزيل APK. يجب رفع كل APK جديد إلى Release جديد، ثم تحديث `latest.json` في الفرع `main` بالقيم الجديدة.

لا ترفع ملفات keystore أو كلمات المرور أو `keystore.properties` إلى هذا المستودع.
