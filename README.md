# Insertion Sort
Soru 1: [22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

--------------------------------------------

Cevap 1 :Karşılaştırma işlemine ikinci elemandan başlanılır. "*" işareti olan elemanlar soldaki elemanlarla tek tek karşılaştırılır. Soldakinden küçük ise yer değiştirirler. Bu işlem seçilen eleman soldaki sayıdan büyük olana kadar devam eder.

İşlem bittiğinde seçildiğinde kaçıncı elemansa sonraki eleman karşılaştırma için seçilir.

[22, 27*, 16, 2, 18, 6] -> Aynı kalır, sağdaki diğer elemanın karşılaştırma işlemine geçilir.
[22, 27, 16*, 2, 18, 6] -> [16, 22, 27, 2, 18, 6]
[22, 27, 16, 2*, 18, 6] -> [2, 16, 22, 27, 18, 6]
[2, 16, 22, 27, 18*, 6] -> [2, 16, 18, 22, 27, 6]
[2, 16, 18, 22, 27, 6*] -> [2, 6, 16, 18, 22, 27]

-------------------------------------------------
Soru 2 : BIG O gösterimini yazınız.

--------------------------------------------

Cevap 2: Eleman sayısı n olduğunda, her eleman için en fazla (n-1) karşılaştırma yapılır. Algoritmanın tüm elemanlarını bu şekilde işlemesi gerektiğinde, toplam karşılaştırma sayısı (n-1) + (n-2) + ... + 1 olur, ki bu toplam (n * (n-1) / 2)'ye eşittir.

Big-O gösterimi için en yüksek dereceli terimi göstermemiz lazım. Onun için formülden (n^2) geldiği için gösterimi O(n^2) olur.

----------------------------------------

Soru 3 : Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.

--------------------------------------------

Cevap 3 : [22,27,16,2,18,6] dizisi sıralandıktan sonra [2,6,16,18,22,27]. 18 sayısıı dizinin ortasında olduğundan "Average Case".

----------------------------------------------

Soru 4 : [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

---------------------------------------------

Cevap 4 : 
[7, 3*, 5, 8, 2, 9, 4, 15, 6] -> [3, 7, 5, 8, 2, 9, 4, 15, 6]
[3, 7, 5*, 8, 2, 9, 4, 15, 6] -> [3, 5, 7, 8, 2, 9, 4, 15, 6]
[3, 5, 7, 8*, 2, 9, 4, 15, 6] -> [3, 5, 7, 8, 2, 9, 4, 15, 6]
[3, 5, 7, 8, 2*, 9, 4, 15, 6] -> [2, 3, 5, 7, 8, 9, 4, 15, 6]
[2, 3, 5, 7, 8, 9*, 4, 15, 6] -> [2, 3, 5, 7, 8, 9, 4, 15, 6]
[2, 3, 5, 7, 8, 9, 4*, 15, 6] -> [2, 3, 4, 5, 7, 8, 9, 15, 6]
[2, 3, 4, 5, 7, 8, 9, 15*, 6] -> [2, 3, 4, 5, 7, 8, 9, 15, 6]
[2, 3, 4, 5, 7, 8, 9, 15, 6*] -> [2, 3, 4, 5, 6, 7, 8, 9, 15]
