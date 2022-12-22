
//Vücut Kitle İndeksi Hesaplama
//Java ile kullanıcıdan boy ve kilo değerlerini alıp bir değişkene atayın. Aşağıdaki formüle göre kullanıcının "Vücut Kitle İndeks" değerini hesaplayıp ekrana yazdırın.
//Formül
//Kilo (kg) / Boy(m) * Boy(m)

import java.util.Scanner;
public class vucutIndeksi {
    public static void main(String[] args) {
        
       
        Scanner input = new Scanner(System.in);

        double kilo , boy , index;

        System.out.print("LÜTFEN BOYUNUZU GİRİN(Metre): ");
        boy = input.nextDouble();
        System.out.print("LÜTFEN KİLONUZU GİRİN(Kilogram): ");
        kilo = input.nextDouble();

        index = kilo / (boy * boy) ;

        System.out.print("VÜCUT KİTLE İNDEKSİNİZ: " + index);
    }
}
