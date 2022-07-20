# palindrom_sayi.java
www.patika.dev






import java.util.Enumeration;

public class Palindrom_sayi {
    static boolean palindrom(int number){
        int temp =number,reversenumber=0,lastnumber;
        while (temp!=0){
            lastnumber=temp%10;
            reversenumber=(reversenumber*10)+lastnumber;
            temp/=10;
        }
        if(number==reversenumber)
            return true;
        else
            return false;
    }
    public static void main(String[] args) {
        System.out.println(palindrom(4));
    }
}
