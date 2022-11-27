# patika.dev
PatikaDev Proje ödevleri

## Veri Yapıları ve Algoritmalar
## Sıralama Algoritmaları
### Proje 1-A Eklemeli Sıralama (Insertion Sort)
`[22,27,16,2,18,6]` **-> Insertion Sort**

### 1. Yukarı verilen dizinin eklemeli sıralama (inserion sort) türüne göre aşamaları nelerdir?
   1.  -> **22, 27**, 16, 2, 18, 6 -> ilk sayımız (22) bir sonraki sayımızdan (27) küçüktür, ikisi de yerinde kalır.
   2.  -> 22, **27, 16**, 2, 18, 6 -> ikinci sayımız (27) bir sonraki sayımızdan (16) büyüktür, yerleri değiştirilir.
   3.  -> **22, 16**, 27, 2, 18, 6 -> yeni ikinci sayımız (16) bir önceki sayımızdan da (22) küçüktür, yerleri değiştirilir.
   4.  -> 16, 22, **27, 2**, 18, 6 -> üçüncü sayımız (27) bir sonraki sayımızdan (2) büyüktür, yerleri değiştirilir.
   5.  -> 16, **22, 2**, 27, 18, 6 -> yeni üçüncü sayımız (2) bir önceki sayımızdan da (22) küçüktür, yerleri değiştirilir.
   6.  -> **16, 2**, 22, 27, 18, 6 -> yeni ikinci sayımız (2) bir önceki sayımızdan da (16) küçüktür, yerleri değiştirilir.
   7.  -> 2, 16, 22, **27, 18**, 6 -> dördüncü sayımız (27) bir sonraki sayımızdan (18) büyüktür, yerleri değiştirilir.
   8.  -> 2, 16, **22, 18**, 27, 6 -> yeni dördüncü sayımız (18) bir önceki sayımızdan da (22) küçüktür, yerleri değiştirilir.
   9.  -> 2, 16, 18, 22, **27, 6** -> beşinci sayımız (27) bir sonraki (sonuncu) sayımızdan (6) büyüktür, yerleri değiştirilir.
   10. -> 2, 16, 18, **22, 6**, 27 -> yeni beşinci sayımız (6) bir önceki sayımızdan da (22) küçüktür, yerleri değiştirilir.
   11. -> 2, 16, **18, 6**, 22, 27 -> yeni dördüncü sayımız (6) bir önceki sayımızdan da (18) küçüktür, yerleri değiştirilir.
   12. -> 2, **16, 6**, 18, 22, 27 -> yeni üçüncü sayımız (6) bir önceki sayımızdan da (16) küçüktür, yerleri değiştirilir.
   13. -> 2, **6**, 16, 18, 22, 27 -> yeni ikinci sayımız (6) bir önceki sayımızdan (2) büyüktür, **sıralama tamamlanır.**



### 2. Big-O gösterimi
Eklemeli sıralamanın (insertion sort) **Worst-Case** performansı **O(n2)**’dir.
Bunun sebebi dizideki eleman sayısı kadar geçiş gerekmesi ve her geçişte en kötü ihtimalle eleman sayısı kadar kaydırma gerekmesidir.
Daha açık ifade etmek gerekirse eklemeli sıralamanın en kötü durumu tersten sıralı bir listedir.
Eklemeli sıralamanın en iyi ihtimali ise zaten sıralı olan bir listedir ve dizinin eleman sayısı kadar işlem yapılacağından
**Best-Case** performansı **O(n)**'dir. Yukarıda verilen `[22,27,16,2,18,6]` karışık dizinin performası ise **Avarage-Case**
kapsamındadır ve **O(2n)**' dir.

### 3. Time Complexity
*Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?*

`2, 6, 16, 18, 22, 27` şeklinde sıralanan dizide 4. eleman olan **18** sayısı  ortalarda olduğundan **Avarage Case** kapsamındadır.

`Average case:` Aradığımız sayının dizinin ortasında olması durumudur.

`Worst case:` Aradığımız sayının dizinin en sonunda olması ya da dizide öyle bir sayı olmaması durumudur.

`Best case:` Aradığımız sayının dizinin en başında olması durumudur.