# FirstLab
Digit Sum Lab
package digitsum;
import java.util.Scanner;
public class DigitSum {

	public static void main(String[] args) {
		
		Scanner input = new Scanner(System.in);
		
		System.out.println("Please input an integer between 0 and 1000:");
		int number = input.nextInt();
		
		while (number < 0 || number > 1000) {
			System.out.println("Sorry. The number you enetered is not between 0 and 1000. Please re-enter:");
			number = input.nextInt();
		}
		
		int DigOne = number % 10;
		int remainder = number / 10;
		
		int DigTwo = remainder % 10;
		remainder = remainder / 10;
		
		int DigThree = remainder % 10;
		remainder = remainder / 10;
		
		int DigFour = remainder % 10;
		
		int sum = DigOne + DigTwo + DigThree + DigFour;
		System.out.println("The sum of the digits is: " +sum);
	}

}
