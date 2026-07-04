# Borç Takip

Kişisel borç, sabit gider ve maaş takip uygulaması. Tamamen tarayıcıda çalışır, veriler sadece cihazında (localStorage) tutulur.

## GitHub Pages'e yükleme

1. GitHub'da yeni bir repo oluştur (örn. `Borc-Takip`).
2. Bu 5 dosyayı reponun **kök dizinine** yükle (aynı klasörde olmalılar):
   - `index.html`
   - `manifest.json`
   - `service-worker.js`
   - `icon-192.png`
   - `icon-512.png`
3. Repo **Settings → Pages** kısmından, Branch olarak `main` (veya `master`) ve klasör olarak `/ (root)` seçip kaydet.
4. Birkaç dakika sonra uygulaman `https://KULLANICI_ADIN.github.io/REPO_ADI/` adresinde yayında olacak.
5. iPhone'da Safari'den bu adresi aç → Paylaş → **Ana Ekrana Ekle**. Böylece bağımsız bir uygulama gibi, tam ekran ve **offline** çalışır.

## Güncelleme yaparken dikkat

- Her güncellemeden önce uygulama içinden ⚙ Ayarlar → **Yedek İndir** ile mutlaka yedek al.
- `service-worker.js` içindeki `CACHE_NAME` değerini her güncellemede değiştir (`v1` → `v2` → `v3`...). Aksi halde iPhone eski sürümü önbellekten göstermeye devam edebilir.
- Güncellenmiş dosyaları GitHub'a yükledikten sonra iPhone'da uygulamayı bir kez kapatıp yeniden açman yeterli.
