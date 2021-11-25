# maxmin_javamethods
import java.awt.*;
import java.util.Arrays;
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner a = new Scanner(System.in);
        System.out.print("Enter the array size:");
        int input = a.nextInt();
        int[] number = new int[input];
        System.out.println("Enter the array elements:");
        for(int i=0;i<input;i++){
        int number1 = a.nextInt();
        number[i]=number1;
            
        }
        System.out.println(Arrays.toString(number));
        min(number);
        max(number);
    }
        
        public static void min(int[] number){
            int initial = number[0];
            for(int i=0;i<number.length;i++){
                if (number[i]<initial){
                    initial=number[i];
                    
                }
                
            }
            System.out.println("The minimum is: "+initial);
        }
          // System.out.println(Arrays.toString(number));}
        
        public static void max(int[] number){
            int initial = number[0];
            for(int i=0;i<number.length;i++){
                if (number[i]>initial){
                    initial=number[i];
                    
                }
               
            }
             System.out.println("The maximum is: "+initial);
        }
        
        

}
