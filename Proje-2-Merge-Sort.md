# Proje-2
### [16,21,11,8,12,22] -> Merge Sort

#### 1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
###### Tek eleman kalana kadar dizimizi 2'ye bölüyoruz.

|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|-----------------------------------------------  |- |- |- |- |- |- |- |- |- |- |- |- |
|Diziyi ikiye bölerek yeniden yazıyoruz           |  |  |  |16|21|11|8 |12|22|  |  |  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|Sol ve sağdaki dizileri tekrar ikiye böluyoruz.  |  |  |16|21|11|  |  |8 |12|22|  |  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|Tek eleman kalana kadar bir kez daha bölüyoruz.  |  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|                                                 |16|  |21|  |11|  |  |8 |  |12|  |22|


######  Tek elemanlı dizilerimizi elde ettikten sonra birleştirme (merge) aşamasına geçiyoruz. Bu aşamada birleştirirken elemanları sıralayarak birleştiriyoruz.

|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|----------------------------------------------- |- |- |- |- |- |- |- |- |- |- |- |- |
|                                                |16|  |21|  |11|  |  |8 |  |12|  |22|
|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|ikili ikili ikili sıralayarak birleştiriyoruz.  |  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|Tekrar ikili ikili sıralayarak birleştiriyoruz. |  |  |11|16|21|  |  |8 |12|22|  |  |
|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|Son birleştirmede dizimizi elde ediyoruz.       |  |  |  |8 |11|12|16|21|22|  |  |  |
    

#### 2. Big-O gösterimini yazınız.
Sürekli diziyi 2'ye böldüğü için $ O(logn) $ ve bu işlemi dizinin büyüklüğü olan $ n $ defa yaptığı için Big-O gösterimi $ O(nlogn) $ olmaktadır.
