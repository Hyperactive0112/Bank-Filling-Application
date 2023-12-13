# Bank-Filling-Application

package methods;

public class BankApplication {
	
	static int currentBalance = 1000;
	public static void greetCustomer() {
		System.out.println("Hello welcome to banking application");
		
	}
	
	public void deposit(int amount) {
		currentBalance = currentBalance + amount;
		System.out.println("Amount deposited successfully");
		
	}
	
	public static void withdrawal(int amount) {
		currentBalance = currentBalance - amount;
		System.out.println("Amount withdrawal successfully");
		
	}
	
	public int getcurrentBalence() {
		return currentBalance;
		
		
	}
	
	public static void main(String[] args) {
		BankApplication bank = new BankApplication();
		greetCustomer();
		System.out.println("current balance is : "+ bank.getcurrentBalence());
		bank.deposit(500);
		System.out.println("current balance is : "+ bank.getcurrentBalence());
		withdrawal(100);
		System.out.println("current balance is : "+ bank.getcurrentBalence());
		
	}

}
