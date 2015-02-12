# Tale-Recursion-Factorial
import java.util.Scanner;

public class Tale_Factorial {
	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		System.out.println("Enter number to be factorialized");
		int x = input.nextInt();

		System.out.println(factorial(x, x - 1));

	}

	public static int factorial(int oldNum, int n) {
		// if n is one then add return the numbers that have been multiplied
		// with recursion
		if (n == 1)
			return oldNum;
		// other wise keep multiplying the old number by the new number that is
		// the previous number of the old number.
		else

			return factorial(oldNum * n, n - 1);
	}
}
