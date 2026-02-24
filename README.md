# 🥙 kebab.games

kebab.games - Lezzetli Oyunlar, Sınırsız Eğlence!

Modern, responsive ve kullanıcı dostu bir oyun platformu. Blazor WebAssembly teknolojisi ile geliştirilmiş klasik oyunların web versiyonları.

## 🎮 Özellikler

- **5 Oyun**: Yılan Oyunu, Tetris, Mayın Tarlası, Sudoku ve Renk Sıralama
- **Responsive Tasarım**: Mobil, tablet ve masaüstü cihazlarda sorunsuz çalışır
- **Modern UI**: Şık ve kullanıcı dostu arayüz
- **Klavye Kontrolleri**: Oyunlar klavye tuşları ile kontrol edilebilir
- **Blazor WebAssembly**: Hızlı ve performanslı single-page application

## 🎯 Oyunlar

### 🐍 Yılan Oyunu
Klasik yılan oyunu. Yılanı kontrol ederek yemi topla ve büyü!
- **Kontroller**: Ok tuşları veya WASD
- **Hedef**: Yemi topla ve kendine çarpma
![Yılan Oyunu](https://github.com/user-attachments/assets/481f7db8-d454-438b-a24b-8cd8025df3f5)

### 🧱 Tetris
Efsanevi blok yerleştirme oyunu.
- **Kontroller**: 
  - Sol/Sağ ok: Bloğu hareket ettir
  - Yukarı ok: Bloğu döndür
  - Aşağı ok: Hızlı düşür
  - Boşluk: Anında düşür
- **Hedef**: Satırları tamamla ve puan kazan
![Tetris](https://github.com/user-attachments/assets/2c656997-7143-4449-af52-8b80ffe5c4e8)

### 💣 Mayın Tarlası
Klasik mayın tarlası oyunu.
- **Kontroller**: 
  - Sol tık: Hücreyi aç
  - Sağ tık: Bayrak koy
- **Hedef**: Tüm mayınları işaretle ve güvenli hücreleri aç
![Mayın Tarlası](https://github.com/user-attachments/assets/28459a12-04d0-4739-a63c-3e5e97eed7d8)

### 🔢 Sudoku
Klasik Sudoku bulmacası.
- **Kontroller**: Ok tuşlarıyla hücre seç, 1-9 ile sayı gir, Backspace/Delete ile sil
- **Hedef**: Tüm hücreleri doğru sayılarla doldur
![Sudoku](https://github.com/user-attachments/assets/3cda1659-aa73-4cc4-8828-2b2f356400ff)

### 🧪 Renk Sıralama
Renkli sıvıları tüplerde doğru şekilde sıralama oyunu.
- **Kontroller**: Tüplere tıkla ve aynı renkteki sıvıyı uygun tüpe dök
- **Hedef**: Her tüpte tek renk kalacak şekilde sıvıları ayır

![Renk Sıralama](https://github.com/user-attachments/assets/9a5d5078-0562-4387-9f15-41af0cf33396)

### 🌯 Kebab Hunters
Eğlenceli ve zorlu bir yakalama oyunu! Yukarıdan düşen dürümleri yakala, sebzelerden kaç!
- **Kontroller**: 
  - A veya ← : Sola hareket
  - D veya → : Sağa hareket
  - Mobil: Dokunmatik kontrol butonları
- **Oynanış**:
  - 🌯 Dürümleri yakalayarak puan kazan (+10 puan)
  - 🥬🥒🥕 Sebzeleri yakalama (-1 can)
  - Her 100 puanda +1 can kazan (maksimum 5 can)
  - Her 3 saniyede sebze oranı %5 artıyor
  - Her 10 saniyede düşen item sayısı +1 artıyor
- **Zorluk Sistemi**:
  - Oyun başlangıcında %50 sebze, %50 dürüm
  - 30 saniye sonra %95 sebze düşüyor (maksimum zorluk!)
  - Düşme hızı giderek artıyor
  - Uzun süre hayatta kalmak gerçek bir başarı!

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
│   ├── Sudoku.razor              # Sudoku oyunu
│   ├── ColorSort.razor           # Renk sıralama oyunu
│   ├── Counter.razor             # Demo sayfa
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
