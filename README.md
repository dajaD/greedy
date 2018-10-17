# greedy
// program on how to use greedy algorithm using curreny
//program creates change for the given amount

public class MyClass {
    public static void main(String args[]) {
        
      int total = 10022;
      int currency[] = {100,50,20,10,5,1}; //the shortest way to convert the currency to the total amount
      int moneyy;
      
      for(int i =0; i<currency.length; i++)
      {
          
          if (currency[i] <= total)
          {
              moneyy = total/currency[i];
              System.out.println(moneyy +" "+ "$"+ currency[i]);
              total -= moneyy*currency[i];
          }
      }
      
    }
}
