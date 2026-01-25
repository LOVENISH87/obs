 - return -> 


- sequence is -> 
	- n:   0 1 2 3 4 5 6
	- F(n):0 1 1 2 3 5 8
	  
	  
<span style="color:rgb(0, 176, 80)">To solve the problem, I ask the same problem again.</span> 
 <h5 style= 'text-green'>
 Think of it like climbing stairs:

To reach step `n`, you must first reach step `n-1`."
</h5>
<a>fib(n) = fib(n-1) + fib(n-2) </a>

[[fib limitations]]
this one is view!!!

<span style="color:red ">
<br>summary</span>

-  ❌ Simple recursion

- **Works**
    
- **Very slow**
    
- **Repeats calculations**
    

### ✅ Memoized recursion

- **Fast**
    
- **Same speed as iterative**
    
- **Uses extra memory**
