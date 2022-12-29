import java.util.Scanner;
public class kullanıcıGirişi {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String password,userName,secenek;

        System.out.print("Kullanıcı Adını Gir: ");
        userName = input.nextLine();
        System.out.print("Şifreyi Gir: ");
        password = input.nextLine();

        if (userName.equals("haziran") && password.equals("hazır123")){
            System.out.print("GİRİŞ BAŞARILI");
        }
        else {
            System.out.println("ŞİFRE YANLIŞ");
            System.out.println("ŞİFREYİ SIFIRLAMAK İSTER MİSİN?");
            System.out.print("YES - NO:");
            secenek = input.next();
            if (secenek.equals("yes")){

                System.out.print("YENİ ŞİFREYİ GİR: ");
                password = input.next();

                if ( password.equals("hazır123")){
                    System.out.println("AYNI ŞİFREYİ TEKRAR GİREMEZSİNİZ");
                }
                else {
                    System.out.println("YENİ ŞİFRE OLUŞTU");
                }
            }
        }
    }
}
