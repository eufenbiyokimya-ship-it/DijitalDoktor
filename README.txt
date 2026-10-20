DİJİTAL DOKTOR - Android Studio projesi (çevrim dışı, internet izni yok)
1) Android Studio'yu açın: File > Open > bu klasörü seçin (ilk açılışta Gradle ve SDK 34 indirilir, internet gerekir).
2) Test: telefonu USB ile bağlayıp Run, veya Build > Build APK(s).
3) Çıktı: app/build/outputs/apk/debug/app-debug.apk (telefona kopyalayıp kurabilirsiniz; "bilinmeyen kaynak" iznini açın).
4) Mağazaya yüklemek için: Build > Generate Signed Bundle / APK.
İçerik güncellemek için app/src/main/assets/index.html dosyasını değiştirin.
CSV: Takip sekmesindeki "CSV indir" düğmesi Android'de paylaşım menüsünü açar (Drive, Dosyalar, e-posta vb.).
Simge (sola dönük hilal): app/src/main/res/mipmap-* ve drawable/ic_launcher_foreground.xml; açılış ekranı: drawable/splash.xml ve values/themes.xml.

--- BİLGİSAYARA KURULUM YAPMADAN APK (GitHub ile, ücretsiz) ---
1) github.com'da hesap açın, "New repository" ile boş bir depo oluşturun.
2) Bu klasörün içindekileri depoya yükleyin (Add file > Upload files). ".github" klasörü gizli görünebilir;
   yüklenmezse depoda Add file > Create new file deyip yol olarak ".github/workflows/build-apk.yml" yazın ve build-apk.yml içeriğini yapıştırın.
3) Depoda Actions sekmesi > "APK derle" > Run workflow. 4-6 dakika sonra bitince çalıştırmanın altındaki "Artifacts" bölümünden DijitalDoktor-APK dosyasını indirin.
4) İndirilen zip içindeki app-debug.apk dosyasını telefona kopyalayıp kurun.
