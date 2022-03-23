# Write-a-program-to-sort-a-numeric-array-element-in-ascending-order
import java.util.*;
import java.util.Scanner;

public class A1_Ex10 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.print("Enter Number of elements in array:");
		Scanner sc=new Scanner(System.in);
		int n;
		n=sc.nextInt();
		System.out.println("Enter elements in array:");
		int a[]=new int[n];
		for(int i=0;i<n;i++)
		a[i]=sc.nextInt();
		int temp;
		for(int i=0;i<n;i++) {
			for
			(int j=i+1; j<n; j++) {
			if(a[i]>a[j]) {
			temp=a[i];
			a[i]=a[j];
			a[j]=temp;
			}
			}
			}
			System.out.println("Sorted Array is:");
			for(int i=0;i<n;i++)
			System.out.print(a[i]+" ");

		}
	}
