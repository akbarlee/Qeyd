Asymptotic notasya nədir?: 
 Yazılan alqoritmin səmərəliliyi onun icra olunma müddətindən asılıdır. Alqoritmaya daxil edilən məlumatların sayı və çeşidliliyi eyni performans icra etmir.
 Bu səmərəlik  notasyaların köməyi ilə təyin edilir.

3 əsas asymptotic notation mövcuddur:

1. Big-O Notation (O-notation)
2. Omega Notation (Ω-notation)
3. Theta Notation (Θ-notation)
 
 Bubble sort alqoritmasını örnək götürək. Bütün elementlər doğru sıralanıbsa (böyükdən kiçiyə) algoritmin götürdüyü
zaman xətti olacaq O(n) . Əgər elementlər böyükdən kiçiyə doğru sıralanıbsa zaman bölgüsü kvadratik olacaq O(n^2). Bubble sort alqoritmin işləmə prinsipi
aşağıdaki kimidir: 

![Bubble-sort-example-300px](https://user-images.githubusercontent.com/62420106/205504008-86fe75e3-9df3-4726-a7e6-3449c1809382.gif) 

Big O , üst limit ( upper bound )  algoritmin ən pis çalışma müddətini (a worst-run time) təyin edir. Məsələn n ölçüdə listimiz var. Sadə axtarış zamanı
 n qədər vaxt alacaq yəni, Big O notasiyası  O (n) olacaq. Big O notasiyası alqoritmin saniyədə nə qədər sürrətli olacağını demir , icra olunacaq əməliyyatları
 müqayisə edərək ən sürrətli olanı təyin etməyə çalışır.
Məsələn: 
f(n) =4n^2 +2n+4 

 Nəticə:
 
f(1)=4+2+4                    
f(2)=16+4+4        
f(3)=36+6+4      
f(4)=64+8+4   

 n^2 kvadratik olduğu üçün n funksiyası çox böyük qiymətlər aldıqda hər funksiyanın icrası çox böyüyəcək və ləngimələr artaraq gedəcək.
n^2+2n+4 ——–>n^2 Burda n^2 Ən yüksək artım tempi ( highest rate of growth ) sayıldığı üçün 2n+4 görməzdən gəlirik.

Time Complexity (Zaman mürəkkəbliyi) -  İnput/Outputların ölçüsündən asılı olaraq funksiyanın çalışma müddətinin zamana görə azalıb artmasını təyin edir. 3 növü var: 

  Xətti zaman (Linear time) - n qiyməti 0.1n və ya 1000n olsa da fərq olmadan standart ardıcıllıqla artır. Array içində ən böyük və ən kiçik qiyməti tapmağa kömək 
edir.   
```
for (int i = 0; i < n; i++) {
    System.out.println("Nəticə: " + i);
} 
```
  Sabit zaman (Constant time) - n qiyməti çox böyük qiymətlər alsa belə prosesin çalışma müddəti sabit qalır. O(1) ilə işarə olunur.   N’in aldığı qiymət önəm daşımır. Çünki 1 əməliyyat sabit zaman ilə icra olunur. Məsələn:  
int n = 1000; 
System.out.println("Nəticə: " + n); 

  Çoxhədli  zaman  (Polynomial  time) -  n qiyməti artdıqca prosesin icra müddəti eksponensial ( üst qiymət) olaraq artır 
