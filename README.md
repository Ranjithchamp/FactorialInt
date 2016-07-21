# FactorialInt
import java.util.Scanner;

public class Factorial {

	public static void main(String[] ard) {
		int input;
		Scanner a = new Scanner(System.in);
		input = a.nextInt();
		long output = 1;
		long factorial;
		double ans = 1;
		if (input < 0) {
			System.out.println("the factorial of " + input + " is " + 0);
		} else if (input == 0) {
			output = 1;
		} else if (input >= 22) {
			for (long i = 1; i <= input; i++) {
				ans = ans * i;
			}
			System.out.println("range out of long so output in double");
			System.out.println("factorial of " + input + " ans=" + ans);
		} else {
			for (long i = 1; i <= input; i++) {
				output = output * i;
			}
			factorial = output;
			System.out.println("factorial of " + input + " is " + factorial);
		}
	}
}
