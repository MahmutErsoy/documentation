# FVM (Flutter Version Management) Rehberi

Bu dökümantasyon, FVM'nin ne olduğunu, ne amaçla kullanıldığını ve nasıl kurulup kullanıldığını açıklamaktadır.

## İçindekiler
- [FVM Nedir?](#fvm-nedir)
- [FVM Ne Amaçla Kullanılır?](#fvm-ne-amaçla-kullanılır)
- [FVM Nasıl Kurulur?](#fvm-nasıl-kurulur)
  - [MacOS ve Linux](#macos-ve-linux)
  - [Windows](#windows)
- [FVM Nasıl Kullanılır?](#fvm-nasıl-kullanılır)
  - [Flutter Sürümünü Yükleme](#flutter-sürümünü-yükleme)
  - [Proje İçin Flutter Sürümünü Ayarlama](#proje-için-flutter-sürümünü-ayarlama)
  - [Mevcut Sürümü Görüntüleme](#mevcut-sürümü-görüntüleme)
  - [Flutter Sürümünü Değiştirme](#flutter-sürümünü-değiştirme)
- [Sonuç](#sonuç)

## FVM Nedir?
FVM, Flutter Version Management'ın kısaltmasıdır. FVM, Flutter projelerinde birden fazla Flutter SDK sürümünü yönetmenize ve belirli bir proje için farklı bir Flutter SDK sürümünü kolayca kullanmanıza olanak tanır.

## FVM Ne Amaçla Kullanılır?
FVM, aşağıdaki amaçlar için kullanılır:
- Birden fazla Flutter projesinde farklı SDK sürümlerini kullanma.
- Proje bağımlılıklarının ve sürüm uyumluluğunun yönetimi.
- Takım projelerinde belirli bir Flutter sürümünün kullanılmasını sağlama.
- Yeni Flutter sürümlerini test etme ve entegrasyon süreçlerini kolaylaştırma.

## FVM Nasıl Kurulur?
FVM'yi kurmanın yolları işletim sistemine göre değişir.

### MacOS ve Linux
1. Homebrew kullanarak FVM'yi kurun:
    ```bash
    brew tap leoafarias/fvm
    brew install fvm
    ```

2. FVM'nin doğru kurulduğunu doğrulamak için:
    ```bash
    fvm --version
    ```

### Windows
1. Scoop kullanarak FVM'yi kurun:
    ```powershell
    scoop bucket add fvm https://github.com/leoafarias/scoop-bucket.git
    scoop install fvm
    ```

2. FVM'nin doğru kurulduğunu doğrulamak için:
    ```powershell
    fvm --version
    ```

## FVM Nasıl Kullanılır?
FVM'yi kullanarak Flutter SDK sürümlerini yönetebilir ve projelerinize özel sürümler atayabilirsiniz.

### Flutter Sürümünü Yükleme
Belirli bir Flutter sürümünü indirmek için:
```bash
fvm install <version>
```
Örnek 
```bash
fvm install 2.2.3
```

### Proje İçin Flutter Sürümünü Ayarlama
Belirli bir proje için kullanılacak Flutter sürümünü ayarlamak için projenizin kök dizininde:

```bash
fvm use <version>
```
Örnek 
```bash
fvm use 2.2.3
```

### Mevcut Sürümü Görüntüleme
Proje için geçerli olan Flutter sürümünü görüntülemek için:

```bash
fvm flutter --version
```

### Flutter Sürümünü Değiştirme
Başka bir sürüme geçmek için:

```bash
fvm use <version>
```

## Sonuç
FVM, Flutter projelerinde farklı SDK sürümlerini yönetmek için güçlü bir araçtır. Bu dökümantasyon, FVM'nin ne olduğunu, nasıl kurulacağını ve kullanılacağını açıklamaktadır. Daha fazla bilgi ve detaylı kullanım kılavuzu için FVM'nin resmi dökümantasyonuna başvurabilirsiniz.

### Ek Kaynaklar
- [Flutter Documentation](https://docs.flutter.dev)
- [FVM Kullanım Kılavuzu](https://fvm.app/docs)
