import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class WrapperClassExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<Integer> numbers = new ArrayList<>();
        
        System.out.print("Enter numbers separated by space: ");
        String input = scanner.nextLine();
        String[] strNumbers = input.split(" ");

        for (String str : strNumbers) {
            numbers.add(parseInteger(str)); // Autoboxing
        }

        int sum = calculateSum(numbers); // Unboxing in sum calculation
        System.out.println("Sum of numbers: " + sum);

        scanner.close();
    }

    private static Integer parseInteger(String str) {
        return Integer.parseInt(str);
    }

    private static int calculateSum(List<Integer> numbers) {
        int sum = 0;
        for (Integer num : numbers) {
            sum += num; // Unboxing
        }
        return sum;
    }
}
