# selection-sort
selection sort using for loop in java
package javaproject;

public class selectionsort {

	public static void main(String[] args) {
		int i,j;
		int arr[]= {34,1,89,32,46};
		for(i=0;i<=arr.length-1;i++)
		{
			int max_index=0;
			for(j=0;j<arr.length-1-i;j++) {
				if(arr[max_index]<arr[j])
					max_index=j;
			}
		int temp=arr[arr.length-1-i];
		arr[arr.length-1-i]=arr[max_index];
		arr[max_index]=temp;
		}
		for(i=0;i<=arr.length-1;i++)
			System.out.println(arr[i]);
	}

}
