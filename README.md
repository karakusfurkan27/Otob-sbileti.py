# Bilet Fiyatı Hesaplama Programı

Bu Python programı, bilet fiyatını yolcu sayısı, mesafe ve indirim oranına göre hesaplar. Mesafe üzerinden ek bir ücret ve indirim uygulayarak toplam bilet fiyatını hesaplamak için kullanılabilir.

## Fonksiyon: `bilet_fiyati_hesapla`

### Parametreler:
- `bilet_fiyati` (float): Bir yolcunun bilet fiyatı. Örneğin, 100 TL gibi.
- `yolcu_sayisi` (int): Toplam yolcu sayısı.
- `mesafe` (float, opsiyonel): Gidilen mesafe (kilometre cinsinden). Bu parametre verilirse, mesafe başına ek ücret eklenir. Varsayılan değer `None`'dır.
- `indirim_orani` (float, opsiyonel): Uygulanacak indirim oranı. Yüzde cinsinden belirtilir. Varsayılan değer `0`'dır.

### Açıklama:
- Program, verilen bilet fiyatı ve yolcu sayısına göre toplam bilet fiyatını hesaplar.
- Eğer indirim oranı (`indirim_orani`) belirtilmişse, bu oran üzerinden bir indirim uygulanır.
- Eğer mesafe (`mesafe`) verilmişse, mesafe başına ek bir ücret (kilometre başına 0.10 TL) eklenir.
- Son olarak, tüm hesaplamalar sonucunda toplam bilet fiyatı döndürülür.

### Örnek Kullanım:

```python
bilet_fiyati = 100  # 100 TL bilet fiyatı
yolcu_sayisi = 2
mesafe = 300  # 300 km
indirim_orani = 10  # %10 indirim

toplam_fiyat = bilet_fiyati_hesapla(bilet_fiyati, yolcu_sayisi, mesafe, indirim_orani)
print(f"Toplam Bilet Fiyati: {toplam_fiyat} TL")
```

### Çıktı:
```
Toplam Bilet Fiyati: 610.0 TL
```

## Kullanım Açıklaması:
1. `bilet_fiyati` parametresiyle her bir yolcunun bilet fiyatı belirlenir.
2. `yolcu_sayisi` ile toplam yolcu sayısı belirtilir.
3. `mesafe` ile mesafe girildiğinde, her kilometre için 0.10 TL ek ücret uygulanır.
4. `indirim_orani` ile belirtilen indirim yüzdesi, toplam fiyat üzerinden hesaplanır.

Bu fonksiyon, seyahat organizasyonları, turizm sektöründeki şirketler veya bilet satışları yapan işletmeler için faydalı olabilir.
