# InsertionSortProject

### Insertion Sort Aşamaları (Dizi: [22,27,16,2,18,6])

Insertion Sort algoritması, her elemanı bir önceki sıralı diziye ekleyerek sıralama işlemi gerçekleştirir. Aşamalar şu şekildedir:

1. İlk eleman zaten sıralı kabul edilir: **[22]**
2. İkinci eleman 27, 22'den büyük olduğu için yer değiştirmez: **[22,27]**
3. Üçüncü eleman 16, 27'den küçük olduğu için önce onunla, sonra 22 ile karşılaştırılarak öne alınır: **[16,22,27]**
4. Dördüncü eleman 2, 16'dan küçük olduğu için en başa alınır: **[2,16,22,27]**
5. Beşinci eleman 18, 22'den küçük ama 16'dan büyük olduğu için aralarına yerleştirilir: **[2,16,18,22,27]**
6. Son eleman 6, 16'dan küçük olduğu için aralarına yerleştirilir: **[2,6,16,18,22,27]**

### Big-O Gösterimi

- **Big-O Notasyonu (Worst Case)**: Insertion Sort'un en kötü durum zaman karmaşıklığı **O(n²)**'dir, çünkü her eleman için geri dönüp karşılaştırma yapması gerekebilir.
  
### Time Complexity

18 sayısı sıralı dizide ortalarda bulunur (3. indeks). Bu nedenle:
- **Average Case** kapsamına girer.

---

### Selection Sort Aşamaları ([7,3,5,8,2,9,4,15,6])

Selection Sort her adımda en küçük elemanı bulup, sıralı dizinin sonuna ekler.

1. İlk adım: Dizideki en küçük eleman 2, 7 ile yer değiştirilir. **[2,3,5,8,7,9,4,15,6]**
2. İkinci adım: 3 en küçük eleman olarak kalır, yer değiştirmez. **[2,3,5,8,7,9,4,15,6]**
3. Üçüncü adım: 5 en küçük olarak kalır, yer değiştirmez. **[2,3,5,8,7,9,4,15,6]**
4. Dördüncü adım: 4 en küçük elemandır, 8 ile yer değiştirilir. **[2,3,5,4,7,9,8,15,6]**

Bu dört adım sonrasında dizi sıralama işlemine devam eder.

---

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

---

### Binary Search Tree Aşamaları (Dizi: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2])

Verilen diziyi kullanarak Binary Search Tree (BST) oluştururken, her elemanı sırayla ekleyip, küçük olanları sola, büyük olanları sağa yerleştiririz.

1. **Root 7'dir.**
   - Root olarak ilk eleman seçilir: **7**

2. **5, 7'nin solunda bulunur.**
   - 5, 7'den küçük olduğu için soluna yerleştirilir.

3. **1, 5'in solunda bulunur.**
   - 1, 5'ten küçük olduğu için 5'in soluna yerleştirilir.

4. **8, 7'nin sağında bulunur.**
   - 8, 7'den büyük olduğu için sağa eklenir.

5. **3, 1'in sağında bulunur.**
   - 3, 1'den büyük olduğu için 1'in sağına eklenir.

6. **6, 5'in sağında bulunur.**
   - 6, 5'ten büyük olduğu için 5'in sağına eklenir.

7. **0, 1'in solunda bulunur.**
   - 0, 1'den küçük olduğu için 1'in soluna eklenir.

8. **9, 8'in sağında bulunur.**
   - 9, 8'den büyük olduğu için 8'in sağına eklenir.

9. **4, 3'ün sağında bulunur.**
   - 4, 3'ten büyük olduğu için 3'ün sağına eklenir.

10. **2, 3'ün solunda bulunur.**
    - 2, 3'ten küçük olduğu için 3'ün soluna eklenir.

### Sonuçta elde edilen Binary Search Tree yapısı şu şekildedir:

        7
       / \
      5   8
     / \    \
    1   6    9
   / \
  0   3
     / \
    2   4

