---
theme: geist
class: 'text-center'
highlighter: shiki
lineNumbers: true
drawings:
  persist: false
---

# Hello World

<div class="text-xl abs-br m-5 flex gap-2">
	GALILE#15
</div>

---

# Templates  
We might use **this** template to explains.

```cpp {all|1|2-5|all}
#include <stdio.h>
int main(){

	return 0;
}
```

---

# Variables
| datatype | stores             |
| -------- | ------------------ |
| `int`    | Integer            |
| `double` | Real Number        |
| `char`   | Single Charactor   |

<Note>Variable is being used to stores values!</Note>

---

# I/O  
Input/Output

| function   | usage                       |
| ---------- | --------------------------- |
| `printf()` | print out format to console |
| `scanf()`  | scan format into variables  |

<Note>To use these functions you must include `stdio.h` as header file.</Note>

---

# Examples
```cpp{all|1|2-7|all}
#include <stdio.h>
int main(){
	int n;
	scanf("%d", &n);
	printf("%d", n + 20);
	return 0;
}
```

If input is `12` the output might be `32`.

---

# Conditionals Statements

We use `if` to check that condition is true.
```cpp
if(condition){
	// do something
}
```

<Note>You can change `condition` to your own.</Note>

---

# Operator of Conditions
We can use these operators in your condition.
| Operator   | Meanings           |
| ---------- | ------------------ |
| `==`       | equals             |
| `>`        | more than          |
| `>=`       | more than or equal |
| `<`        | less than          |
| `>=`       | less than or equal |

---

# Example
```cpp{all|1-2|3|4-6|7-9|10-11|all}
#include <stdio.h>
int main(){
	int n = 20;
	if(n < 20){
		printf("Yes");
	}
	else{
		printf("No");
	}
	return 0;
}
```

In this case, output might be `No`.

---

# Loops
There are many types of loops

For Loops
```cpp
for(initialize; condition; update){
	// do something
}
```

While Loops
``` cpp
while(condition){
	// do something
}
```

---

# Loops(2)
Do While Loops
```cpp
do{
	// do something
}while(condition);
```

<Note>In most of cases, we uses `for` loops.</Note>

---

# Example

```cpp
#include <stdio.h>
int main(){
	int n = 25;
	for(int i=20; i<=n; ++i){
		printf("%d\n", i);
	}
	return 0;
}
```

In this case, output might be: 
```
20
21
22
23
24
25
```

---

---

---

# 1

```cpp
#include <stdio.h>
int main(){
	int n = 20;
	for(int i=1; i<=n; ++i){
		printf("%d\n", i);
	}
	for(int i=1; i<=n; ++i){
		for(int j=1; j<=n; ++j)
			printf("*");
	}
	return 0;
}
```

---

# 2

```cpp
#include <stdio.h>
int main(){
	int n;
	scanf("%d", &n);
	for(int i=1; i<=n; ++i){
		for(int j=1; j<=n; ++j){
			printf("%c", (i == 1 || i == n || j == 1 || j == n) ? '#': '*');
		}
		printf("\n");
	}
	return 0;
}
```

---

# 3

```cpp
#include <stdio.h>
int main(){
	int n = 20;
	for(int i=n; i>=1; --i){
		printf("%d\n", i);
	}
	printf("%d", n + 20);
	if(n == 29){
		printf("90");
	}
	return 0;
}
```
