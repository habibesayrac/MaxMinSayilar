# MaxMinSayilar
import java.util.Scanner;
public class Main {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        int enBuyuk=0;
        int enKucuk=0;

        System.out.println("Kaç tane sayı gireceksiniz? :  ");
        int n1= input.nextInt();

        for(int i=1;i<=n1;i++) {
            System.out.println(i + ". Sayı: ");
            int n2 = input.nextInt();

            if (i == 1) {
                enBuyuk = n2;
                enKucuk = n2;
            } else {
                if (n2 > enBuyuk) {
                    enBuyuk = n2;
                } else if (n2 < enKucuk) {
                    enKucuk = n2;
                }
            }
        }
        System.out.println("En Büyük Sayı " + enBuyuk);
        System.out.println("En Küçük Sayı " + enKucuk);
    }
}
