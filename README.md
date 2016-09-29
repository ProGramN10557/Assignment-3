public class Assignment3 {
	// assignments
	/**
	 * Write a method to find N numbers which are power of three. e.g. n=4,
	 * return {1,3,9,27}
	 */
	public int[] findPowerOfThree(int n) {
		if (n < 1) {
			return null;
		}
		int num = 3; 
		int array[] = new int[n];
		array[0] = 1;
		for(int i = 1; i < n; i++) {
	             array[i] = array[i-1] * num;
		  }
	
		return array;
	}

/**
