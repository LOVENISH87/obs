# so hasshmap is storage that stores in key val pairs man!!!
[[batman]]
[[node +   mongo]]

hash_map is *locker room* ->  
- [?] key is the locker number
	- [?] value is the data that we had inserted !!!
		- [?] hash function decides which locker number to use
			- [?] fast <mark style="background: #FFB86CA6;">lookup</mark> and insertion -> <mark style="background: #ADCCFFA6;">putting someting inside</mark> time O(1)

```cpp
#include <hashmap.h>
main(){
unordered_map <string, int> mp;

%% now for insert adding vals in hmp %%

mp[key] = value;


}
```


  this is for init map => => **map<_keytype, valuetype_> _mapName_**
. [node]



# C++ maps are mutable, meaning we can add, modify, or delete elements.

- yes we can iterate through maps using loops!!!! - but this is not same as iterating through vectors !!!
- because in maps we need to deal with pairs!!! `.first` and `.second` 
````cpp
    // Iterate through the map and print all key-value pairs
    for (const auto& pair : student_age) {
        std::cout << pair.first << ": " << pair.second << std::endl;
    }
````

- here we use range based loop to iterate the pair!!!
- where pair.first holds the key  and pair.second holds the value!!!
- You’re using:

`unordered_map<string, int>`

An `unordered_map`:
- **Does NOT preserve insertion order**
- **Does NOT sort**
- Stores elements in **hash buckets**
- Iteration order depends on the hash function + internal layout
# sort order depends upon the key no matter what the value is!!!
 - Your keys are strings, so they’re sorted **lexicographically (alphabetical order)**.


| Container       | Order behavior                |
| ----------------------- | ------------------------------------- |
| unordered_map | ❌ no order (hash-based chaos) |
| Map           | ✅ sorted by key               |
| set           | ✅ sorted by value             |
| vector        | ✅ insertion order             |


