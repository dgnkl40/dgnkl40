import java.util.Scanner;
public class hesapMakinesi {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
       
       int n1 ,n2 ,select ;

        System.out.print("İLK SAYIYI GİRİN: ");
        n1 = input.nextInt();
        System.out.print("İKİNCİSAYIYI GİRİN: ");
        n2 = input.nextInt();

        System.out.println("1-TOPLAMA ");
        System.out.println("2-ÇIKARMA ");
        System.out.println("3-ÇARPMA ");
        System.out.println("4-BÖLME ");

        System.out.print("SEÇİMİNİZİ YAPIN: ");
        select = input.nextInt();

        switch(select) {
            case 1:
                System.out.print("TOPLAM: " + (n1 + n2));
                break;
            case 2:
                System.out.print("ÇIKARMA: " + (n1 - n2));
                break;
            case 3:
                System.out.print("ÇARPMA: " + (n1 * n2));
                break;
            case 4:
                System.out.print((n2==0) ? "HİÇBİR SAYI SIFIRA BÖLÜNEMEZ" : "BÖLME :" + (n1 / n2));

                break;
            default:
                System.out.print("HİÇ BİR SAYI SIFIRA BÖLÜNMEZ");
                System.out.print("HATALI GİRİŞ");
        }

    }
}
