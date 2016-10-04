# Read-Number
import java.util.Scanner;

public class EX1 {

	public static void main(String[] args) {
		
		/*Написать программу которая считывает 5-и значное число с клавиатуры и выводит цифры из которого оно состоит. Например : Считываеться число 54698
        Выводиться:
        5
        4
        6
        9
        8*/
			
			int enterNumber;
			int firstNumber;
			int secondNumber;
			int thirdNumber;
			int fourthNumber;
			int fifthNumber;
			int b,c,d;
			
			Scanner sc = new Scanner(System.in);
			System.out.println("Enter the five-digit number and press ENTER: ");
			
			enterNumber = sc.nextInt();
			String transformation = Integer.toString(enterNumber);
			
			if (transformation.length() != 5){
				System.out.println("You entered is not a five-digit number!");
			}else{
			firstNumber = enterNumber/10000;
			b = enterNumber%10000;
			secondNumber = b/1000;
			c = b%1000;
			thirdNumber = c/100;
			d = c%100;
			fourthNumber = d/10;
			fifthNumber = d%10;
			
			System.out.println(firstNumber);
			System.out.println(secondNumber);
			System.out.println(thirdNumber);
			System.out.println(fourthNumber);
			System.out.println(fifthNumber);
			
			}
			
	}

}
