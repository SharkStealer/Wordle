import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class WordGame {
  
    private static final int ROW = 6;
    private static final int COL = 5;
    private static final int KEYBOARD_ROW = 3;
    private static final int KEYBOARD_COL = 10;
  
    private static final String[] wordList = {
        "apple", "banana", "cherry", "date", "elderberry", 
        "fig", "grape", "honeydew", "kiwi", "lemon", 
        "mango", "nectarine", "orange", "pear", "quince"
    };
  
    private static String[][] guesses = new String[ROW][COL];
    private static char[][] keyboard = {
        {'q', 'w', 'e', 'r', 't', 'y', 'u', 'i', 'o', 'p'},
        {'a', 's', 'd', 'f', 'g', 'h', 'j', 'k', 'l'},
        {'z', 'x', 'c', 'v', 'b', 'n', 'm'}
    };
    
  
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice = 0;
        do {
            System.out.println("Word Game Menu:");
            System.out.println("1. Start a new game");
            System.out.println("2. Randomize the word list");
            System.out.println("3. Sort the word list");
            System.out.println("4. Print the word list");
            System.out.println("5. Quit");
            System.out.print("Enter your choice: ");
            choice = sc.nextInt();
            switch (choice) {
                case 1:
                startNewGame();
                break;
                case 2:
                randomizeWordList();
                break;
                case 3:
                sortWordList();
                break;
                case 4:
                printWordList();
                break;
            }
        } while (choice != 5);
            System.out.println("Thank you for playing the Word Game!");
            sc.close();
    }
  
    private static void startNewGame() {
        String word = chooseWord();
        System.out.println("The word is: " + word);
        System.out.print("Enter your guess (5 letters only): ");
        Scanner sc = new Scanner(System.in);
        String guess = sc.nextLine().toLowerCase();
        while (!checkLength(guess)) {
            System.out.println("Invalid input! Your guess must be 5 letters only.");
            System.out.print("Enter your guess (5 letters only): ");
            guess = sc.nextLine().toLowerCase();
        }
        System.out.println("Your guess: " + guess.toUpperCase());
        if (checkGuess(word, guess)) {
            System.out.println("Correct! You win.");
        } else {
            System.out.println("Your guess: " + guess.toUpperCase());

    // Check if the length of the guess is 5
    if (guess.length() != 5) {
        System.out.println("Your guess must be 5 letters long.");
        return;
    }

    String word = words[randomIndex];
    StringBuilder result = new StringBuilder();

    // Check each letter of the guess
    for (int i = 0; i < 5; i++) {
        char c = guess.charAt(i);
        if (word.charAt(i) == c) {
            result.append(Character.toUpperCase(c));
        } else if (word.indexOf(c) != -1) {
            result.append(Character.toLowerCase(c));
        } else {
            result.append("\u0336").append(c);
        }
    }

    // Check if the guess is correct
    if (result.toString().equals(word)) {
        System.out.println("Correct! The word is " + word);
    } else {
        System.out.println(result);
    }
    
    
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Welcome to Word Guess Game!");
        System.out.println("1. Randomize words");
        System.out.println("2. Sort words");
        System.out.println("3. Print words");
        System.out.println("4. Guess word");

        int choice = input.nextInt();

        // Randomize words
        if (choice == 1) {
            randomizeWords(words);
            System.out.println("Words randomized successfully.");
        }
        // Sort words
        else if (choice == 2) {
            Arrays.sort(words);
            System.out.println("Words sorted successfully.");
        }
            // Print words
        else if (choice == 3) {
            System.out.println(Arrays.toString(words));
        }
        // Guess word
        else if (choice == 4) {
            guessWord();
        } else {
            System.out.println("Invalid choice. Please try again.");
        }
    }

    public static void randomizeWords(String[] words) {
        Random random = new Random();
        for (int i = words.length - 1; i > 0; i--) {
            int index = random.nextInt(i + 1);
            String temp = words[index];
            words[index] = words[i];
            words[i] = temp;
        }
    }
    public static void displayGuessArray(String[][] guessArray) {
        System.out.println("6x5 Guess Array:");
        for (String[] row : guessArray) {
            for (String column : row) {
            System.out.print(column + " ");
            }
        System.out.println();
        }
    }

    public static void displayKeyboardArray(char[][] keyboardArray) {
        System.out.println("3x10 Keyboard Array:");
        for (char[] row : keyboardArray) {
            for (char column : row) {
            System.out.print(column + " ");
            }
        System.out.println();
        }
    }
    }
  }
}
