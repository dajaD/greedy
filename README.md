# greedy
// program on how to use greedy algorithm using curreny
//program creates change for the given amount

public class MyClass {
    public static void main(String args[]) {
        
      int total = 1000;
      int currency[] = {1,5,10,20,50,100}; //the shortest way to convert the currency to the total amount 100*10
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
