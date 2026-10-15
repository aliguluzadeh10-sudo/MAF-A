# TH Mafia – APK qurulumu

Bu qovluq hazır Android layihəsidir (Capacitor). APK-nı GitHub özü qurur, kompüterdə heç nə quraşdırmaq lazım deyil.

## Yol 1: GitHub ilə (tövsiyə olunur)
1. github.com-da hesab aç (pulsuzdur) və yeni boş repo yarat (Public və ya Private).
2. Bu qovluğun içindəkiləri repoya yüklə. "uploading an existing file" linkinə bas və qovluğun bütün məzmununu (www, .github, package.json, capacitor.config.json) sürüklə.
   Əgər .github qovluğu görünmürsə, Git ilə yüklə:
   git init && git add . && git commit -m "init" && git branch -M main
   git remote add origin <repo-linki> && git push -u origin main
3. Repoda Actions bölməsinə keç. "Build APK" işləyəcək (3-6 dəqiqə).
4. İş bitəndə həmin run-a daxil ol, aşağıda Artifacts bölməsindən TH-Mafia-APK faylını endir. Zip-in içində app-debug.apk var.
5. APK-nı telefona at, aç. Android "naməlum mənbə" icazəsi istəyəcək, icazə ver.

## Yol 2: Android Studio ilə
npm install, npx cap add android, npx cap sync, npx cap open android. Sonra Build > Build APK(s).

## Oyunu dəyişmək
Bütün oyun www/index.html faylındadır.
