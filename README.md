# Insertion-Sort-Algorithm
Insertion Sort Algorithm was applied to a 6-element array and efficiency of the algorithm was examined.

[22,27,16,2,18,6] -> Insertion Sort

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

1- Insertion Sort algoritmasının çalışma mekanizması şu şekildedir; içinde n tane eleman olan kümeyi küçükten büyüğe sıralamak ister. Bu sıralamayı her adımda en küçük elemanı bulup en başa göndererek yapmaktadır.

1. adım: [22,27,16,2,18,6] #ilk adım olarak dizinin bütün elemanlarını tarıyoruz. Taradıktan sonra en küçük eleman olarak "2" bulunur. Daha sonra en küçük elemanımızı listenin başına atmak için "22" ve "2" nin yerini değiştiririz.
2. adım: [2,27,16,22,18,6] #oluşacak dizi bu şekildedir. Baştaki elemanımız dışında tekrar tarama yaptığımız zaman bu sefer bir küçük elemanımız "6"dır ve "27" ile yer değişir.
3. adım: [2,6,16,22,18,27] #oluşacak dizi bu şekildedir. "2" ve "6" dan sonra en küçük elemanımız "16"dır ve yerindedir. Bu sefer "2", "6" ve "16"dan sonraki en küçük elemanımızı aramamız gerekir. Bu eleman "8"dir ve "22"ile yer değişir.
4. adım: [2,6,16,18,22,27] #bu işlemlerimizin son adımıdır ve görüldüğü gibi bütün elemanlar küçükten büyüğe doğru sıralanmıştır. 
  
  
 2- Big-O Notation:
 
 Big-O notation'nın amacı algoritmanın verimliliğini ölçmek için bir araçtır. Aşağıdaki grafiğe bakıldığı zaman hangi bölgede algoritmanın verimliliği iyi ya da kötü anlaşılabilir.
 
 ![image](https://user-images.githubusercontent.com/67806354/147411124-e9bcdcc3-94ed-47ec-8bbd-7da32a4a3e15.png)
 
 ***referans (https://medium.com/kodcular/nedir-bu-big-o-notation-b8b9f1416d30)
 
 *Başlangıçta n tane eleman olduğunu varsayalım. 1. sorunun ilk adımında en küçük elemanı bulmak için n tane değeri de taradık, yani burada n işlem yapılmış oldu.
 
 *İkinci adımda en küçük eleman bulundu, artık o eleman listenin en başında ve yeni taramada bu elemanın kontrol edilmesine ihtiyaç yok. Eleman sayısı bu şekilde n-1'e düştü. Sonuç olarak n-1 tane işlem yapılmış oldu.
 
 *Bundan sonraki adımlarda ise eleman sayısı 1'e düşene kadar algoritma taramaya devam edecek ve her adımda eleman sayım bir azalacak.
 
 Sonuç olarak yapılan işlem sayısı şu şekilde olacaktır;
 
 n + (n-1) + (n-2) + .... + 1
 
 Bu işlemler toplandığı zaman;
 
 n*(n+1)/2 = 1/2*(n^2 + n)  toplamına ulaşılır.
 
 Big-O notation'da güçlü olan değerler dikkate alınır, bu örnekte güçlü olan değer n^2 olacaktır. Böylece O(n^2) şeklinde olacaktır.
 
 
 3- Time Complexity:
 
 -Best Case: En iyi durum dizinin küçükten büyüğe sıralı bir halde bulunmasıdır. Algoritma bu durumda sadece bütün elemanları tarar ve hepsinin olmadı gerektiği sırada olduğuna karar verir. Böylece n tane işlem yapılacaktır. Sonuç olarak O(n) best case'i göstermektedir.
 
 -Worst Case: En kötü durum dizideki elemanların istenilen sıranın tam tersi şeklinde sıralı olmasıdır. Bu durumda algoritma her elemanı değiştirmek zorunda kalacağı için n*(n+1)/2 kadar işlem yapacaktır. Sonuç olarak O(n^2) best case'i göstermektedir.
 
 -Average Case: Burada ise en iyi ve en kötü durumun ortalaması alınmaktadır. Sonuç olarak average case için Big-O Notation O(n^2) şeklinde olacaktır.
 
 
 4- [7,3,5,8,2,9,4,15,6] şimdi bu dizinin Insertion Sort algoritmasını referans alarak ilk 4 adımı yazacağız.
 
 1. adım: [2,3,5,8,7,9,4,15,6] 
 2. adım: [2,3,4,8,7,9,5,15,6] 
 3. adım: [2,3,4,5,7,9,8,15,6] 
 4. adım: [2,3,4,5,6,9,8,15,7]
