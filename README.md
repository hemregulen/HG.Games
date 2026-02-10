# 🥙 kebab.games

kebab.games - Lezzetli Oyunlar, Sınırsız Eğlence!

Modern, responsive ve kullanıcı dostu bir oyun platformu. Blazor WebAssembly teknolojisi ile geliştirilmiş klasik oyunların web versiyonları.

## 🎮 Özellikler

- **3 Klasik Oyun**: Yılan Oyunu, Tetris ve Mayın Tarlası
- **Responsive Tasarım**: Mobil, tablet ve masaüstü cihazlarda sorunsuz çalışır
- **Modern UI**: Şık ve kullanıcı dostu arayüz
- **Klavye Kontrolleri**: Oyunlar klavye tuşları ile kontrol edilebilir
- **Blazor WebAssembly**: Hızlı ve performanslı single-page application

## 🎯 Oyunlar

### 🐍 Yılan Oyunu
Klasik yılan oyunu. Yılanı kontrol ederek yemi topla ve büyü!
- **Kontroller**: Ok tuşları veya WASD
- **Hedef**: Yemi topla ve kendine çarpma

### 🧱 Tetris
Efsanevi blok yerleştirme oyunu.
- **Kontroller**: 
  - Sol/Sağ ok: Bloğu hareket ettir
  - Yukarı ok: Bloğu döndür
  - Aşağı ok: Hızlı düşür
  - Boşluk: Anında düşür
- **Hedef**: Satırları tamamla ve puan kazan

### 💣 Mayın Tarlası
Klasik mayın tarlası oyunu.
- **Kontroller**: 
  - Sol tık: Hücreyi aç
  - Sağ tık: Bayrak koy
- **Hedef**: Tüm mayınları işaretle ve güvenli hücreleri aç

## 🛠️ Teknolojiler

- **.NET 10.0**: En son .NET framework
- **Blazor WebAssembly**: Client-side C# ile web uygulaması geliştirme
- **C#**: Oyun mantığı ve uygulama kodu
- **HTML/CSS**: Modern ve responsive tasarım
- **Bootstrap Icons**: İkonlar için

## 📁 Proje Yapısı

```
HG.Games/
├── Layout/
│   ├── MainLayout.razor          # Ana sayfa düzeni
│   └── MainLayout.razor.css      # Düzen stilleri
├── Pages/
│   ├── Home.razor                # Ana sayfa - Oyun listesi
│   ├── Snake.razor               # Yılan oyunu
│   ├── Tetris.razor              # Tetris oyunu
│   ├── Minesweeper.razor         # Mayın tarlası oyunu
│   ├── Counter.razor             # Demo sayfa
│   ├── Weather.razor             # Demo sayfa
│   └── NotFound.razor            # 404 sayfası
├── wwwroot/
│   ├── css/                      # Stil dosyaları
│   ├── index.html                # Ana HTML dosyası
│   └── ...
├── App.razor                     # Uygulama root component
├── Program.cs                    # Uygulama giriş noktası
├── _Imports.razor                # Global using'ler
└── HG.Games.csproj              # Proje dosyası
```

## 🚀 Kurulum ve Çalıştırma

### Gereksinimler
- [.NET 10.0 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)

### Projeyi Klonlama
```bash
git clone https://github.com/hemregulen/HG.Games.git
cd HG.Games
```

### Projeyi Çalıştırma

#### Geliştirme Modu
```bash
dotnet run
```
Tarayıcıda otomatik olarak açılacaktır: `https://localhost:5001` veya `http://localhost:5000`

#### Production Build
```bash
dotnet publish -c Release
```
Build çıktısı `bin/Release/net10.0/publish/` klasöründe olacaktır.

Statik dosyalar `bin/Release/net10.0/publish/wwwroot/` altında bulunur. Bu klasörü bir statik sunucuyla servis ederek projeyi yeniden derlemeden kullanabilirsiniz (tarayıcı kısıtlamaları nedeniyle `index.html` dosyasını doğrudan açmak çalışmaz).

### Projeyi Build Etme
```bash
dotnet build HG.Games.sln
```

## 🎨 Geliştirme

### Yeni Oyun Ekleme

1. `Pages/` klasörüne yeni bir `.razor` dosyası oluştur
2. Oyun mantığını ve UI'ı component içinde tanımla
3. Oyunun stilini için `.razor.css` dosyası oluştur (scoped CSS)
4. `Pages/Home.razor` dosyasına oyun kartını ekle

### Stil Özelleştirme

- Her component için scoped CSS kullanılır (`.razor.css` dosyaları)
- Global stiller `wwwroot/css/app.css` dosyasında
- Layout stilleri `Layout/MainLayout.razor.css` dosyasında

## 📝 Lisans

Bu proje açık kaynaklıdır.

## 👥 Katkıda Bulunma

Katkılarınızı bekliyoruz! Pull request göndermekten çekinmeyin.

## 📧 İletişim

Proje ile ilgili sorularınız için issue açabilirsiniz.

---

**kebab.games** - Eğlence başlasın! 🎮
