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
Problem 3 :
-------------
Kullanıcının girdiği vize1,vize2,final notlarına notlarına göre harf notunu hesaplayın.

    Vize1 toplam notun %30'una etki edecek.

    Vize2 toplam notun %30'una etki edecek.

    Final toplam notun %40'ına etki edecek.     
    
cevap :
---------
vize1=int(input("1.vize notunuzu giriniz :"))
vize2=int(input("2.vize notunuzu giriniz :"))
final=int(input("final notunuzu giriniz :"))
sys_ortalama = (vize1*0.3+vize2*0.3+final*0.4)

if(sys_ortalama>=90) :
    print("sınıfı geçtiniz harf notunuz : AA")
elif(sys_ortalama>=85 and sys_ortalama <90) :
    print("sınıfı geçtiniz harf notunuz : BA")
elif (sys_ortalama >= 80 and sys_ortalama < 85):
    print("sınıfı geçtiniz harf notunuz : BB")
elif (sys_ortalama >= 75 and sys_ortalama < 80):
    print("sınıfı geçtiniz harf notunuz : CB")
elif (sys_ortalama >= 70 and sys_ortalama < 75):
    print("sınıfı geçtiniz harf notunuz : CC  tekrardan ders almanız yararınıza olur")
elif (sys_ortalama >= 65 and sys_ortalama < 70):
    print("sınıfı geçtiniz harf notunuz : DC  tekrardan ders almanız yararınıza olur")
elif (sys_ortalama >= 60 and sys_ortalama < 65):
    print("sınıfı geçtiniz harf notunuz : DD  tekrardan ders almanız yararınıza olur")
elif (sys_ortalama >= 55 and sys_ortalama < 60):
    print("dersten kaldınız harf notunuz: FD ")
elif (sys_ortalama <= 50  ):
    print("dersten kaldınız harf notunuz : FF"
    
---------------------------------------------------------------------------------------------------------------------------  Problem 4 :(sorulacakkk)
-------------------------
Şimdi de geometrik şekil hesaplama işlemi yapalım. İlk olarak kullanıcıdan üçgenin mi dörtgenin mi tipini bulmak istediğini sorun.

Eğer kullanıcı "Dörtgen" cevabını verirse , 4 tane kenar isteyip bu dörtgenin kare mi , dikdörtgen mi yoksa sıradan bir dörtgen mi olduğunu bulmaya çalışın.

Eğer kullanıcı "Üçgen" cevabını verirse , 3 tane kenar isteyip bu üçgenin ikizkenar mı , eşkenar mı yoksa sıradan bir üçgen mi olduğunu bulmaya çalışın. Eğer verilen kenarlar bir üçgen belirtmiyorsa, ekrana "Üçgen belirtmiyor" şeklinde bir yazı yazın.o

Üçgen belirtme şartını bilmiyorsunuz internetten bakabilirsiniz.

Ayrıca , bu problemde mutlak değer bulmaya ihtiyacınız olacak. Bunun için, Pythonda hazır bir fonksiyon olan abs() fonksiyonunu kullanabilirsiniz. Kullanımı şu şekildedir ;

cevap
-----------
şekil=input("hangi şeklin tipini öğrenmek istersiniz :")
if(şekil=="dörtgen") :
    print("lütfen kenarları sırası ile giriniz ")
    a = int(input("kenar 1 :"))
    b = int(input("kenar 2 :"))
    c = int(input("kenar 3 :"))
    d = int(input("kenar 4 :"))
    if(a==b and a==c and a==d) :
         print("kare")
    elif(a==c and b==d or a==b and c==d or a==d and b==c) :
         print("dikdörtgen")
    else:
         print("dörtgen")


elif (şekil=="üçgen") :
    a = int(input("kenar 1 :"))
    b = int(input("kenar 2 :"))
    c = int(input("kenar 3 :"))
    if(abs(a+b)>c and abs(b+c)>a and abs(a+c)>b):
       if(a==b and b==c) :
           print("eş kenar")
        elif((a==b and b!=c) or (a==c and b!=c) or (b==c and a!=c)):
           print("ikizkenar")
        else:
            print("çeşitkenar üçgen")
    else:
        print("üçgen belirtmiyor")
else:
    print("geçersiz şekil")


