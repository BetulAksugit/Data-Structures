# Proje 2

### [16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
*  Bir listeyi her adımda parçaya ayırıp tek eleman kalıncaya kadar bölüyor. Böldükten sonra sıralı bir şekilde bize sunuyor

* İlk olarak tek eleman kalana kadar diziyi 2'ye bölelim.

|  |  |  |  |  |  |  |  |  |  |  |  |
|- |- |- |- |- |- |- |- |- |- |- |- |
|  |  |  |16|21|11|8 |12|22|  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |16|21|11|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |21|11|  |  |  |8 |12|  |22|  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |21|  |11|  |  |8 |  |12|  |22|

* Ardından ikili sıraları birleştirerek artan sıralamaya göre düzenliyoruz. 

|  |  |  |  |  |  |  |  |  |  |  |  |
|- |- |- |- |- |- |- |- |- |- |- |- |
|16|  |21|  |11|  |  |8 |  |12|  |22|
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |21|11|  |  |  |8 |12|  |22|  |
|  |  |11|16|21|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |8 |11|12|16|21|22|  |  |  |

2. Big-O gösterimini yazınız.
    *  Best case    : O(n*logn)
    *  Average case : O(n*logn)
    *  Worst case   : O(n*logn)