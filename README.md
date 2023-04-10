# selection-sort-proje
----
Selection Sort Nedir?

Selection sort, bir dizi içerisindeki elemanları sıralamak için kullanılan basit bir sıralama algoritmasıdır. Bu algoritma, elemanların doğru konumlarına yerleştirilmesi için karşılaştırma ve değiştirme işlemleri yapar.

İlk olarak, dizinin en küçük elemanı bulunur ve ilk elemanla yer değiştirilir. Daha sonra, ikinci en küçük eleman bulunur ve ikinci elemanla yer değiştirilir. Bu işlem, dizinin tamamı sıralanana kadar devam eder.

Selection sort algoritması, her adımda en küçük elemanı bulmak için tüm diziyi tarar, bu nedenle en iyi durumda bile O(n^2) zaman karmaşıklığına sahiptir. En kötü durumda, dizinin tamamının sıralanması için O(n^2) karşılaştırma ve O(n) yer değiştirme işlemi yapar. Bu nedenle, büyük dizilerde kullanıldığında performansı düşük olabilir. Ancak, küçük dizilerde ve özellikle verilerin neredeyse sıralı olduğu durumlarda oldukça etkilidir.
--------------

[22,27,16,2,18,6] -> Selection Sort
1) Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

 
1. adım: [2, 27, 16, 22, 18, 6] -->  (n tarama)
2. adım: [2, 6, 16, 22, 18, 27] -->  (n-1)
3. adım: [2, 6, 16, 22, 27, 18] -->  (n-2)
4. adım: [2, 6, 16, 18, 27, 22] -->  (n-3)
5. adım: [2, 6, 16, 18, 22, 27] -->  (n-4)
-------------

Insertion sort nedir?

Insertion sort, bir dizi içerisindeki elemanları sıralamak için kullanılan bir sıralama algoritmasıdır. Bu algoritma, elemanların yer değiştirme işlemleri yaparak doğru konumlarına yerleştirilmesiyle sıralama yapar.

Insertion sort algoritması, ilk elemanın doğru konumunda olduğunu varsayar ve sonraki elemanların sıralama yapılacak kısmı içinde uygun pozisyonuna yerleştirilmesiyle sıralama yapar. Bu nedenle, sıralama işlemi bir dizi oluşturur: sıralı kısım ve sıralanmamış kısım. Her adımda, sıralanmamış kısmın ilk elemanı, sıralı kısım içindeki doğru pozisyona yerleştirilir.

Örneğin, verilen bir diziyi sıralamak istediğimizde, ilk eleman doğru pozisyonda olduğu varsayılır. İkinci eleman, ilk elemanla karşılaştırılır ve doğru konuma yerleştirilir. Üçüncü eleman, sıralı kısım içindeki uygun pozisyona yerleştirilir. Bu işlem, dizinin son elemanına kadar devam eder ve sonuçta sıralı bir dizi elde edilir.

Insertion sort algoritması, en iyi durumda O(n) zaman karmaşıklığına sahiptir, yani dizinin zaten sıralı olması durumunda en hızlı şekilde işlem yapar. Ancak en kötü durumda O(n^2) zaman karmaşıklığına sahip olabilir, yani dizinin tamamı ters sıralı olduğunda en yavaş şekilde işlem yapar.

1. [22, 27, 16, 2, 18, 6]
2. [22, 27, 16, 2, 18, 6] -> [22, 27, 16, 2, 18, 6]
3. [16, 22, 27, 2, 18, 6]
4. [2, 16, 22, 27, 18, 6]
5. [2, 16, 18, 22, 27, 6]
6. [2, 6, 16, 18, 22, 27]
---
Verilen dizi [22, 27, 16, 2, 18, 6] üzerinde sıralama yapmak için kullanılan Insertion Sort veya Selection Sort gibi temel sıralama algoritmalarının Big-O gösterimi O(n^2)'dir.

Bu, algoritmanın en kötü durumda n^2 adım atabileceği anlamına gelir. En iyi durumda (örneğin dizi zaten sıralıysa), bazı sıralama algoritmaları O(n) zaman karmaşıklığına sahip olabilir. Ancak, Insertion Sort ve Selection Sort, her durumda n^2 adım atabilen algoritmalar olduğundan Big-O gösterimi O(n^2) olarak ifade edilir.
----

Verilen diziyi Selection Sort algoritması kullanarak sıralamak istediğimizde ilk 4 adım şu şekilde olacaktır:

1. [7, 3, 5, 8, 2, 9, 4, 15, 6] -> En küçük eleman 2 olduğu için 2 ile ilk elemanı yer değiştir.
   [2, 3, 5, 8, 7, 9, 4, 15, 6]

2. [2, 3, 5, 8, 7, 9, 4, 15, 6] -> En küçük eleman 3 olduğu için 3 ile 2. elemanı yer değiştir.
   [2, 3, 5, 8, 7, 9, 4, 15, 6]

3. [2, 3, 5, 8, 7, 9, 4, 15, 6] -> En küçük eleman 4 olduğu için 4 ile 3. elemanı yer değiştir.
   [2, 3, 4, 8, 7, 9, 5, 15, 6]

4. [2, 3, 4, 8, 7, 9, 5, 15, 6] -> En küçük eleman 5 olduğu için 5 ile 4. elemanı yer değiştir.
   [2, 3, 4, 5, 7, 9, 8, 15, 6]
