# towerofhanoi

public class recursion {
    public static void towerOfHanoi(int n, String sorc, String temp , String dest){
        if(n==1)
        {
           System.out.println("transfer disk " +n + " from "+sorc+" to "+dest);
           return ;
        }
        
        towerOfHanoi( n-1 , sorc , dest , temp);
         System.out.println("transfer disk " +n + " from "+sorc+" to "+dest);
        towerOfHanoi( n-1 , temp , sorc , dest);
    }
    public static void main(String[] args) {
    int n = 3;
    
   towerOfHanoi(n, "s", "t","d");
    
    }
}
