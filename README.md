# Comp-12.2

public class DivisorCalc {
    public static int gcd(int num1,int num2){
        try{
        if(num2%num1!=0){
            return gcd(num2,num1%num2);
        }
        else{
            return num1;
        }
        }
        catch(ArithmeticException ex){
            System.out.println("division by zero");
            return 0;
        }
    }
}
