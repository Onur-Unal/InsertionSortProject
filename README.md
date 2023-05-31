# InsertionSortProject
Patika Veri Yapıları ve Algoritmalar - Selection Sort Projesi

## Soru
[22, 27, 16, 2, 18, 6] -> Insertion Sort

Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

- Average case: Aradığımız sayının ortada olması
- Worst case: Aradığımız sayının sonda olması
- Best case: Aradığımız sayının dizinin en başında olması.


[7, 3, 5, 8, 2, 9, 4, 15, 6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

## Cevap

[22, 27, 16, 2, 18, 6] -> Insertion Sort

### Yukarıda verilen dizinin sort türüne göre aşamaları:

[22, 27, 16, 2, 18, 6] -> n

En küçük eleman bulunur ve listenin ilk sırasına yerleştirilir. İlk sırada bulunan elemanı silmek istemiyoruz. O yüzden o elemanı taşıdığımız elemanın yerine koyarız (en küçük eleman 2, ilk sırada bulunan 22 ile yer değiştirir). 
[2, 27, 16, 22, 18, 6] -> n-1

En küçük ikinci eleman bulunarak aynı işlem yapılır, ikinci sıraya taşınır (en küçük ikinci eleman 6, ikinci sırada bulunan 27 ile yer değiştirir).
[2, 6, 16, 22, 18, 27] -> n-2

En küçük üçüncü eleman olan 16 sayısı zaten üçüncü sırada olduğu için bir sonraki küçük elemana bakılır (18 ile 22 yer değiştirir). Böylece tüm elemanlar küçükten büyüğe sıralanmış olur.
[2, 6, 16, 18, 22, 27] -> 1

### Big O gösterimi:

n + (n-1) + (n-2) + ... + 1 = (n.(n+1)) / 2 = (n^2 + n) / 2

Domine eden karater alınır ve katsayısı olan 1/2 yazılmaz.

O(n^2) şeklindedir.

### Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer ?

[2, 6, 16, 18, 22, 27] dizi küçükten büyüğe yanda verilen şekilde sıralandıktan sonra 18 sayısı ortada yer alamaktadır.

Bu nedenle 'average case' kapsamına girer.

### [7, 3, 5, 8, 2, 9, 4, 15, 6] dizisinin Selection Sort'a göre ilk 4 adımı:

[7, 3, 5, 8, 2, 9, 4, 15, 6] -> n

[2, 3, 5, 8, 7, 9, 4, 15, 6] -> n-1

[2, 3, 4, 8, 7, 9, 5, 15, 6] -> n-2

[2, 3, 4, 5, 7, 9, 8, 15, 6] -> n-3

[2, 3, 4, 5, 6, 9, 8, 15, 7] -> n-4

Şeklinde ilk dört sıra küçükten büyüğe göre sıralanıp, yer değiştirerek gerçekleşir.
