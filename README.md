public static void main(String[] args) {
        System.out.println("SIMPLE CALCULATOR");
        int a, b;
        char operator;
        String option;
        Scanner scanner = new Scanner(System.in);
        while (true) {
        System.out.println("enter the number a=");
        a = scanner.nextInt();
        System.out.println("enter the number b=");
        b = scanner.nextInt();
        System.out.println("enter the operator");
        operator = scanner.next().charAt(0);
            switch (operator) {
                case '+': {
                    System.out.print(a + b);
                    break;
                }
                case '-': {
                    System.out.print(a - b);
                    break;
                }
                case '*': {
                    System.out.print(a * b);
                    break;
                }
                case '/': {
                    System.out.print(a / b);
                    break;
                }
                default:
                    System.out.println("invalid");
            }
                System.out.println("do u want continue:");
                option = scanner.next();
                if (option.equals("no")) {
                    break;
                }
            }
        }
    }



