# sort algorithms
elimizdeki verileri sıralarken sıralama metoduna göre farklı performanslar elde ederiz.
## insertion sort
birinci elemandan başlayarak dizideki en küçük elemanı dizinin birinci elemanı ile yer değiştirip sonraki eleman dan itibaren dizi sonuna kadar aynı işlemi tekrar ederek yapılan sıralamadır.

### **[22,27,16,2,18,6]** dizisi örneği için;
- **Dizinin sort türüne göre aşamaları.**
[22,27,16, 2,18, 6] 
[ 2,22,27,16,18, 6] 
[ 2, 6,22,27,16,18] 
[ 2, 6,16,22,27,18] 
[ 2, 6,16,18,22,27]
[ 2, 6,16,18,22,27]
[ 2, 6,16,18,22,27]


- **Big-O gösterimi.**
n^2 = 36

- **Time Complexity:**
**En iyi durum  :** O(n)   (Best case: Dizinin sıralı olması durumu)
**En kötü durum :** O(n^2) (Worst case: Aradığımız sayının sonda olması)
**Ortalama      :** O(n^2) (Average case: Aradığımız sayının ortada olması)

- Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? 
## merge sort
sıralanacak diziyi ikiye bölüp kendi içinde sıralı küçük parçaları birleştirme mantığına dayanır.
### **[16,21,11,8,12,22]** dizisi örneği için;
-   Dizinin sort türüne göre aşamaları:
[16,21,11,8,12,22]
[16,21,11]      [8,12,22]
[16]   [21,11]   [8]   [12,22]
[16]   [21,11]   [8]   [12,22]
[16,21,11]   [8,12,22]
[8,12,16,21,11,22]

-   Big-O gösterimi:
On(logn)
