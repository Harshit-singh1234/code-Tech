import java.util.Scanner;
import java.lang.Math;

public class armstrong {
    public static void main(String[] args) {
        Scanner muyobj = new Scanner(System.in);
        int n;
        int temp;
        // temp=n;
        n = muyobj.nextInt();
        temp = n;
        int s = 0;
        int rem = 0;
        while (n != 0) {
            rem = n % 10;
            s = s + (int) Math.pow(rem, 3);
            n = n / 10;
        }
        if (temp == s) {
            System.out.println(temp + "the given number is armstrong");
        } else {
            System.out.println("not armstrong");
        }

    }

}
