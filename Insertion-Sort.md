# Proje 1
## [22,27,16,2,18,6] -> Insertion Sort

* Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Insertion sort sıralanmamış dizi elemanlarını tek tek ele alır ve her birini sıralanan parçada doğru konuma yerleştirir.

|1.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|

Dizinin ilk iki elemanı sıralamada karşılaştırılır.
Burada 27, 22'den büyüktür. Her iki öge de artan sırada görünüyor. Herhangi bir değişiklik olmayacak.
|2.Adım|22|27|16|2|18|6|     
|------|- |- |- |-|- |-|

Daha sonra 16 ile 27'yi karşılaştırırız. 16 27'den küçüktür ve sıralı değildir. O yüzden yer değiştiririz. Ardından 16'yı tekrar 22 ile karşılaştırırız ve yine 16 yine 22'den küçüktür.Bu sebeple en başa yazarız.
|3.Adım|22|16|27|2|18|6|-->|16|22|27|2|18|6| 
|------|- |- |- |-|- |-|----|- |- |- |-|- |-|

2 ile bir gerisindeki sayıyı karşılaştırırız. Sıralı değil, yer değiştiririz. Bunu gerisindeki tüm sayılar için yaparız. 
|4.Adım|16|22|2|27|18|6|-->|16|2|22|27|18|6| 
|------|- |- |- |-|- |-|--|- |- |- |-|- |-|

|-->|2|16|22|27|18|6|
|-|- |- |- |-|- |-|

18 ile bir önceki sayıyı kıyaslarız. 18 27'den küçüktür. 27 ile yer değiştiririz. 22 ile 18'i karşılaştırırız. 18 yine küçüktür yer değiştiririz. 16 ile karşılaştırdığımızda doğru artan sırada görünüyor, dolayısıyla değişiklik yapmayız.
|5.Adım|2|16|22|18|27|6|-->|2|16|18|22|27|6|
|------|- |- |- |-|- |-|---|- |- |- |-|- |-|

6 ile bir öncesindeki sayıyı karşılaştırırız ve bunu 6 doğru artan sıraya gelene kadar sıralarız. Sonuç olarak;
|6.Adım|2|16|18|22|6|27|-->|2|16|18|6|22|27|
|------|- |- |- |-|- |-|-------|- |- |- |-|- |-|



* Big-O gösterimini yazınız.
    Best case    : O(n)
    Worst case   : O(n^2)

* Time Complexity: 

Insertion sort performansı O(n^2)’dir. Bunun sebebi dizideki eleman sayısı kadar geçiş gerekmesi ve her geçişte en kötü ihtimalle eleman sayısı kadar kaydırma gerekmesidir. Yani insertion sort’un en kötü durumu tersten sıralı bir listedir. Yukarıdaki örnek için;
     - Worst case: [27, 22, 18, 16, 6, 2]  -> n^2
     - Best case: [2, 6, 16, 18, 22, 27] -> n  


* Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

Dizi sıralandıktan sonra 18 veri setinin ortasında olduğu için average case kapsamına girer.


####  [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
|1.Adım|7|3|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |2.Adım|3|7|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |3.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |4.Adım|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
