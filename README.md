# GetDigitsSum
C Sistem Derneği - Oğuz KARAN Hocamızın dersinden alıntıdır.


package csd;

class App {

	public static void main(String[] args) 
	{
		GetDigitsSumTest.run();
	}
}

class GetDigitsSumTest {
	
	public static void run ()
	{
		java.util.Scanner kb = new java.util.Scanner(System.in);
		System.out.print("Bir sayı giriniz: ");
		int val = Integer.parseInt(kb.nextLine());
		
		System.out.printf("Girilen sayı: %d  --> Basamaklarının toplamı: %d%n", val, GetDigitsSum.NumberUtil(val));		
	}
}


class GetDigitsSum {
	
	public static int NumberUtil (int val)
	{	
		int a = val / 100 ;
		int b = val % 100 / 10 ;
		int c = val % 10;
		
		return a + b + c;	
	}
}
