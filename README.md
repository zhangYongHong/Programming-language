# JavaTest

**code**
public class arrays {
	
	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
         int[]  a = {1,2,3,4,5};
         int[] l = {1001,1002,1003,1004,1005};
         System.arraycopy(a, 2, l, 2, 3);
         for(int i=0; i<l.length; i++)
        	 System.out.println(i + ": "+ l[i]);
         }
}

**result**
0: 1001
1: 1002
2: 3
3: 4
4: 5

----------------------------------------
import java.util.Scanner;


public class test {

	/**
	 * @param args
	 */
	
	public static void main(String[] args) {
		
		Scanner in = new Scanner(System.in);
		int NMAX = in.nextInt();
		int i, j, k;
		int[][] odds = new int[NMAX][];
		for(i=0; i<NMAX; i++){
			odds[i] = new int[i+1];
		}
		
		for(i=0; i<odds.length; i++){
		for(j=0; j<odds[i].length; j++){
				
				int lottterOdds= 1;
				for(k=1; k<=j; k++)
	                        lottterOdds = lottterOdds*(i-k+1)/k;             
	             odds[i][j] = lottterOdds;			
			}
		}
	    	a
		    for(int[] row : odds){
	    		for(int odd:row)
	    		     System.out.printf("%4d", odd);
	    		System.out.println();
	    	}
	}
}


