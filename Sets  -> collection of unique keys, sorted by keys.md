<h1>this is some cool tricks i get to know while working with Sets</h1> 

<h1> unordered_map {two int, int}  </h1> <h1>unordererd_set{only one int})</h1>


<h1>cool stuff: </h1>
1️⃣  – _“creating a place for the club”_
```cpp

creating a set->  
unordered_set<int> st;  <- creating a set {empty}...
 
```

2️⃣ `insert()` <-< try to enter in club!!!
```cpp
st.insert(4);
st.insert(44);
st.insert(4);   
```
cool thing is you can enter only one item in set!!

3`find()` <- finding if that thing is present in set
```cpp
if(st.find(5) != st.end){
	cout << "5 is present!!!";
}
```
- this use iterators under the hood ->
	- like if it finds it tells if not it will move to the end and it won't find it


<span style="color:red">all about find </span> 
- *find is a complex function*
- *it returns a thing called* "ITERATORS" -> *pointing to the set's element.*
- <mark class="hltr-red">let's just say that if the `find` method doesn't find the element</mark>,
		it returns a thing which is equal to `set.end()`.


# also we can use COUNT function it does the same thing because
in set all the elements can have `0 or 1` count, it means every element in set is unique so if its present or not!!
syntax-> 

```cpp
set<int> st;
if(st.count(4) > 0){
		cout << "element is present!! " // if it actually is else not present!!! 
	//todo: try with boolean 
}
```


we can use for Range loop for traversal

```cpp
#include <set>
#include <iostream>

int main() {
    std::set<int> mySet;

    mySet.insert(20);
    mySet.insert(10);
    mySet.insert(30);

    // Print all elements
    for (int item : mySet) {
        std::cout << item << " ";  // Output: 10 20 30 
    }

    return 0;
}
```

# Note that the set always stores elements in the ascending order.

# The set can only have one instance of each element, so `.count` will always return either `0` or `1`.

# Define, add, remove, and check elements in a set using `insert`, `erase`, `find`, and `count`.

# Use iterators to loop through set elements.
