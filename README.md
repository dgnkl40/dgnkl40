import java.util.Scanner;
public class sınıfGecme {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        //Dersler : Matematik, Fizik, Türkçe, Kimya, Müzik
        //Geçme Notu : 55
        //Ödev
        //Eğer girilen ders notları 0 veya 100 arasında değil ise ortalamaya katılmasın.

        double mat , fiz , tur , kim , muz ,avarege;

        System.out.print("Matematik Notu: ");
        mat = input.nextFloat();
        System.out.print("Fizik Notu: ");
        fiz = input.nextFloat();
        System.out.print("Türkçe Notu: ");
        tur = input.nextFloat();
        System.out.print("Kimya Notu: ");
        kim = input.nextFloat();
        System.out.print("Müzik Notu: ");
        muz = input.nextFloat();

        avarege = ((mat + fiz + tur + kim + muz) / 5 );
        System.out.println("Ortalama: " + avarege );

       


        if (avarege >= 55){
            System.out.println("GEÇTİN");
        }
        else {
            System.out.println("KALDIN");
        }
    }
}
