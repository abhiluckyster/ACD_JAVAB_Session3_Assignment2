# ACD_JAVAB_Session3_Assignment2

import java.util.Scanner;
public class PrimeNumber {
	public void calprime(int num)
{
		int k=0;
		
        for (int j=2; j<=num-1; j++)
        {
        	if (num%j==0)
			{	k = k+1;
			   break; 
			   }
		}
		if (k==0)
			System.out.println("Number is prime number " +num);
		else 
			System.out.println("Number is not a prime number " +num);

}
	public static void main(String args[]){	
		System.out.print("enter a number to check to be prime or not");
        Scanner number= new Scanner(System.in);
        int num = number.nextInt();
		PrimeNumber p = new PrimeNumber();
		p.calprime(num);
		number.close();
	}
}
	
