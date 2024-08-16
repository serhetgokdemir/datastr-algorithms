# Problem:
[22,27,16,2,18,6] -> Insertion Sort
A-) Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

B-) Big-O gösterimini yazınız.

C-) Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız
* Average case: Aradığımız sayının ortada olması
* Worst case: Aradığımız sayının sonda olması
* Best case: Aradığımız sayının dizinin en başında olması.

D-) [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

-----------------------
A-)
1. 27, 22'den büyüktür. Değişim olmaz. Sonraki adıma geçilir.
2. 16, 27'den küçüktür. 16 ile 27 yer değiştirir. 16, 22'den küçüktür. 16 ile 22 yer değiştirir.
[16,22,27,2,18,6]
3. 2, 27'den küçüktür, yer değiştirirler. 2, 22'den küçüktür, yer değiştirirler. 2, 16'dan küçüktür, yer değiştirirler.
[2,16,22,27,18,6]
4. 18, 27'den küçüktür yer değiştirirler. 18, 22'den küçüktür yer değiştirirler. 18, 16'dan büyüktür yer değiştirmezler sabit kalırlar.
[2,16,18,22,27,6]
6. 6; 27,22,18,16'dan küçüktür. Hepsiyle sırasıyla yer değiştirir. En sonunda 2'den büyüktür ve orada kalır. Listenin son hali, sort edilmiş hali şöyledir:
[2,6,16,18,22,27]
------------------------
B-)O(m^2)
------------------------
C-)Average Case
------------------------
D-)[7,3,5,8,2*,9,4,15,6] = En küçük eleman 2'dir.
[2,3,5,8,7,9,4,15,6]
[2,3,5,8,7,9,4*,15,6]
[2,3,4,8,7,9,5,15,6]
[2,3,4,8,7,9,5*,15,6]
[2,3,4,5,7,9,8,15,6]
....
....

