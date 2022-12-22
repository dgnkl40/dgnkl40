import java.util.Scanner;
public class manavTartısı {
    public static void main(String[] args) {
        Scanner gırdı = new Scanner(System.in);
        double armut = 2.14,elma = 3.67,domates = 1.11,muz = 0.95 ,patlıcan = 5.00 , total;
        double kga,kge,kgd,kgm,kgp;
        System.out.print("Kaç Kilo Armut: ");
        kga = gırdı.nextDouble();
        System.out.print("Kaç Kilo Elma: ");
        kge = gırdı.nextDouble();
        System.out.print("Kaç Kilo Domates: ");
        kgd = gırdı.nextDouble();
        System.out.print("Kaç Kilo Muz: ");
        kgm = gırdı.nextDouble();
        System.out.print("Kaç Kilo Patlıcan : ");
        kgp = gırdı.nextDouble();

        total = ((armut * kga) + (elma * kge) + (domates * kgd) + (muz * kgm) + (patlıcan * kgp));


        System.out.print("TOPLAM TUTAR: " + total );

    }
}
