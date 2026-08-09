# DAVID Android Updates

Repository ini khusus untuk distribusi update DAVID Android.

## Baseline Production
- App: DAVID
- Package ID: id.david.packingproof
- Version: 1.3.1
- Version Code: 131
- Metadata updater: version.json
- Release APK: DAVID-v1.3.1-release.apk

## Fungsi Repository
- Menyimpan version.json yang dibaca oleh aplikasi DAVID.
- Menyimpan GitHub Release dan APK production untuk update user.
- Repository source aplikasi berada terpisah di DfaundaTolls/david-android-app.

## Aturan Update
1. Build dan sign APK dari repository source DAVID.
2. Gunakan production signing key DAVID yang sama.
3. Jangan mengubah package ID id.david.packingproof.
4. Version Code update baru harus lebih besar dari versi sebelumnya.
5. Upload APK final ke GitHub Release.
6. Setelah release tersedia, update version.json dengan versionName, versionCode, apkUrl, releasePageUrl, notes, dan publishedAt yang benar.
7. Commit dan push version.json ke branch main.

## Penting
Repository ini BUKAN repository source aplikasi dan tidak boleh berisi JKS, password signing, private license generator, atau private key.
