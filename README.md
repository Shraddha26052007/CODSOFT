import java.util.Scanner;
import java.util.Random;

public class GuessGame {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

  // Generate random number between 1 and 100
        int number = rand.nextInt(100) + 1;
        int guess = 0;

   System.out.println("Guess a number between 1 and 100:");
    // Loop until correct guess
   while (guess != number) {
            guess = sc.nextInt();
     if (guess > number) {
                System.out.println("Too high! Try again.");
            } 
            else if (guess < number) {
                System.out.println("Too low! Try again.");
            } 
            else {
                System.out.println("Correct! You guessed the number.");
            }
        }

  sc.close();
    }
}
