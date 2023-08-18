#  PROJECT 2
## Merge Sort
Soru 1 : [16,21,11,8,12,22]  Bu dizinin sort türüne göre aşamalarını yazınız.Merge Sort

--------------------------
Cevap 1: Diziyi her seferinde iki grup olarak parçalıyoruz. Parçalanan dizileri de iki grup olarak parçalıyoruz, ta ki tek elemanlı olana kadar. Sonra tekrar parçaladığımız grupları birleştiriyoruz. Her grubu birleştirmeden önce kendi içinde sıralıyoruz, sonra iki diziyi birleştirirken sıralıyoruz. Son olarak soldan sağa doğru küçükten büyüğe elemanlar dizinin içinde sıralanmış oluyor.

[16,21,11,8,12,22]

[16,21,11]<--->[8,12,22]

[16]<--->[21,11]<--->[8]<--->[12,22]

[16]<--->[21]<--->[11]<--->[8]<--->[12]<--->[22]

[16]<--->[11,21]<--->[8]<--->[12,22]

[11,16,21]<--->[8,12,22]

[8,11,12,16,21,22]

----------------------------------

Soru 2: Big-O gösterimini yazınız.

------------------------------------------------
Cevap 2:

" Merge Sort, bir "böl-ve-fethet" (divide and conquer) algoritmasıdır. Aşağıda Merge Sort'un O(n*logn) zaman karmaşıklığını açıklayan adımları bulabilirsiniz:

Bölme (Divide) Adımı: Verilen diziyi ortadan ikiye böleriz. Bu işlem log(n) adımda gerçekleşir, çünkü her seferinde dizi ikiye bölünür.

Fethetme (Conquer) Adımı: Bölünmüş dizileri tekrar tekrar bölerek (rekürsif olarak) en küçük parçalara (genellikle tek elemanlı veya boş dizilere) ulaşırız. Bu adımda her alt dizinin sıralanması O(1) zaman alır.

Birleştirme (Merge) Adımı: Sıralı alt dizileri birleştirerek, her bir birleştirme adımında iki alt diziyi birleştirir ve sıralı bir alt dizi oluştururuz. Bu birleştirme işlemi, alt dizilerin toplam eleman sayısı kadar zaman alır. Tüm alt diziler birleştirilene kadar bu adım tekrarlanır.

Birleştirme adımı, iki sıralı alt diziyi birleştirirken elemanları karşılaştırır ve sıralı bir şekilde birleştirir. Bu işlem, her alt dizi için O(n) zaman alır. Toplamda, bölme adımında log(n) kez bölündüğü için birleştirme adımı O(n*logn) zaman karmaşıklığına sahiptir.

Sonuç olarak, bölme adımının log(n) zaman aldığını ve birleştirme adımının O(nlogn) zaman aldığını düşündüğümüzde, Merge Sort'un toplam zaman karmaşıklığının O(nlogn) olduğunu söyleyebiliriz. "