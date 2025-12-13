[[CPP again]]


perfix sum [in simple words its the running sum of the elements of the array ] ->

<mark style="background: #BBFABBA6;">int array = [2, 3, -1, 4];</mark>

| index | value | prefix sum |
| :---: | :---: | :--------: |
|   0   |   2   |     2      |
|   1   |   3   |     5      |
|   2   |  -1   |     4      |
|   3   |   4   |     8      |
perdis[i]  = perdx[i-1] + arr[i]
formula to calculate prefix sum  <mark style="background: #BBFABBA6;">isprefix[i] = prefix[i-1] + arr[i]</mark>

