DiskPart ile Temiz ve Yeniden Biçimlendirme (Önerilen)

Bu yöntem, USB'nin tüm gizli bölümlerini temizleyerek gerçek kapasitesine kavuşmasını sağlar .

1. Yönetici olarak Komut İstemi'ni açın: Başlat menüsüne cmd yazın, "Komut İstemi"ne sağ tıklayıp "Yönetici olarak çalıştır" seçeneğini seçin.
2. diskpart yazın ve Enter'a basın.
3. list disk yazın ve Enter'a basın. Bağlı tüm diskleri listeler. USB belleğinizin disk numarasını (örn. Disk 1) boyutundan (5 MB veya 64 GB olarak görünen) bularak not edin. Bilgisayarınızın ana diskini seçmemeye çok dikkat edin.
4. select disk X yazın (X yerine not ettiğiniz numarayı koyun) ve Enter'a basın.
5. Sırasıyla şu komutları yazıp her birinden sonra Enter'a basın:
   · clean: USB'deki tüm bölümleri ve yapılandırmayı siler .
   · create partition primary: Yeni bir ana bölüm oluşturur .
   · format fs=ntfs quick: USB'yi NTFS dosya sistemiyle hızlıca biçimlendirir. (Mac ile de kullanacaksanız format fs=exfat quick yazın) .
   · assign: USB'ye bir sürücü harfi atar .
6. exit yazarak kapatın.