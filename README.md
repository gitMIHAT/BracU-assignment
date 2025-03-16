import java.util.Scanner;
public class quesbank1{
  public static void main (String[]args){
    Scanner sc = new Scanner (System.in);
    System.out.println("Vehicle Speed:");
    int Speed = sc.nextInt();
    System.out.println("Speed Limit: ");
    int speedlimit = sc.nextInt();
    System.out.println("Past Violations:");
    int vio = sc.nextInt();
    int n1= 50;
    int n2= 150 ;
    int n3 = 500 ;
    if (vio >=2){
      int ex = 2;
      n1 *= ex ;
      n2 *=ex;
      n3 *= ex;
    }
    if(Speed > speedlimit ){
       int excced = Speed - speedlimit;
       if (excced <=10){
         System.out.println( "The fine is:$"  + n1  ) ;
       }
       else if (excced <=30){
         System.out.println( "The fine is:$" + n2 ) ;
       }
       else if (excced >30){
          System.out.println( "The fine is:$" + n3 + " along with a lisence suspention ") ;
       }
   }
    else {
      System.out.println ("Under Speed Limit");
    }
 }
}  
   
