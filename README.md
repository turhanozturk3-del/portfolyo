# Turhan Öztürk · Portfolyo

Tek sayfalık statik site. Derleme adımı yok; klasörü olduğu gibi yayınlayın.

## Yayınlama
- **GitHub Pages:** Bu klasörün içeriğini bir repoya yükleyin → Settings → Pages → Branch: `main` / root.
- **Netlify:** app.netlify.com/drop adresine klasörü sürükleyin.
- **Vercel:** `vercel` komutu veya panelden "Import" → Framework: Other.

## İçerik güncelleme
`index.html` içindeki `<script>` bloğunun başında şu diziler var:
`SITE`, `FACTS`, `AWARDS`, `EXPERIENCE`, `PROJECTS`, `SKILLS`, `EDUCATION`, `CERTIFICATES`, `COMMUNITY`.
Yeni staj veya proje eklemek için ilgili diziye bir satır eklemeniz yeterli.

## Logolar
Şirket logolarını `logos/` klasörüne koyun (ör. `logos/vodafone.png`) ve `EXPERIENCE` içinde
`logo: "logos/vodafone.png"` yazın. Logo yoksa veya yüklenemezse şirketin baş harfi gösterilir.

## Sosyal medya önizlemesi
Siteyi yayınladıktan sonra `og:image` değerini tam adresle değiştirin,
ör. `https://kullanici.github.io/portfolyo/img/og.jpg`.
