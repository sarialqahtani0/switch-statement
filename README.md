public class Calc {
    public static void main(String[] args) {

        java.util.Scanner s = new java.util.Scanner(System.in);

        double num1 = s.nextDouble();
        double num2 = s.nextDouble();
        String operator = s.next();

        switch (operator) {
            case "+": System.out.println(num1 + num2); break;
            case "-": System.out.println(num1 - num2); break;
            case "*": System.out.println(num1 * num2); break;
            case "/":
                if (num2 == 0) System.out.println("Division by zero error");
                else System.out.println(num1 / num2);
                break;
            default: System.out.println("Invaled operator");
        }

        s.close();
    }
}
