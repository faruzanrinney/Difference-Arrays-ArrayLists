# Difference-Arrays-ArrayLists
The difference between arrays and array lists in Java are that while arrays are fixed in size, array lists allow more flexibility by having the ability to add and remove elements. In Java, arrays are data structures that store sequences that are fixed in size of elements of the same data type. Arrays are objects in Java, so they can be assigned to a variable, passed as a parameter to a method, and returned as a value from a method. Arrays in Java are also zero-indexed, which means the first element of an array automatically has an index of 0, and so the second element has an index of 1 and so on. The length of an array is set when created and cannot be changed later.&nbsp;Arrays in Java can store elements of any data type, which include primitive types such as int, double, and boolean. They can also store object types such as Strings and Integers. Arrays can be multi-dimensional (they have multiple rows and columns). Arrays are most commonly used to store collections of data, such as numbers, sets of strings, or a series of objects.&nbsp;

Array lists are a class in Java that can be used to store lists or objects like an array, however there are several key problems regarding arrays. While arrays require specifications for a size, as well as not being able to change it after being created, sometimes the size array won't be revealed the instant you create the array, causing confusion and frustration. The second difference is that while it is possible to resize arrays by creating a new and larger array and copying data over from the old array, this results in very clunky and awkward coding. Java ArrayLists classes are there to provide a class that can replicate the many features of arrays, while also adding some new features that are made to work around the problems listed above regarding normal arrays.&nbsp;


// import the ArrayList package
import java.util.ArrayList;
// import the Array package
import java.util.Arrays;


// this will be the Java array
public class DifferenceArraysArrayLists {
    public static void main(String[] args) {

	
    	// Array of object references:
    	String[] family = new String[] {"Meg", "Lois", "Peter", "Chris", "Stewie", "Brian"};
    	
    	System.out.println("java array: " + Arrays.toString(family));
    	
    	// Output: [Meg, Lois, Peter, Chris, Stewie, Brian]
    	System.out.println("java array with element 4: " + family[4]);
    	// Output: Stewie
    	
    	
    	// this is the array list
    	ArrayList<String> family2 = new ArrayList<String>(); // arrayList object
    	family2.add("Meg");
    	family2.add("Lois");
    	family2.add("Peter");
    	family2.add("Chris");
    	family2.add("Stewie");
    	family2.add("Brian");
        System.out.println("java array list: " + family2);
    	// Output: [Meg, Lois, Peter, Chris, Stewie, Brian]
        
        family2.add(0, "idk"); // Insert element at the beginning of the list (0)

        System.out.println("java array list with added element at 0" + family2);
    	
    			}
		}
	
		
	
	
