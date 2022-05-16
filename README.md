#Q1
package lina;
import java.util.*;

public class rounding {
    public static void main(String []args) {
            Scanner scanner = new Scanner(System.in);
            System.out.println("Enter your grade:");
            int grade= scanner.nextInt();
            if (grade > (grade-3 )&& (grade % 5) >= 3)
                grade = grade + (5 - (grade % 5));
            System.out.println(grade);
    }
}


#Q2
package lina;

public class multipleNumbers {
    public static void main(String args[])
    {
        for (int i=1; i<=100; i++)
        {
            // Numbers that are divisible by 3 and 5
            // are always divisible by 15
            // Therefore, "FizzBuzz" is printed in place of that number
            if (i%15==0)
            {
                System.out.println("FizzBuzz");
            }
            // "Fizz" is printed in place of numbers
            // that are divisible by 3
            else if (i%3==0)
            {
                System.out.println("Fizz");
            }
            // "Buzz" is printed in place of numbers
            // that are divisible by 5
            else if (i%5==0)
            {
                System.out.println("Buzz");
            }
            // If none of the above conditions are satisfied,
            // the number is printed
            else
            {
                System.out.println(i);
            }
        }
    }
}


#Q3
package lina;

public class vowel {
        static boolean isVowel(char ch)
        {
            ch = Character.toUpperCase(ch);
            return (ch=='A' || ch=='E' || ch=='I' ||
                    ch=='O' || ch=='U');
        }
        static int countVowels(String str)
        {
            int count = 0;
            for (int i = 0; i < str.length(); i++)
                if (isVowel(str.charAt(i))) // Check for vowel
                    ++count;
            return count;
        }
        static int maxMethod(int num1, int num2)
        {
           int result = Math.max(num1,num2);
          return result;
        }

        public static void main(String args[])
        {
            String str = "Welcome";
            System.out.println(countVowels(str));
            System.out.println(maxMethod(8,10));
        }
}
