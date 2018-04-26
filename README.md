# Task1Burg

import java.util.Scanner;

public class Number {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int i = sc.nextInt();
		int x = i, c = 0;
		while (x != 0) {
			++c;
			x /= 10;
		}
		int[] j = new int[c];
		while (i != 0) {
			j[--c] = i % 10;
			i /= 10;
		}
		for (int k : j)
			System.out.println("Digit " + k);

	}
}
