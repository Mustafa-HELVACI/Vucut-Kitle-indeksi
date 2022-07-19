# Vucut-Kitle-indeksi
Java ile kullanıcıdan boy ve kilo değerlerini alıp  "Vücut Kitle İndeksi" hesaplama.


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        double mt,kg,kitle;

        Scanner input = new Scanner(System.in);
        System.out.print("Lütfen boyunuzu (mt cinsinde) Girin :");
        mt = input.nextDouble();
        System.out.print("Lütfen Kilonuzu Girin :");
        kg = input.nextDouble();

        kitle = kg / (mt * mt);
        System.out.println("Vücut Kitle İndeksiniz :" + kitle);

        System.out.print((kitle >= 20.0) ? "Fazla Kilonuz var. " : "Kilonuz İdeal. ");
        System.out.println((kitle >= 20.0) ? "Biraz daha az yemek yiyerek daha fazla su tüketmelisin." : "Bir deri bir kemik kalacaksın, biraz yemek ye :))).");


    }
}
