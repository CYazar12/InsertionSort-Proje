# [22,27,16,2,18,6]

# Yukarı verilen dizinin Insertion Sort türüne göre aşamalarını yazıyoruz.

## Ilk olarak listeyi tariyoruz  dizinin en kücük elemanini yerini en ön deki sayiyla yer degistiriyoruz

### [2,27,16,22,18,6]  // 2 ile 22 nin yerini degistirdik. 2 artik basta ve sabit.

### [2,6,16,22,18,27]  // 6 ile 27 nin yerini degistiriyoruz ve artik 2 ve 6 sabit.

### [2,6,16,22,18,27]  // 16 listenin geri kalanin en kücük elemani dolayisiyla artik 2, 6, 16  listenin önünde sabitleniyor.

### [2,6,16,18,22,27] // 18 ile 22 yer degistiriyor

### [2,16,18,22,27] // 22 zaten 27 den kücük , liste dogru bir sekilde diziliyor.

## Big-O gösterimi
### [22,27,16,2,18,6]

### [2| 27,16,22,18,6] n tane karsilastirma yapildi 

### [2,6|,16,22,18,27] (n-1) tane karsilastirma yapildi

### [2,6,16|,22,18,27] (n-2) tane karsilastima yapildi 

### [2,6,16,18|,22,27] (n-3) tane karsilastirma yapildi

### [2,16,18,22|,27] (n-4) tane karsilastirma yapildi

### n+(n-1)+(n-2) …..+1 = (n^2-n)/2 ∈ O(n²) dir

## Big O fonksiyonu katsayilardan bagimsiz ve dominat degeri baz alir bu durumda Big -O : O(n²)
 
	* Worst case *: Aradığımız sayının sonda olması =   (n^2-n)/2 ∈ O(n²) dir 


   * Average case *: Aradığımız sayının ortada olması ==   (n^2-n)/4 ∈ O(n²) dir


    * Best case *: Bu algoritma için en iyi ihtimalle başlangıçta dizinin sıralı olmasıdır. 
    
    Böylelikle hiç yer değiştirme yapmadan sıralama bitecektir. O(n )


## 18 sayısı average case kapsamındadır.

##  [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

### [2|,3,5,8,7,9,4,15,6]

### [2,3,| 5,8,7,9,4,15,6]

### [2,3,4| ,8,7,9,5,15,6]

### [2,3,4,5| 7,9,8,15,6]

