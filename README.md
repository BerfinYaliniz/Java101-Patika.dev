# Java101-Patika.dev

Bu repo [Kodluyoruz](Kodluyoruz.org) Java 101 eğitimi için hazırladığım Java pratik ve ödevlerinin soru ve cevaplarını içeren bir adet README içeriyor.

| PRATİKLER | ÖDEVLER |
|-----|-----|
| [PRATİK 1]- Not Ortalaması | [ÖDEV 1]- Vücut Kitle İndeksi Hesaplama|
| [PRATİK 2]- KDV Hesaplama |[ÖDEV 2]- Manav Kasa |
| [PRATİK 3]- Hipotenüs Bulma|
| [PRATİK 4]- Taksimetre |
| [PRATİK 5]- Daire & Alan & Çevre |
| [PRATİK 6]- Hesap Makinesi|
| [PRATİK 7]- Kullanıcı Girişi|
| [PRATİK 8]- Sınıfı Geçme Durumu|
| [PRATİK 9]- Hava Sıcaklığına Göre Etkinlik Önerme|
| [PRATİK 10]- Sayıları Büyükten Küçüğe Sıralayan Program|
| [PRATİK 11]- Burç Bulan Program|

---
## :open_book: PRATİK 1	- Not Ortalaması

### SORU :question:
Not Ortalaması Hesaplayan Program
Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı
yazın.

:interrobang: Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.

### :green_square: CEVAP

<details>
<summary>Kodu görmek için tıklayınız.</summary>
  
```java
package Pratik1;
import java.util.Scanner;

public class NotOrtalamasi {
    public static void main(String[] args) {

// Değişkenler tanımlandı ve veri girişi için scanner kodu kullanıldı.     
    double mat, fiz, kim, tur, tar, muz;
    Scanner input = new Scanner(System.in);
  
// Kullanıcıdan not değerleri alınarak değişkenlere atandı.       
    System.out.print("Matematik notunuzu giriniz = ");
    mat = input.nextInt();

    System.out.print("Fizik notunuzu giriniz = ");
    fiz = input.nextInt();

    System.out.print("Kimya notunuzu giriniz = ");
    kim = input.nextInt();

    System.out.print("Türkçe notunuzu giriniz = ");
    tur = input.nextInt();

    System.out.print("Tarih notunuzu giriniz = ");
    tar = input.nextInt();

    System.out.print("Müzik notunuzu giriniz = ");
    muz = input.nextInt();

// Değişkenler ile işlemler yapılarak ortalama değer hesaplandı.    
    double toplam = mat+fiz+kim+tur+tar+muz;
    double ortalama = toplam/6;
    
// Bulunan sonuç istenen koşul ile sorgulanarak ekrana yazdırıldı.
    System.out.println("Ortamanız = " + ortalama);
    boolean kosul1 = ortalama >= 50;
    System.out.println("Durum = " + (kosul1==true ? "Geçti" : "Kaldı"));
    
    }
}
```
