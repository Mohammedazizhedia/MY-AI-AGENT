# بناء الـ APK بدون Android Studio (عن طريق GitHub)

## الخطوات (من المتصفح بس)
1. اعمل حساب مجاني على github.com.
2. اعمل Repository جديد (New repository) واسمه مثلا `my-agent`.
3. اضغط **Add file > Upload files**، وارفع **كل محتويات هذا المجلد** بنفس الترتيب:
   `www/`، `package.json`، `capacitor.config.json`، و`.github/workflows/build-apk.yml`.
   (لو الرفع من المتصفح مش بيقبل مجلد `.github` المخفي، اعمله بـ **Add file > Create new file**
   واكتب الاسم `.github/workflows/build-apk.yml` وانسخ محتوى الملف.)
4. اضغط Commit. هيبدأ البناء لوحده.
5. روح تبويب **Actions**، افتح آخر تشغيل، ولما يخلص (حوالي 5-8 دقايق) نزّل **my-agent-apk** من تحت.
6. فك الضغط، هتلاقي `app-debug.apk`. انقله للتاب والتليفون وثبّته.

## على الهواوي
- النسخة دي بتشتغل على HarmonyOS 4 عن طريق دعم تطبيقات أندرويد.
- التثبيت: افتح الملف من تطبيق الملفات، ووافق على التثبيت من مصدر خارجي.
- في الإعدادات جوه التطبيق حط مفتاح Claude API.

## بعد أي تعديل
عدّل `www/index.html` على GitHub واعمل Commit، والـ APK الجديد هيتبني تاني.
