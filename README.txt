COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		Yes, it was slightly slower overall but more efficient with handling insertions and removals for a bigger list.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			This removes the element at index 5 in the list.

		list.remove(Integer.valueOf(5)); // what does this one do?

			This removes the object 5 the first time it occurs in the list. 

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			It modifies the list directly and while iterating it can cause an error since it modifies the collection outside the iterators control.

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  163ms 99ms 105ms val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: 38ms 34ms 36ms val4 val5 val6
		testArrayListAccess:     23ms 24ms 20ms val4 val5 val6
        testLinkedListAccess:    22ms 20ms 17ms val4 val5 val6

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  124ms 105ms 113ms val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: 43ms 34ms 41ms val4 val5 val6
		testArrayListAccess:     44ms 21ms 30ms val4 val5 val6
        testLinkedListAccess:    41ms 33ms 38ms val4 val5 val6

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  338ms 219ms 210ms val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: 61ms 31ms 30ms val4 val5 val6
		testArrayListAccess:     36ms 22ms 21ms val4 val5 val6
        testLinkedListAccess:    555ms 293ms 293ms val4 val5 val6

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  1592ms 1708ms 1638ms val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: 41ms 39ms 38ms val4 val5 val6
		testArrayListAccess:     33ms 36ms 26ms val4 val5 val6
        testLinkedListAccess:    4162ms 5026ms 4395 val4 val5 val6

	listAccess - which type of List is better to use, and why?

		Arraylist is better because it is quicker to access the list given a bigger size despite being slower at add/remove with larger sizes.

	listAddRemove - which type of List is better to use, and why?

		LinkedList is much better for AddRemove because it is much faster even with larger sizes.
