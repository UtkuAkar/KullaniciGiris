# KullaniciGiris

import java.util.Scanner;

public class Kullanici {
    public static void main(String[] args) {

        String userName,password,yenipas,pasreset="";

        Scanner input=new Scanner(System.in);

        System.out.println("Kullanıcı Adınız : ");
        userName=input.nextLine();

        System.out.println("Şifreniz  : ");
        password=input.nextLine();


        if (userName.equals("patika") && password.equals("java123")){ //equals eşitmi demek sadece strıngler ıcın kullanılır
            System.out.println("Giriş Yaptınız ");
        }
        else {
            System.out.println("Hata Yaptınız.Sifre Sıfırlamak istermisiniz. yes/no ");
            pasreset= input.nextLine();

            if(pasreset.equals("no")){
                System.out.println("Program kapanıyor");

            }
            else if(pasreset.equals("yes")){
            System.out.println("Yeni Sifre : ");
            yenipas=input.nextLine();

                if(yenipas.equals("patika") || yenipas.equals("java123")){
                System.out.println("Aynı Sifre Olamaz: ");

                }
                else {
                System.out.println("Sifre Sıfrenız Degıstı: ");
                }

            }
            else{
                System.out.println("HATALI  Secım.");
            }

        }

    }
}
