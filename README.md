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
