#  PROJECT 3
## Binary Sort

Soru 1: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

* root x'dir. root'un sağından y bulunur. Solunda z bulunur *

----------------------
Cevap 1: Bir elemanı root olarak seçiyoruz. Sonra dizinin solundaki elemandan sağındaki elemana kadar teker teker karşılaştırıyoruz.

Dengeli bir dağılım için root olarak 7 elemanını aldım.

Aşamalar:

Dizinin solundan elemanları teker teker inceliyorum. 7 ile 5 i karşılaştıracağım. 5, 7'den küçük olduğu için sol tarafa yazılır.
            7
           /
          5

Sırada 1 var. 1, 7'den küçük sola, 5'ten küçük sola yerleştirilir.
            7
           /
          5
         /
        1

8, 7'den büyük sağa...
            7
           / \
          5   8
         /
        1

3, 7'nin soluna, 5'in soluna, 1'in sağına...
            7
           / \
          5   8
         /
        1
         \
          3

6, 7'nin soluna, 5'in sağına...
            7
           / \
          5   8
         / \
        1   6
         \
          3

0, 7'nin soluna, 5'in soluna, 1'in soluna...
            7
           / \
          5   8
         / \
        1   6
       / \
      0   3

9, 7'nin sağına, 8'in sağına...
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3

4, 7'nin soluna,5'in soluna, 1'in sağına, 3'ün sağına...
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
           \
            4

2, 7'nin soluna, 5'in soluna, 1'in sağına, 3'ün soluna yazılır.
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
         / \
        2   4 