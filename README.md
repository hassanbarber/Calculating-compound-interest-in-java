# Calculating-compound-interest-in-java
Calculating compound interest in java
public class TinhLaiKep {
     public void calculate(int p, int t, double r, int n) {
         double amount = p * Math.pow(1 + (r / n), n * t);
         double cinterest = amount - p;
         System.out.println("Compound interest after " + t + " year is : "+cinterest);
         System.out.println("The amount obtained after " + t + " year is: "+amount);
     }
     public static void main(String args[]) {
         TinhLaiKep obj = new TinhLaiKep();
         obj.calculate(2000, 5, .08, 12);
     }
}
