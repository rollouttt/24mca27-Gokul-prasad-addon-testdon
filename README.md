package exam;

public class exam1 {
    public static void main(String[] args) {
        int n = 5;
        int mid = (n / 2) + 1;

    
        for (int i = 1; i <= mid; i++) {
            for (int j = 1; j <= mid - i; j++)
                System.out.print("  "); 
            for (int j = 1; j <= (2 * i - 1); j++)
                System.out.print("* ");
            System.out.println();
        }

      
        for (int i = mid - 1; i >= 1; i--) {
            for (int j = 1; j <= mid - i; j++)
                System.out.print("  "); // print spaces
            for (int j = 1; j <= (2 * i - 1); j++)
                System.out.print("* ");
            System.out.println();
        }
    }
}
 QUESTION 2 ;
package exam;

public class exam2 {
    public static void main(String[] args) {
        System.out.print("Perfect numbers between 1 and 1000: ");
        for (int num = 1; num <= 1000; num++) {
            int sum = 0;
            for (int i = 1; i < num; i++) {
                if (num % i == 0) {
                    sum = sum + i;
                }
            }
            if (sum == num) {
                System.out.print(num + " ");
            }
        }
    }
}

QUESTION 3
package exam;

public class exam3 {
	
    public static void main(String[] args) {
        int[] arr = {10, 20, 50, 30, 40};
        int largest = arr[0];
        int second = arr[0];

        for (int i = 0; i < arr.length; i++) {
            if (arr[i] > largest) {
                second = largest;
                largest = arr[i];
            } else if (arr[i] > second && arr[i] != largest) {
                second = arr[i];
            }
        }

        System.out.println("Second largest element = " + second);
    }
}
QUESTION 4;
package exam;
public class exam4 {
    public static void main(String[] args) {
        String s = "programming";
        String result = "";

        for (int i = 0; i < s.length(); i++) {
            char ch = s.charAt(i);
            if (result.indexOf(ch) == -1) {
                result = result + ch;
            }
        }

        System.out.println("Result = " + result);
    }
}
QUESION 5;
package exam;

import exam.Rectangle;

class Rectangle {
    int length;
    int breadth;

    Rectangle() {
        length = 1;
        breadth = 1;
    }

    Rectangle(int l, int b) {
        length = l;
        breadth = b;
    }

    int getArea() {
        return length * breadth;
    }
}

public class exam5 {
    public static void main(String[] args) {
        Rectangle r1 = new Rectangle();
        Rectangle r2 = new Rectangle(5, 10);

        System.out.println("Area (default): " + r1.getArea());
        System.out.println("Area (5,10): " + r2.getArea());
    }
}























 

question ; 2
