# Simple-quiz-game-in-java
import java.util.*;
public class Quiz {
    public static void main(String args[]) {
        String questions[] = new String[3];
        questions[0] = "how many continents there are ?";
        questions[1] = "which country is the worlds populated country ?";
        questions[2] = "smallest state in india ?";
        String answer[] = {"one", "two", "three", "seven"};
        String answer2[] = {"india", "china", "austriala", "america"};
        String answer3[] = {"goa", "delhi", "gujrat", "punjab"};
        double score = 0;
        Scanner obj = new Scanner(System.in);
        for (int i = 0; i < 5; i++) {
            if (i == 0) {
                System.out.println("  " + questions[i]);
                System.out.println("the options are :-");
                for (int j = 0; j < 4; j++) {
                    System.out.println("  " + j + "  = " + answer[j]);
                }
                System.out.println("enter your option");
                String firstopt;
                firstopt = obj.nextLine();
                System.out.println("the answer of this question is " + answer[3]);
                if (firstopt.compareToIgnoreCase(answer[3]) == 0) {
                    System.out.println(" correct answer");
                    score = score + 5;
                } else {
                    System.out.println(" incorrect");

                }
            }
            if (i == 1) {
                System.out.println("  " + questions[i]);
                System.out.println("the options are ;-");
                for (int b = 0; b < 4; b++) {
                    System.out.println("  " + b + " = " + answer2[b]);
                }
                System.out.println("enter your option");
                String secondopt;
                secondopt = obj.nextLine();
                System.out.println(" the answer of this question is  " + answer2[1]);
                if (secondopt.compareToIgnoreCase(answer2[1]) == 0) {
                    System.out.println(" correct answer");
                    score = score + 5;
                } else {
                    System.out.println(" incorrect");
                }
            }
            if (i == 2) {
                System.out.println("  " + questions[i]);
                System.out.println("the options are ;-");
                for (int c = 0; c < 4; c++) {
                    System.out.println("  " + c + " = " + answer3[c]);
                }
                System.out.println("enter your option");
                String thirdopt;
                thirdopt = obj.nextLine();
                System.out.println(" the answer of this question is  " + answer3[0]);
                if (thirdopt.compareToIgnoreCase(answer3[0]) == 0) {
                    System.out.println(" correct answer");
                    score = score + 5;
                } else {
                    System.out.println(" incorrect");
                }
            }
        }
        System.out.println(" your score is  = " + score);
    }
}



