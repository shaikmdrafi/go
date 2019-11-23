# Variable Declaration

```
package main

import "fmt"

func main() {
// Type-1 Declaration
        i := 42
// Type-2 Declaration
        var j int
        j = 52
// Type-3 Declaration
        var k int = 62
        fmt.Println(i)
        fmt.Println(j)
        fmt.Println(k)

}

```


# For Loop

```
package main

import "fmt"

func main() {
	for i := 0; i < 5; i++ {
	fmt.Println(i)
	}
}
```

# Math Operations

```
package main

import "fmt"

func main() {
	x := 5
	y := 7
	var sum int = x + y
	fmt.Println(sum)
}
```

# If condition

```
package main

import "fmt"

func main() {
	x := 4
	if x >= 6 {
		fmt.Println("x value is more than or equal to 6")
	} else if x <= 2{
		fmt.Println("x value is less than or equal to 2")
	} else {
		fmt.Println("x value is in between 3 and 5")
	}
	
}
```

# Array's
```
package main

import "fmt"

func main() {
	var a [5]int
	fmt.Println(a)

	var b [5]int
	b[2] = 10 
	fmt.Println(b)
	
	c := [6]int{10,20,70,90,5,15}
	fmt.Println(c)
	
	d := []int{1,2,3,4,5,6,7,8,9}
	fmt.Println(d)
	
	d = append(d,10)
	fmt.Println(d)
}
```
