# Java-Quiz-Game
The Java Quiz Game is a console-based program that tests users’ Java knowledge through multiple-choice questions. It provides instant feedback—showing if the answer is correct or wrong and displaying the correct answer when needed. At the end, it calculates the total score and shows pass/fail.


```java
import java.util.Scanner;

public class QuizGame {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int score = 0;

        System.out.println("===== JAVA QUIZ GAME =====");

        // Question 1
        System.out.println("\nQ1. Java is a ?");
        System.out.println("1) Programming Language");
        System.out.println("2) Operating System");
        System.out.println("3) Browser");
        System.out.println("4) Game");
        int ans1 = sc.nextInt();

        if (ans1 == 1) {
            System.out.println("Correct Answer!");
            score++;
        } else {
            System.out.println("Wrong Answer!");
            System.out.println(" Correct Answer is: 1) Programming Language");
        }

        // Question 2
        System.out.println("\nQ2. Which loop runs at least one time?");
        System.out.println("1) for");
        System.out.println("2) while");
        System.out.println("3) do-while");
        System.out.println("4) switch");
        int ans2 = sc.nextInt();

        if (ans2 == 3) {
            System.out.println("Correct Answer!");
            score++;
        } else {
            System.out.println("Wrong Answer!");
            System.out.println("Correct Answer is: 3) do-while");
        }

        // Question 3
        System.out.println("\nQ3. Which keyword is used to create object?");
        System.out.println("1) class");
        System.out.println("2) new");
        System.out.println("3) static");
        System.out.println("4) void");
        int ans3 = sc.nextInt();

        if (ans3 == 2) {
            System.out.println("Correct Answer!");
            score++;
        } else {
            System.out.println("Wrong Answer!");
            System.out.println(" Correct Answer is: 2) new");
        }

        // Question 4
        System.out.println("\nQ4. Which data type is used for decimal values?");
        System.out.println("1) int");
        System.out.println("2) char");
        System.out.println("3) float");
        System.out.println("4) boolean");
        int ans4 = sc.nextInt();

        if (ans4 == 3) {
            System.out.println("Correct Answer!");
            score++;
        } else {
            System.out.println("Wrong Answer!");
            System.out.println(" Correct Answer is: 3) float");
        }

        // Question 5
        System.out.println("\nQ5. Which symbol is used for single-line comment?");
        System.out.println("1) /* */");
        System.out.println("2) //");
        System.out.println("3) #");
        System.out.println("4) <!-- -->");
        int ans5 = sc.nextInt();

        if (ans5 == 2) {
            System.out.println("Correct Answer!");
            score++;
        } else {
            System.out.println("Wrong Answer!");
            System.out.println(" Correct Answer is: 2) //");
        }

        // Final Result
        System.out.println("\n===== RESULT =====");
        System.out.println("Your Score: " + score + " / 5");

        if (score >= 3) {
            System.out.println(" Congratulations! You Passed");
        } else {
            System.out.println(" Try Again");
        }

        sc.close();
    }
}


