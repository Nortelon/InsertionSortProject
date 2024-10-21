# InsertionSortProject

Insertion Sort Aşamaları (Dizi: [22,27,16,2,18,6])
Insertion Sort algoritması, her elemanı bir önceki sıralı diziye ekleyerek sıralama işlemi gerçekleştirir. Aşamalar şu şekildedir:

İlk eleman zaten sıralı kabul edilir: [22]
İkinci eleman 27, 22'den büyük olduğu için yer değiştirmez: [22,27]
Üçüncü eleman 16, 27'den küçük olduğu için önce onunla, sonra 22 ile karşılaştırılarak öne alınır: [16,22,27]
Dördüncü eleman 2, 16'dan küçük olduğu için en başa alınır: [2,16,22,27]
Beşinci eleman 18, 22'den küçük ama 16'dan büyük olduğu için aralarına yerleştirilir: [2,16,18,22,27]
Son eleman 6, 16'dan küçük olduğu için aralarına yerleştirilir: [2,6,16,18,22,27]
Big-O Gösterimi
Big-O Notasyonu (Worst Case): Insertion Sort'un en kötü durum zaman karmaşıklığı O(n²)'dir, çünkü her eleman için geri dönüp karşılaştırma yapması gerekebilir.
Time Complexity
18 sayısı sıralı dizide ortalarda bulunur (3. indeks). Bu nedenle:

Average Case kapsamına girer.


### Merge Sort Aşamaları (Dizi: [16,21,11,8,12,22])

Merge Sort algoritması, bir diziyi sürekli olarak ikiye bölerek en küçük parçalara ayırır, ardından bu parçaları sıralayarak birleştirir. İşte aşamaları:

1. **Diziyi ikiye bölme**: 
   - [16,21,11] ve [8,12,22]

2. **Her iki parçayı tekrar ikiye bölme**:
   - [16,21,11] → [16] ve [21,11]
   - [21,11] → [21] ve [11]
   - [8,12,22] → [8] ve [12,22]
   - [12,22] → [12] ve [22]

3. **Tek elemanlı parçaları sıralama**:
   - [16] → zaten sıralı
   - [21,11] → [11,21] (sıralanır)
   - [8] → zaten sıralı
   - [12,22] → zaten sıralı

4. **Parçaları sıralı şekilde birleştirme**:
   - [16] ve [11,21] → [11,16,21]
   - [8] ve [12,22] → [8,12,22]

5. **İki ana parçayı birleştirme**:
   - [11,16,21] ve [8,12,22] → [8,11,12,16,21,22]

Sonuç olarak sıralı dizi: **[8,11,12,16,21,22]**

### Big-O Gösterimi

Merge Sort'un zaman karmaşıklığı her durumda (best, worst, average case) **O(n log n)**'dir. Bu, diziyi her seferinde ikiye böldüğü ve her aşamada tüm elemanları birleştirdiği için geçerlidir.
