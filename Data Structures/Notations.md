3 əsas asymptotic notation mövcuddur:

1. Big-O Notation (O-notation)
2. Omega Notation (Ω-notation)
3. Theta Notation (Θ-notation)

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
