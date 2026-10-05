# Turhan Öztürk — Portfolyo

Referansın siyah, iri tipografili ve piksel desenli görsel yönünden esinlenilerek hazırlanmış kişisel portfolyo. Ana sayfanın HTML, CSS ve JavaScript kodları `index.html` içindedir. React, npm veya derleme gerektirmez.

## Önizleme

`index.html` dosyasını tarayıcıda açın. Görseller, CV ve sunumlar için klasör yapısını koruyun. Google Fonts internet bağlantısıyla yüklenir; çevrimdışı kullanımda sistem yazı tipleri devreye girer.

## Vercel’de yayınlama

1. ZIP’i açın. `index.html`, `vercel.json`, `img`, `logos`, `projeler` ve PDF aynı proje kökünde kalmalı.
2. Bu klasörün içeriğini bir GitHub deposuna yükleyin.
3. Vercel → Add New → Project üzerinden depoyu içe aktarın.
4. Framework Preset: **Other**. Root Directory: dosyaların bulunduğu kök klasör. Build Command: **boş**. Output Directory: **.**
5. Deploy seçeneğiyle yayınlayın. `vercel.json` statik site ayarlarını içerir.

Vercel CLI zaten kuruluysa bu klasörde `vercel --prod` ile de yayınlanabilir.

Resmi belge: https://vercel.com/docs/frameworks/more-frameworks

## İçeriği düzenleme

- Başlık, giriş metni ve üst düğmeler: `index.html` içindeki `hero` bölümü.
- Hakkımda, e-posta, LinkedIn, deneyimler ve projeler: aynı dosyadaki `SITE`, `EXPERIENCE`, `PROJECTS` ve diğer içerik dizileri.
- Renkler: `:root` değişkenleri.
- Fotoğraflar: `img/`; kurum logoları: `logos/`.
- Proje sunumları: `projeler/`; CV: `Turhan_Ozturk_CV.pdf`.

Metinli üst dock menüsü, dört projeli carousel, açık/koyu tema, e-posta kopyalama ve CV indirme bulunur. Menü, başlık, açıklama, etiket ve düğme metinleri görünür olduklarında TextEffect per-char fade benzeri biçimde harf harf saydamlıktan görünür hale gelir. Her harf 800 ms’de belirir; harfler arası gecikme en fazla 45 ms, bir metnin toplam açılma süresi en fazla 2,6 saniyedir. Satır düzeni ve bağlantılar korunur; takım sayılarının mevcut rakam animasyonu devam eder. İlk ekrandaki unvanlar öğrenci, dijital pazarlama stajyeri, stratejist ve sosyal girişimci sırasıyla 4,2 saniyede bir döner; geçişte dikey hareket, döndürme ve bulanıklık kullanılır. Takım sayıları görünür olduğunda 2 saniyelik kayan rakam animasyonu oynar. Ana düğmeler ve tüm “Sunumu aç” bağlantıları fareye doğru, iç metinleriyle birlikte yay hareketi yapar. Carousel oklarla, nokta göstergeleriyle, sağ/sol klavye tuşlarıyla ve dokunmatik yatay kaydırmayla gezilir. Her proje sunumuna kendi düğmesinden ulaşılır. Kaydırma çubuğu turuncu-sarı piksel temasındadır; üstteki sayfa ilerleme göstergesi kesintisiz, düz turuncu çizgidir. Alt piksel alevleri hızlandırılmıştır; yalnızca ilk ekranda imleç hareket ederken veya sabit dururken, @, %, #, *, + ve = sembolleri içeren piksel alevleri çıkar. Alev izi ilk ekranın dışına taşmaz; diğer bölümlerde ve proje sunumlarında görünmez. Efektler React gerektirmeyen HTML/CSS/JavaScript karşılıklarıdır; import edilen bir bileşen paketi yoktur. Cihazın hareket azaltma tercihi etkin olduğunda animasyonlar durur.

Godiva sunumu kullanıcının gönderdiği güncel godiva-reflect-portfolyo.html ile değiştirilmiştir. Diğer üç proje sunumu ve CV korunmuştur. Ana sayfa yeniden tasarlanmıştır; proje sunumları kendi tasarımlarıyla açılır. E-posta düğmesi cihazın e-posta uygulamasını açar; mesaj göndermez.
