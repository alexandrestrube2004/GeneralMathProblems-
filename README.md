import java.util.Scanner;
public class MatricesGenerator
{
    public static void main ()
    {
         Scanner ler = new Scanner (System.in);
         int X1, X2, X3, Y1, Y2, Y3, R;
         System.out.printf ("\n Hello! Give me six numbers and I will calculate the Matrices (3,2) for you ;)");
         System.out.print ("\n \n Example: \n (X1,Y2) \n (X2,Y2) \n (X3,Y3)");
         
         System.out.printf ("\n \n Enter X1: ");
         X1 = ler.nextInt ();
         
         System.out.printf ("\n Enter Y1: ");
         Y1 = ler.nextInt ();
         
         System.out.printf ("\n Enter X2: ");
         X2 = ler.nextInt ();
         
         System.out.printf ("\n Enter Y2: ");
         Y2 = ler.nextInt ();
         
         System.out.printf ("\n Enter X3: ");
         X3 = ler.nextInt ();
         
         System.out.printf ("\n Enter Y3: ");
         Y3 = ler.nextInt ();
         
         R = (X1 * Y2 * 1) + (Y1 * 1 * X3) + (1 * X2 * Y3) - (1 * Y2 * X3) - (X1 * 1 * Y3) - (Y1 * X2 * 1);
         
         if (R==0)
         {
             System.out.printf ("\n The answer is %d, it is COLLINEAR!!!", R);
         }
         else
         {
             System.out.printf ("\n The answer is %d, it is NOT COLLINEAR!!!", R);
         }
    }
}
