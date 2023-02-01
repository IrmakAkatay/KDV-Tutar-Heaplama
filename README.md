# KDV-Tutar-Heaplama
import java.io.FilterOutputStream;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    .

        double tutar,kdvOran=0.18,kdvliTutar,kdvOranı1= 0.18,kdvOranı2= 0.08,kdvTutarı1,kdvTutarı2,kdvOranı ;

        Scanner abs = new Scanner(System.in);
        System.out.print("Ücret Tutarını Giriniz :");
        tutar = abs.nextDouble();

        double kdvTutar= tutar * kdvOran ;
         kdvliTutar = tutar+kdvTutar;

        kdvOranı1 = kdvOranı1* tutar;
        kdvOranı2 = kdvOranı2* tutar;

        kdvOran= tutar>=0 && tutar<=1000?  kdvOranı1:kdvOranı2;
        kdvTutar=tutar/kdvOran;
        kdvliTutar=kdvOran+tutar;


         System.out.println("KDV Oranı : " + kdvOran+"TL");
         System.out.println("KDV Tutarı : " + kdvTutar+"TL");
         System.out.println("KDV'siz Tutar :" +tutar+ "TL");
         System.out.println("KDV'li Tutar : " + kdvliTutar+"TL");

         }

    }
    www.patika.dev
