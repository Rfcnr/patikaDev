# patika.dev
PatikaDev Proje ödevleri

## Veri Yapıları ve Algoritmalar
## Sıralama Algoritmaları
### Proje 1-B Seçmeli Sıralama (Selection Sort)
`[7, 3, 5, 8, 2, 9, 4, 15, 6]` **-> Selection Sort**

### 1. Yukarı verilen dizinin seçmeli sıralama (selection sort) türüne göre ilk 4 aşaması nasıl gerçekleşir?

1.  |7, 3, 5, 8, **2**, 9, 4, 15, 6 -> birinci elemandan itibaren dizideki en küçük sayı (2) bulunur ve birinci sıradaki elemanla (7) yerleri değiştirilir.
2.  2,| **3**, 5, 8, 7, 9, 4, 15, 6 -> ikinci elemandan itibaren dizideki en küçük sayı (3) bulunur ve zaten ikinci sırada olduğu için aynı yerinde kalır.
3.  2, 3,| 5, 8, 7, 9, **4**, 15, 6 -> üçüncü elemandan itibaren dizideki en küçük sayı (4) bulunur ve üçüncü sıradaki elemanla (5) yerleri değiştirilir.
4.  2, 3, 4,| 8, 7, 9, **5**, 15, 6 -> dördüncü elemandan itibaren dizideki en küçük sayı (5) bulunur ve dördüncü sıradaki elemanla (8) yerleri değiştirilir.
5.  Dört aşama sonrasında dizinin son hali **2, 3, 4, 5,| 7, 9, 8, 15, 6** şeklindedir ve ilk dört eleman sıralanmış durumdadır.