import java.util.Scanner;  // Scanner sınıfını dahil ettik

public class Main {
    public static void main(String[] args) {
        // Değişkenleri oluştur
        int mat, fizik, kimya, turkce, tarih;

        // Scanner sınıfımızı tanımladık
        Scanner input = new Scanner(System.in);

        // Kullanıcıdan değerleri al
        System.out.print("Matematik notunuzu giriniz: ");
        mat = input.nextInt();

        System.out.print("Fizik notunuzu giriniz: ");
        fizik = input.nextInt();

        System.out.print("Kimya notunuzu giriniz: ");
        kimya = input.nextInt();

        System.out.print("Türkçe notunuzu giriniz: ");
        turkce = input.nextInt();

        System.out.print("Tarih notunuzu giriniz: ");
        tarih = input.nextInt();

        // Notların ortalamasını hesapla
        double ortalama = (mat + fizik + kimya + turkce + tarih) / 5.0;

        // Ortalamayı ekrana yazdır
        System.out.println("Ortalamanız: " + ortalama);

        // Başarı durumunu kontrol et
        if (ortalama >= 60) {
            System.out.println("Tebrikler, sınıfı geçtiniz!");
        } else {
            System.out.println("Maalesef kaldınız, sınıfta kaldiniz daha fazla çalışmalısınız.");
        }

        // Scanner nesnesini kapat
        input.close();
    }
}
