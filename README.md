# KDV-Tutar-Hesaplayan-Program
KDV-Tutar-Hesaplayan-Program

package Giris;

import java.util.Scanner;

public class Kdvtutari {
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        System.out.println("tutar giriniz: ");
        int tutar =input.nextInt();

        if(tutar<=1000 && tutar>0) {
            double kdvli = (0.18) * tutar + tutar;
            System.out.println("tutar: " +tutar);
            System.out.println("KDV tutarı: 0.18" );
            System.out.println("KDV'li fiyat: " + kdvli);
        }
        if(tutar>1000){
            double kdv= (0.08)*tutar +tutar;
            System.out.println("tutar: " +tutar);
            System.out.println("KDV tutarı: 0.08");
            System.out.println("KDV'li fiyat: " + kdv);
        }
    }
}

