# NotaPusula

Müzisyenler için şarkı bilgisi arama arayüzü. Akor, BPM, ton, tür ve enstrüman notlarını sunar; seçilen şarkı çalışma kartını tarayıcıdan PDF'e kaydeder.

## Çalıştırma

`index.html` dosyasına çift tıklayın veya klasörde terminal açıp:

```bash
python3 -m http.server 8000
```

Ardından `http://localhost:8000` adresini açın.

## GitHub'a yükleme

1. GitHub'da giriş yapıp **New repository** seçin.
2. Depo adını `notapusula` yapın. Başlangıçta README/License eklemeyin.
3. Bu klasörde terminal açın ve çalıştırın:

```bash
git init
git add index.html README.md
git commit -m "NotaPusula ilk sürüm"
git branch -M main
git remote add origin https://github.com/KULLANICI_ADIN/notapusula.git
git push -u origin main
```

`KULLANICI_ADIN` kısmını kendi GitHub kullanıcı adınızla değiştirin. GitHub kimlik doğrulama penceresi açılırsa hesabınızla onaylayın.

## GitHub Pages ile yayına alma

1. Depoda **Settings → Pages** bölümünü açın.
2. **Deploy from a branch** seçin.
3. Branch olarak `main`, klasör olarak `/(root)` seçip **Save**'e basın.
4. Birkaç dakika sonra Pages ekranında verilen `https://KULLANICI_ADIN.github.io/notapusula/` adresini açın.

## MVP sınırı

Bu sürümde katalog örnek verilerden oluşur; şarkı arama ve analiz sonuçları gerçek bir müzik veritabanına bağlı değildir. Ses dosyasından otomatik akor/BPM/tür çıkarımı için lisanslı bir analiz API'si veya sunucu tarafı model entegrasyonu gerekir. PDF özelliği tarayıcının yazdırma ekranını açar; yazıcı hedefinde **PDF olarak kaydet** seçilir.
