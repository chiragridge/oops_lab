import java.util.Scanner;
interface Methods{
	void divide(int x , int y);
	void modules(int x , int y);
}
class Overrides  implements Methods{
	public void divide(int x , int y ) {
		System.out.println("divide="+x/y);
	}
	public void modules(int x , int y) {
		System.out.println("modules="+x%y);
	}
}


public class Function {
public static void main(String[] args) {
	Overrides O = new Overrides();
        int a,b;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter first number");
	a=sc.nextInt();
	System.out.println("Enter second number");
	b=sc.nextInt();
     O.divide(a,b);
	O.modules(a,b);
}
}
