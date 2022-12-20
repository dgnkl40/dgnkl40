import java.util.Scanner ;

public class taksmetre {
    public static void main(String[] args) {

        //Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.
        //
        //Taksimetre KM başına 2.20 TL tutmaktadır.
        //Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
        //Taksimetre açılış ücreti 10 TL'dir.

        Scanner input = new Scanner(System.in) ;
        int km ;
        double perKm = 2.20 , total , start = 10 ,stotal ;

        System.out.print("Gidelecek Mesafeyi KM cinsinden Giriniz: ");
        km = input.nextInt() ;

        total = (perKm * km) + start ;


         stotal = total <= 20 ? 20 : total ;

        System.out.print("Toplam Ödenecek Tutar: " + stotal);
    }
}
