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
   
   
