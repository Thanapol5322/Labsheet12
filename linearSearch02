import java.util.LinkedList;
import java.util.Random;
import java.util.Scanner;

// Exercise No.4
public class linearSearch02 {

	public static void main(String[] args) {
		
		LinkedList<Integer> nums = new LinkedList<Integer>();
		nums = random_initial();
		
		System.out.print("Elements : ");
		
		for (int num : nums) {
			
			System.out.print(num + " ");
			
		}
		
		// Convert LinkedList<integer> to int[] from linearSearch().
		int[] array = new int[nums.size()];
		for (int i = 0; i < nums.size(); i++) {
			
			array[i] = nums.get(i);

		}

		Scanner input = new Scanner(System.in);
		System.out.print("\n\nEnter target: ");
		int target = input.nextInt();
		
		int index = linearSearch(array, target);

		if (index != -1) {

			System.out.println("The target (" + target + ") at index " + index);

		} else {

			System.err.println("Cannot found " + target + " in this linked list");

		}

	} // End of main()
	
	public static LinkedList<Integer> random_initial() {
		
		Random rnd = new Random();
		LinkedList<Integer> nums = new LinkedList<Integer>();
		
		for (int i = 0; i < 10; i++) {
			
            nums.add(rnd.nextInt(100));
            
        } // End of for.
		
		return nums;
		
	} // End of random_initial()
	
	public static int linearSearch(int[] nums, int target) {
		
		for (int i = 0; i < nums.length; i++) {
			
			if (target == nums[i]) {
				
				return i;
				
			}
			
		} // End of for.
		
		return -1;
		
	} // End of linearSearch()
	
} // End of class.
