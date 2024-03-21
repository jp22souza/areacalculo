package aplications;
import java.util.Locale;
import java.util.Scanner;
 
public class course {
    public static void main (String []args){

   Locale.setDefault(Locale.US);
   Scanner Sc = new Scanner (System.in);
    double xA;
      double xB;
   double xC;
   double yA;
   double yB;
   double yC;
    
        System.out.println("enter the measures of triangle x:");
      xA= Sc.nextDouble();
      xB=Sc.nextDouble();
      xC=Sc.nextDouble();
       System.out.println("Enter the measures of triangle Y: ");
   
    yA = Sc.nextDouble();
yB =    Sc.nextDouble();
yC = Sc.nextDouble();
    double p = (xA + xB + xC) / 2.0;
    double areaX = Math.sqrt(p*(p-xA)*(p-xB)*(p-xC));
    p  = (yA + yB + yC) / 2.0;
   double areaY = Math.sqrt(p * (p - yA) * (p - yB) * (p - yC));
   System.out.printf("Triangle X area: %.4f%n", areaX);
System.out.printf("Triangle Y area: %.4f%n", areaY);
   if (areaX>areaY){
       System.out.println("Larger area: X");
   }
   else {
       System.out.println("Larger area: Y");
  
   }
   Sc.close();
    }
}
