# Proje 1 Insertion Sort

## [22,27,16,2,18,6] -> Insertion Sort

* Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.
    1. Dizinin en küçük elemanını bul ve ilk elemanla yer değiştir.

        ### [ ***22*** , 27 , 16, ***2*** , 18 , 6 ] -> [ ***2*** , 27 , 16 , ***22*** , 18 , 6 ]
    
    2. Dizinin 2. elemanından itibaren dizinin en küçük elemanını bul ve 2.eleman ile yer değiştir. 

        ### [ 2 | , ***27*** , 16 , 22 , 18 , ***6*** ] -> [ 2 | , ***6*** , 16 , 22 , 18 , ***27*** ]

    3. Dizinin 3.elemanından itibaren dizinin en küçük elemanını bul ve 3. eleman ile yer değiştir. ***16***'dan küçük eleman olmadığı için işlem yapma. Algoritma bu şekilde devam eder.
        ### [ 2 , 6 | , ***16*** , 22 , 18 , 27 ]

    4.  ### [ 2 , 6 , 16 | , ***22*** , ***18*** , 27 ] -> [ 2 , 6 , 16 | , ***18*** , ***22*** , 27 ]
    
    5.  ### [ 2 , 6 , 16 , 18 | , ***22*** , ***27*** ] -> [ 2 , 6 , 16 , 18 | , 22 , 27 ]

    6. ### [ 2 , 6 , 16 , 18 , 22 | , 27 ] Dizinin sıralanmış son hali


*   Big-O gösterimini yazınız.
    $$ O(n^2)