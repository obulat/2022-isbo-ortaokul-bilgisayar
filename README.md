# 2022-isbo-ortaokul-bilgisayar
2022 İstanbul Bilim Olimpiyatları Ortaokul Bilgisayar Soruları

# Bilgisayar

1 D
```c
int main() {
    int i = 0;
    int topl = 0;
    for (i = 0; i<12;i++) {
        topl = topl + i;
    }
    printf("%d", topl);
}
```

Yukarıdaki programın çıktısı şıklardan hangisinde doğru olarak verilmiştir?

A 36
B 42
C 55
D 66
E 78

2 B
```c
int main() {
    printf("%d", !3 + !2 + !1 + !0);
}
```
Yukarıdaki programın çıktısı şıklardan hangisinde doğru olarak verilmiştir?
A 0
B 1
C 2
D Derleme hatası verir
E Çalışma hatası verir

3 A

```c
int main() {
    char str[] = "abcISBOdef!";
    char res[256];
    int i = 0;
    do {
        res[i] = str[i] >= 'a' &&
        str[i] <= 'z' && i & 1
        ? str[i] + 'A' - 'a' : str[i];
    } while (str[i++]);
    printf("%s\n", res);
}
```
A aBc+dEf!
B abc-def+
C AbC+DeF!

4 B

```c
int main() {
    int a = 5;
    int b = 20;
    int c = 2*a-b;
    switch(c) {
        case -35:
        printf("0");
        case -10:
        printf("1");
        break;
        case 0:
        printf("2");
        case 10:
        printf("3");
        default: 
        printf("4");
    }
    return 0;
}
```

Yukarıda verilen programın çıktısı ne olur?

A 0
B 1
C 23
D 34
E 4

5 B
```c
int main() {
    char *dizi[3] = { "matematik", "bilgisayar", "fizik"};
    int i,j;
    int a = 1;
    for (i = 0; i < 5; i ++) {
        if (dizi[0][i] == dizi[1][i] ||
        dizi[1][i] == dizi[2][i] ||
        dizi[0][i] == dizi[2][i]) {
            a = a*2;
        }
    }
    printf("%d", a);
    return 0;
}
```
Yukarıda verilen programın çıktısı ne olur?
A 1
B 2
C 4
D 8
E 16

6 A
```c
int main(){
    double a = 11/2 +5/2.0 + 3/12 +  3.0;
    printf("%lf", a);
}
```
Yukarıda verilen program çıktı olarak ne üretir?
A 10.5
B 11
C 11.25
D 12
E Hiçbiri


7 C
```c
int main()
{
    int a = 0, b = 0, c = 0;
    int i;
    for (i = 0; i < 1000; i++) {
        if (i % 3 == 0) {
            a += 1;
        }
        if (i % 5 == 0) {
            b += 1;
        }
        if (i % 15 == 0) {
            c += 1;
        }
    }
}
```
Yukarıdaki programın çıktısı ne olur?
A 324
B 420
C 467
D 511
E 559

8 A
```c
int main() {
    char a[8] = "istanbul";
    char b[5] = "bilim";
    char c[13] = "olimpiyatlari";
    printf("%c%c%c", a[0]-32, b[0]-32, c[0]-32);
    return 0;
}
```
Yukarıda verilen program çıktı olarak ne üretir?

9 A

```c
inf func(int x) {
    return x%2 ? x++ : --x;
}
int main() {
    int i = 0, p = 0;
    while (i < 10) {
        p = p + func(i);
        i++;
    }
    printf("%d", p);
    return 0
}
```
Yukarıdaki programın çıktısı ne olur?
A 40
B 41
C 43
D 45
E 50

10 B

```c
int f(int x) {
    int a = 0;
    for(int i = 1; i <= x; i++) {
        if (x%i == 0) {
            a = a + 1;
        }
    }
}
return a;
}
```
Yukarıda verilen fonksiyonun amacı ne olabilir?
A Bir sayının asal bölenlerin sayısını bulmak
B Bir sayının pozitif bölenlerin sayısını bulmak
С Bir sayının bölenlerinin toplamını bulmak
D Bir sayının karesinin pozitif bölenlerinin sayısını bulmak
E Bir sayının çift bölenlerinin sayısını bulmak

# Matematik

1 C
$\frac{(2^6 - 3^2)(2^6 + 3^2)}{5}$ işleminin sonucu aşağıdakilerden hangisidir?
A 403
B 603
C 803
D 1003
E 1203

2 E
Mahpeyker'in kitaplığının her bir rafında, raf sayısının iki katı kadar kitap bulunuyor. Kitaplarının sayısı 1800 olan Mahpeyker'in kitaplıgında kaç raf vardır?

A 9
B 15
C 18
D 24
E 30

3 A
Bir kutuda 12 kırmızı 28 mavi bilye, bir torbada 18 kırmızı 22 mavi bilye vardır. Kutudan ve torbadan birer tane bilye seçiliyor. İki bilyenin de kırmızı olma ihtimali $a/b$ sadeleşmeyen kesrine eşittir. Buna göre $a + b$ kaçtır?

A 227
B 229
C 230
D 231
E 232

4 B
Rakamlar kümesinin alt kümelerinin kaç tanesinde 5 bulunur, 3'ün katı bulunmaz?
A 16
B 32
C 64
D 128
E Hiçbiri

5 D
Ahmet ardışık beş sayı belirliyor ve bu sayıların 7 ile bölünmesinden elde edilen kalanları topluyor. Elde ettiği toplamı tahtaya yazan Ahmet yine ardışık beş sayı belirleyip benzer şekilde elde ettiği toplamı tahtaya yazıyor. Mümkün olan tüm fraklı toplamları elde edene kadar böylece devam ediyor.

Ahmet tahtaya kaç farklı sayı yazmıştır?
A 3
B 4
C 6
D 7
E Sonsuz çoklukta

6 B

Ahmet ardışık beş sayı belirliyor ve bu sayıların 7 ile bölünmesinden elde edilen kalanları topluyor. Elde ettiği toplamı tahtaya yazan Ahmet yine ardışık beş sayı belirleyip benzer şekilde elde ettiği toplamı tahtaya yazıyor. Mümkün olan tüm fraklı toplamları elde edene kadar böylece devam ediyor.

Ahmet'in tahtaya yazdığı sayılar arasında en fazla kaç tane ardışık sayı vardır?

A 2
B 3
C 4
D 5
E Sonsuz Çoklukta

7 B

2022'den küçük ve 11'in tam katı olan pozitif sayıların kaç tanesi 5 ile tam bölünür?
A 32
B 36
C 40
D
44
E 48

8 B
$10^n - 1$ sayısının rakamları toplamı 2025 olduğuna göre $n$ kaçtır

A 222
B 225
C 252
D 255
E Hiçbiri

9
Bir $\mathbb{O}$ öperatörü, sıfırdan farklı $x,y$ sayıları verildğiğnde bu sayıların kareleri toplamının bu sayıların çarpımına bölüyor ve sonuç $\mathbb{O}_{x,y}$ ile gösteriliyor. Başka bir  $\mathbb{O}'$ operatörü sıfırdan faklı $x, y$ sayıları verildiğinde bunların toplamlarının karesini alıyor ve sonuç $\mathbb{O}'_{x,y}$ ile gösteriliyor.
Buna göre, $\frac{mathbb{O}'_{x,x}}{mathbb{O}_{y,y}+2}$ ifadesi 72,242,625,2022,20000 sayılarından kaç tanesine eşit olamaz?

10
Bir satranç tahtasından ne ortak kenarı ne ortak köşesi olan iki kare kaç farklı şekilde seçilebir?

A 1806
B 1828
C 1836
D 1874
E 1898
