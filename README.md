# Ghost Pizza & Döner

Cizre Ghost Pizza & Döner için tanıtım, QR menü ve WhatsApp sipariş sitesi. Tek dosya (`index.html`), sunucu gerektirmez.

## Düzenleme

Bütün işletme bilgileri `index.html` içindeki `CONFIG` ve `MENU` bölümlerinde:

- `phone`: telefon (ör. `05xx xxx xx xx`). Boşsa arama butonları gizlenir.
- `whatsapp`: sipariş numarası, başında ülke kodu ile (ör. `905xxxxxxxxx`). Boşsa sipariş metni panoya kopyalanır.
- `address`: tam adres.
- `hours`: haftanın 7 günü, `["açılış","kapanış"]`. Pazar ile başlar. Kapalı gün için `null` yaz. Tamamı `null` ise saat bölümü gizlenir.
- `siteUrl`: yayın adresi. Boşsa QR kodlar sayfanın açıldığı adresi kullanır.
- `MENU`: kategoriler, ürünler ve fiyatlar.

## Masa QR kodları

Sitede QR menü sayfasında masa sayısını gir, kodları oluştur ve yazdır. Her kod `?masa=N` ile açılır ve sipariş mesajına masa numarası eklenir.

## Yayınlama (GitHub Pages)

Repo ayarlarında Settings, Pages bölümünde "Deploy from a branch", `main` ve `/ (root)` seçilir.
