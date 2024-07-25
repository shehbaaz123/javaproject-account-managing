# javaproject-account-managing
import java.util.Scanner;

 class atm {
 
    float balance;
    int PIN=7890;
    void checkpin(){
     Scanner sc=new Scanner(System.in);
    System.out.println("Enter the Pincode");
    int num=sc.nextInt();
    if (num==PIN) {
        System.out.println("welcome to Menu");
        menu();
    }
    else{
        System.out.println("please enter the valid pin ");
        menu();
    }
    }



    void menu(){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter Your choice ");
        System.out.println("1.check the balance");
        System.out.println("2.Withdraw Money ");
        System.out.println("3 deposit Money ");
        System.out.println("4.Exit  ");
       int choice=sc.nextInt(); 
    
       if(choice==1){
         CheckBalance();
       }
       else if(choice==2){
        WithdrawMoney();
      }
      else if(choice==3){
     DepositMoney();
      }
      else if(choice==4){
        System.out.println("thank you :)");
        return;
      }
     else {
          System.out.println("Invalid option ");  
          menu();
          }
        
    }
  void CheckBalance(){
      System.out.println("YOUR BALANCE IS "+balance);
  menu();
  }
  void WithdrawMoney(){
   System.out.println("enter the amount to withdraw");
   Scanner sc=new Scanner(System.in);
   int amt =sc.nextInt();
   if (amt>balance) {
    System.out.println("insufficient Balance");
    menu();
   }
   else{
   balance=balance-amt;
   System.out.println("WITHDRAW DONE SUCCESSFULLY");
   System.out.println("CURRENT BALANCE: " +balance);
    menu();
   }
  }
   void DepositMoney(){
    System.out.println("enter the amount want to deposit");
    Scanner sc=new Scanner(System.in);
    int depoamt =sc.nextInt();
    balance=balance+depoamt;
    System.out.println("DEPOSIT DONE SUCCESSFULLY");
   System.out.println("CURRENT BALANCE: " + balance);
    menu();
   }

}
public class  ATMachine {
public static void main(String[] args) {
 atm obj= new atm();
 obj.checkpin();
}
    
}
