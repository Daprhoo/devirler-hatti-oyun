# Devirler Hattı

Tarayıcıda oynanan, çağ atlayan bir şerit strateji oyunu. Tek dosya (`index.html`), kurulum gerektirmez.

**Oyna:** https://daprhoo.github.io/devirler-hatti-oyun/ (GitHub Pages açıldıktan sonra)

## Öne çıkanlar
- **Yürüyen kale:** Üssün tekerlekler, paletler ya da itici motorlar üzerinde ilerler. Hattı daraltır, kulelerini cepheye taşır. `M` ile ilerlet/durdur.
- **Kıvılcım Taşı:** Haritanın ortasındaki taşı tutan taraf %30 fazla altın, tecrübe ve düzenli aralıklarla doktrin kazanır.
- **Devir ağacı:** Her çağ atlayışında iki medeniyet yolundan birini seçersin (ör. Şövalye Tarikatı ya da Bozkır Hanlığı). Her yol kendi bonusunu ve özel birliğini getirir.
- 7 çağ: Taş, Bronz, Ortaçağ, Barut, Çelik, Yıldız, Kuantum
- 12 bölümlük hikâye modu (Sefer), 4 zorluklu Serbest Savaş
- 4 komutan, 12 doktrin, savaş alanı olayları, kalıcı Miras Ağacı
- Her çağa özel üretken müzik ve konumsal ses efektleri

## Çalıştırma
`index.html` dosyasını tarayıcıda aç. Yazı tipleri Google Fonts'tan yüklenir; internet yoksa yedek yazı tipiyle çalışır.

## GitHub Pages
Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, klasör `/ (root)` → Save.

## Kontroller
`1` `2` `3` birlik · `4` kule · `5` özel güç · `6` komutan · `E` çağ atla · `M` kale · `Boşluk` duraklat

## Kod yapısı (`index.html` içinde)
- DATA: çağlar, birlikler, medeniyet yolları, kuleler, özel güçler, komutanlar, doktrinler, olaylar, hikâye
- AUDIO: ses efektleri ve çağa göre değişen müzik (Web Audio)
- DRAWING: birlik, kale, kule, Kıvılcım Taşı ve arka plan çizimleri (Canvas 2D)
- SIM: oyun mantığı, yapay zekâ
- HUD / SCREENS: arayüz ve menüler

İlerleme tarayıcının localStorage'ına kaydedilir (`devirler_hatti_v1`).
