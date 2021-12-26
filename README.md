# Insertion-Sort-Algorithm
Insertion Sort Algorithm was applied to a 6-element array and efficiency of the algorithm was examined.

[22,27,16,2,18,6] -> Insertion Sort

1- Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

2- Big-O gösterimini yazınız.

3- Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.

4- Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


1- Insertion Sort algoritmasının çalışma mekanizması şu şekildedir; içinde n tane eleman olan kümeyi küçükten büyüğe sıralamak ister. Bu sıralamayı her adımda en küçük elemanı bulup en başa göndererek yapmaktadır.

  n: [22,27,16,2,18,6] #ilk adım olarak dizinin bütün elemanlarını tarıyoruz. Taradıktan sonra en küçük eleman olarak "2" bulunur. Daha sonra en küçük elemanımızı listenin başına atmak için "22" ve "2" nin yerini değiştiririz.

n-1: [2,27,16,22,18,6] #oluşacak dizi bu şekildedir. Baştaki elemanımız dışında tekrar tarama yaptığımız zaman bu sefer bir küçük elemanımız "6"dır ve "27" ile yer değişir.

n-2: [2,6,16,22,18,27] #oluşacak dizi bu şekildedir. "2" ve "6" dan sonra en küçük elemanımız "16"dır ve yerindedir. Bu sefer "2", "6" ve "16"dan sonraki en küçük elemanımızı aramamız gerekir. Bu eleman "8"dir ve "22"ile yer değişir.

  1: [2,6,16,18,22,27] #bu işlemlerimizin son adımıdır ve görüldüğü gibi bütün elemanlar küçükten büyüğe doğru sıralanmıştır. 
  
  
 2- Big-O Notation:
 
 
