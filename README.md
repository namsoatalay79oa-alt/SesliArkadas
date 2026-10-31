# Sesli Arkadaş — Android proje başlangıcı

Bu proje temel Türkçe ses tanıma ve sesli cevap prototipidir. Sürekli arka plan dinlemesi yapmaz.
Arama, SMS gönderme veya kişilere erişme gibi hassas işlemleri otomatik gerçekleştirmez; yalnızca
arama ekranını açar. Serbest yapay zekâ sohbeti için ayrıca güvenli bir sunucu/API entegrasyonu gerekir.

## Yerel derleme
1. Android Studio (JDK 17 desteği olan güncel sürüm) kurun.
2. Bu klasörü Android Studio ile açın ve Gradle senkronizasyonunu tamamlayın.
3. Build > Build Bundle(s) / APK(s) > Build APK(s) seçin.
4. APK: `app/build/outputs/apk/debug/app-debug.apk`

## GitHub Actions ile otomatik APK
1. Bu proje klasörünü GitHub deposuna yükleyin.
2. `Actions` sekmesine girin ve `Build Android APK` iş akışını çalıştırın (veya `main` dalına push edin).
3. İşlem tamamlanınca workflow çalışmasının `Artifacts` bölümünden `Sesli-Arkadas-debug-APK` dosyasını indirin.
4. ZIP'i açın; içindeki APK'yı Android telefona aktarın. Dosyayı açınca yalnızca bu kurulum için bilinmeyen uygulama yükleme izni verin.

## Önemli
- Bu, tam kapsamlı bir telefon kontrol botu değil, başlangıç prototipidir.
- APK üretimi için burada Android SDK/Gradle derlemesi çalıştırılmadı; proje Android Studio veya GitHub Actions üzerinde derlenmelidir.
- API anahtarı eklemeyin veya GitHub'a sır olarak konmamış gizli anahtarları yüklemeyin.
