# Apple-and-Orange
Hackerrank Problem Solution in java
import java.util.Scanner;

public class AppleAndOrange {
	
	 static int apple(int s, int t, int a,int app[]) {
		 int ac = 0;
		 
		 for (int i = 0; i < app.length; i++) {
			if(a + app[i] >= s && a + app[i] <= t) {
				    ac++;
			}
		}
		 return ac;
	 }
	 static int orange(int s,int t, int b,int or[]) {
		 int oc = 0;
		 
		 
		 for (int j = 0; j < or.length; j++) {
				if(b + or[j] >= s && b + or[j] <= t) {
					    oc++;
				}
			}
		 
		 return oc;
	 }

	public static void main(String[] args) {
         Scanner scan = new Scanner(System.in);
         int s = scan.nextInt();
         int t = scan.nextInt();
         
         int a = scan.nextInt();
         int b = scan.nextInt();
        
         int m = scan.nextInt();
         int n = scan.nextInt();
         int app [] = new int [m];
         int or [] = new int[n];
         for (int i = 0; i <app.length; i++) {
			   app[i]  = scan.nextInt();
		}
         for (int j = 0; j <or.length; j++) {
			   or[j]  = scan.nextInt();
		}
         
         
         System.out.println(apple(s,t,a,app));
        System.out.println(orange(s,t,b,or));
        
        
         
        
		}
	}
