# Java_DSA_Problem-
Find the number of rotations in a circularly sorted array
Given a circularly sorted integer array, find the total number of times the array is rotated. Assume there are no duplicates in the array, and the rotation is in the anti-clockwise direction.

Input:  nums = [8, 9, 10, 2, 5, 6]
Output: The array is rotated 3 times



// first Method is just to find the index of the minimum element of the array. Here is my Java code for the same :
import java.util.*;
public class Main
{  
    static int countRotation(int[] arr){
        int min=arr[0],index=0;
        for(int i=0;i<arr.length-1;i++){
            if(min>arr[i]){
                min =arr[i];
                index=i;
            }
        }
        return index;
    }
	public static void main(String[] args) {
		int [] nums ={8,9,10,2,5,6};
	    System.out.println(countRotation(nums));
	}
}


