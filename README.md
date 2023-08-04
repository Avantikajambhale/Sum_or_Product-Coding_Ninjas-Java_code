# Sum_or_Product-Coding_Ninjas-Java_code
import java.util.* ;
import java.io.*; 
public class Solution {

	public static long sumOrProduct(int n, int q) {
		long sum=0;
		long pro=1;
		long m = 1000000007;

		// Write your code here
		if(q==1){
			for(int i=1; i<=n; i++){
				sum = sum+i;
			}
			return sum;
		}
		else if(q==2){
			for(int i=1; i<=n; i++){
				pro = (pro*i)%m;
			}
			return pro;
		}
		return -1;
	}
}
