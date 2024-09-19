import java.util.Scanner;

/**
 * Клас, що представляє число Фібоначчі.
 */
class FibonacciNumber {
    private int number;
    private long value;

    /**
     * Конструктор для обчислення числа Фібоначчі.
     *
     * @param num Порядковий номер числа Фібоначчі.
     */
    public FibonacciNumber(int num) {
        this.number = num;
        this.value = calculateFibonacci(num);
    }

    /**
     * Отримати значення числа Фібоначчі.
     *
     * @return Значення числа Фібоначчі.
     */
    public long getValue() {
        return value;
    }

    /**
     * Перевірити, чи можна число Фібоначчі представити у вигляді w^2 + 1.
     *
     * @return true, якщо число можна представити у вигляді w^2 + 1; false інакше.
     */
    public boolean isSquarePlusOne() {
        long w = (long) Math.sqrt(value - 1);
        return (w * w + 1) == value;
    }

    /**
     * Обчислити число Фібоначчі для заданого порядкового номера.
     *
     * @param n Порядковий номер числа Фібоначчі.
     * @return Значення числа Фібоначчі.
     */
    private long calculateFibonacci(int n) {
        if (n <= 2) {
            return 1;
        } else {
            return calculateFibonacci(n - 1) + calculateFibonacci(n - 2);
        }

    }
}
/**
 * Клас для обчислення чисел Фібоначчі та перевірки, чи можна їх представити у вигляді w^2 + 1.
 */
class Fibonacci {
    /**
     * Головний метод програми.
     * @param args Масив аргументів командного рядка. Перший аргумент - кількість чисел Фібоначчі для обчислення.
     */
    public static void main(String[] args) {
        int n;
        if (args.length > 0) {
            n = Integer.parseInt(args[0]);
        } else {
            System.out.print("Введіть кількість чисел Фібоначчі: ");
            Scanner scanner = new Scanner(System.in);
            n = scanner.nextInt();
            scanner.close();
        }

        for (int i = 1; i <= n; i++) {
            FibonacciNumber fib = new FibonacciNumber(i);
            if (fib.isSquarePlusOne()) {
                System.out.println("Число Фібоначчі " + i + " (" + fib.getValue() + ") можна представити у вигляді w^2 + 1");
            }
        }
    }
}





