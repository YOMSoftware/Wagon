import java.util.ArrayList;
import java.util.List;

public class ListEdit {

	public static void main(String[] args) {
		int sum = 0;
		// create an array list
		List<Integer> al = new ArrayList<Integer>();
		List<Integer> rmList = new ArrayList<Integer>();
		System.out.println("Initial list");

		// add elements to the array list
		al.add(4);
		al.add(1);
		al.add(2);
		al.add(9);
		al.add(4);
		al.add(1);
		al.add(2);
		al.add(9);
		al.add(10);
		al.add(10);
		al.add(8);
		al.add(11);
		al.add(7);
		al.add(12);
		al.add(10);
		al.add(6);
		al.add(0, 6);

		for (int x : al) {
			System.out.println(x);
		}

		while (al.isEmpty() == false) {
			System.out.println("Current max = " + FindMax(al));

			if (sum + FindMax(al) > 14) {
				System.out.println();
				rmList.add(sum);
				sum = 0;
			} else {
				sum = sum + FindMax(al);
			}

			System.out.println("sum = " + sum);
			al.remove(Location(al, FindMax(al)));

			System.out.println("After:");
			for (int x : al) {
				System.out.println(x);
			}
		}
		rmList.add(sum);

		System.out.println("Removed list");
		for (int x : rmList) {
			System.out.println(x);
		}
	}

	public static int FindMax(List<Integer> array) {
		Integer list2[] = new Integer[array.size()];
		list2 = array.toArray(list2);

		int max = list2[0];
		for (int x : list2) {
			if (x > max) {
				max = x;
			}
		}

		return max;

	}

	public static int Location(List<Integer> array, int key) {
		Integer list2[] = new Integer[array.size()];
		list2 = array.toArray(list2);

		int position = -1;

		for (int i = 0; i < list2.length; i++) {
			if (key == list2[i]) {
				position = i;
			}
		}
		return position;
	}

	/*
	 * public static void Update(int array[]) { sum = sum +
	 * array[Location(array, FindMax(array))]; System.out.println("sum: " +
	 * sum); }
	 */

}
