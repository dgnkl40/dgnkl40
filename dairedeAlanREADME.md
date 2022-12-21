import java.util.Scanner ;
public class daireAlan {
    public static void main(String[] args) {

        //Ödev
        //Yarıçapı r, merkez açısının ölçüsü 𝛼 olan daire diliminin alanı bulan programı yazınız.
        //𝜋 sayısını = 3.14 alınız.
        //Formül : (𝜋 * (r*r) * 𝛼) / 360

        double yarıcap , mAcı , pi = 3.14 , dDaire ;
        Scanner input = new Scanner(System.in) ;

        System.out.print("Yarıçapı Girin: ");
        yarıcap = input.nextDouble();
        System.out.print("Merkez Açı Ölçüsünü Girin: ");
        mAcı = input.nextDouble();

        dDaire = (pi*(yarıcap*yarıcap)*mAcı) / 360 ;

        System.out.print("Daire Diliminin Alanı: " + dDaire);


    }
}

