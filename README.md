# pytho_kosullu_ifadeler_soru
------------------------------
1.problem :
-----------
Kullanıcıdan alınan boy ve kilo değerlerine göre beden kitle indeksini hesaplayın ve şu kurallara göre ekrana şu yazıları yazdırın.

 Beden Kitle İndeksi: Kilo / Boy(m) *  Boy(m)

 BKİ 18.5'un altındaysa -------> Zayıf

 BKİ 18.5 ile 25 arasındaysa ------> Normal

 BKİ 25 ile 30 arasındaysa --------> Fazla Kilolu

 BKİ 30'un üstündeyse -------------> Obez
 
 cevap :
 -------
 boy=float(input("boyunuzu metre cinsinden giriniz :"))
kilo=int(input("kilonuzu kg cinsinden giriniz :"))
BKİ=(kilo/boy**2)
if(BKİ<18.5) :
    print("normal BKİ için zayıfsınız kilo almanız gerek .")
elif(BKİ>=18.5 and BKİ<25) :
    print("BKİ ' niz normal .")
elif(BKİ>=25 and BKİ<30) :
    print("normal BKİ 'için kilonuz fazla zayıflamanız lazım .")
else :
     print("BKİ'nin çok1 üstündesiniz acil olarak zayıflamanız lazım(obez).")
     ------------------------------------------------------------------------------------------------------------------------
     Problem 2 :
     ------------
    
    Kullanıcıdan 3 tane sayı alın ve en büyük sayıyı ekrana yazdırın.
cevap :
---------
a=int(input("a :"))
b=int(input("b :"))
c=int(input("c : "))
if(a>b and a>c ) :
    print(" en büyük sayı :",a)
elif(b>a and b>c) :
    print(" en büyük sayı :",b)
else :
    print(" en büyük sayı : ",c)
---------------------------------------------------------------------------------------------------------------------------


     
