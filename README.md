# userPasswordControler
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner inp =new Scanner(System.in);
        String userName,password, passwordNew;
        int select;
        System.out.println("Lütfen Kullanıcı Adını Giriniz: ");
        userName=inp.nextLine();
        System.out.println("Lütfen Şifrenizi Giriniz: ");
        password=inp.nextLine();
        if(userName.equals("patika")&&password.equals("java123")){
            System.out.println("Sisteme Giriş Yaptınız");
        }else{
            System.out.println("Yanlış Giriş Yaptınız.\nŞifrenizi Sıfırlamak için 1'e Basınız \nÇıkmak için 0'a Basınız");
            select=inp.nextInt();
            switch (select){
                case 1:
                    Scanner input =new Scanner(System.in);
                    System.out.println("Lütfen Yeni Şifre Oluşturunuz: ");
                    passwordNew=input.nextLine();

                    if(passwordNew.equals("java123")){
                        System.out.println("Şifre oluşturulamadı, lütfen önceki şifrenizden başka bir şifre giriniz.");
                        passwordNew =inp.nextLine();
                    }else{
                        System.out.println("Şifrenizi Oluşturdunuz:"+passwordNew);
                    }
                    break;

            }
            }
            }
        }
       
