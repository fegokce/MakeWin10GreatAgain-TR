# Windows 10'u Yeniden Harika Hale Getirin
Windows 10'u daha az sinir bozucu ve daha kullanışlı hale getirmek için ince ayarlar.

İşte bu kodun yaptığı:

1. Cortana'yı devre dışı bırakır
2. Bildirim Merkezini Devre Dışı Bırakır
3. Windows Güncellemeleri yüklendikten sonra otomatik yeniden başlatmaları devre dışı bırakır
4. Microsoft.com hesaplarını Windows Oturum Açma'dan devre dışı bırakır
5. Bilinen dosya türleri için dosya uzantılarını gösterir
6. Explorer'ı "Bu PC"ye açılacak şekilde ayarlar
7. Gizli dosyaları gösterir (işletim sistemi dosyaları dahil değildir)
8. OneDrive'ı Kaldırır
9. Masaüstünde "Bu Bilgisayar" simgesini gösterir
10. Geliştirici modunu etkinleştirir (Linux Alt Sistemi için gereklidir)
11. Linux Alt Sistemini Kurar
12. Powershell Get-Help öğelerini günceller
13. SMBv1'i devre dışı bırakır
14. Tüm Başlat Menüsü öğelerinin sabitlemesini kaldırın
15. WPAD'yi devre dışı bırakır

## Kurulum
Maalesef, bu betiği kullanmak için yürütme politikanızı sınırsız olarak ayarlamanız gerekecek.

Yönetici Powershell isteminden:
```
Set-ExecutionPolicy Sınırsız
cd MakeWindows10 GreatAgain
.\MakeWindows10GreatAgain.ps1
Set-ExecutionPolicy Kısıtlı
```

## Notlar
Win10 başlat menüsüyle birlikte gelen varsayılan uygulamaları/döşemeleri kaldırmak için bazı ince ayarlar eklemeyi düşündüm, ancak [Klasik Kabuk](http://classicshell.net/) beni çok şaşırttı. Win10 için mükemmel bir başlat menüsü değişimi. Sadece bunu yüklemenizi tavsiye ederim.

Bu komut dosyası, Windows 10'un gizlilik sorunlarının hiçbirini ele almıyor çünkü zaten bir sürü araç var (http://www.ghacks.net/2015/08/14/comparison-of-windows-10-privacy -tools/) zaten bunu yapıyor.
