# Praktikum7

## Soal1.cpp 

**Alur Argoritma**

1.Mulai program tersebut
2.Input interger fungsi (int, int)
3.Input interger a dan b dan deskripsikan a=0, dan b=1.
4.Jika nilai suku satu (b) adalah =1 dan jika nilai suku dua (a) adalah =0.
5.Maka cetak rumus fungsi iteratif menggunakan for intruksikan fungsi fibonacci di awali dengan 2 dan di akhiri dengan indexs suku.
6.Deskripsikan variable untuk mencetak fuungsi selanjutnya.
7.Cetak suku fibonacci menggunakan pemanggilan fungsi itertif.

**Pseudecode**

```
1.int typedatar (a, b)
2.if (bil=1) return a
3.if (bil=0) return b
4.for (int i=2; i<=bil; i++)
5.c= a+b, a=b, b=c
6.end
```


**Code Program**
```c++
#include <iostream>

using namespace std;

int iteratif (int bil, int a, int b, int c)
{
a=0, b=1;
if (bil == 1) return b;
if (bil == 0) return a;

else{
for(int i=2; i<=bil; i++){

c = a + b;
a = b;
b = c;
}
return c;
}
}

int main()
{
int bil, a, b,c;

cout<<"Masukkan bilangan deret ke-: ";
cin>>bil;
cout<<"\nBilangan fibonaccinya untuk "<<bil<<" adalah ";
cout<< iteratif ( bil,  a,  b,  c);

return 0;
}
```


Hasil1
![Screenshot](https://raw.githubusercontent.com/putrintans/Praktikum7/master/Soal1/Screenshot1.png)

CMD1
![CMD](https://raw.githubusercontent.com/putrintans/Praktikum7/master/Soal1/CMD1.png)


## Soal2.cpp

**Alur Argoritma**

1.Mulai program tersebut.
2.Input interger fungsi (int a, int b).
3.Jika nilai interger (b==0) return 0.
4.Jika nilai (b>0) intruksikan return a + type data (a, b - 1).
5.Sebaliknya return (-a) + type Data (a, b+1).
6.Masukkan variabel a,b untuk menginput nilai awal dan dibagi degan nilai selanjutnya.
7.Cetak nilai perkalian dengan memanggil fungsi rekursif menggunakan type datanya.

**Pseudecode**

```
deskripsi a x b =
1. 0, untuk b = 0
2. a + (a x (b-1)), untuk b > 0
3. -a + (a x (b + 1)), untuk b < 0
4. end
```


**Code Program**
```c++
#include <iostream>
using namespace std;


int kali_rekursif(int a, int b)
{
 if (b==0)
  return 0;
 else if (b > 0)
  return a + kali_rekursif(a, b - 1);
 else
  return (-a) + kali_rekursif(a, b+1);
}


main()
{
 int a, b;
 cout << "Masukan Bilangan : ";
 cin >> a;
 cout << "Dikli Dengan :";
 cin >> b;
 cout << " AxB = " << kali_rekursif(a, b) << endl;
}
```

Hasil2
![Screenshot](https://raw.githubusercontent.com/putrintans/Praktikum7/master/Soal2/Screenshot2.png)


## Soal3.cpp 

**Alur Argoritma**

1.Mulai program tersebut.
2.Input menggunakan intruksi void dan menggunakan pointer untuk menetapakan void typedata (char s).
3.Jika nilai s!=0--> menggunakan Pointer() maka masukkan intruksi membalik (&s[1]).
4.Masukkan char untuk intruksi kata yang ingin kita ubah dan intruksi balik.
5.Cetak pembalikkan kata dengan memanggil fungsi rekursif menggunakan type datanya.

**Pseudecoede**

```
#include
#include
void balik(char *k){
if(*k!=”){
balik(&k[1]);
cout<
}
}main(){
char *kata=”....”;--> //untuk masukan kata
balik(kata);
cout<
return 0;
```


**Code Program**
```c++
#include<iostream>
#include<string.h>

using namespace std;
void balik(char *s)
{ if (*s != '\0'){
balik(&s[1]);
cout << s[0];
}
}
int main()
{
      char* kata = (char*) "septi";
    balik(kata); cout << endl;
    return 0;

}
```

Hasil3
![Screenshot](https://raw.githubusercontent.com/putrintans/Praktikum7/master/Soal3/Screenshot3.png)
