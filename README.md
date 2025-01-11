# Electricity-bill
package electricity.bill;
import java.util.Scanner;
public class ElectricityBill {
    public static void main(String[] args) {
         Scanner scan = new Scanner (System.in);
        System.out.println("Enter the numbers of units consumed:");
        double units=scan.nextDouble();
        double billamount;
        if(units<=100){
            billamount=units*1.50;
        }else if (units<=200){
            billamount=(100*1.50)+((units-100)*2.00);
        }else{
            billamount=(100*1.50)+(100*2.00)+((units-200)*300);
        }
        System.out.println("The electricity bill is:Rs."+billamount);
    }
}
        
    


Output:

Enter the numbers of units consumed:
75
The electricity bill is:Rs.112.5
