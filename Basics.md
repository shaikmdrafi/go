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

# If Condition

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

# String Mapping

```
package main

import "fmt"

func main() {
	vertices := make(map[string]int)
	
	vertices["traingle"] = 2
	vertices["square"] = 3
	vertices["polygon"] = 5
	
	fmt.Println(vertices)
	fmt.Println(vertices["square"])
	
	delete(vertices, "traingle")
	fmt.Println(vertices)
}
```

# Loop with Array

```
package main

import "fmt"

func main() {
	arr := []string{"a","b","c"}
	for index, value := range arr{
		fmt.Println("index:", index, "value:", value)
	}	
}
```

```
package main

import "fmt"

func main() {
	m := make(map[string]string)
	m["a"] = "alpha"
	m["b"] = "beta"
	
	for key, value := range m {
		fmt.Println("key:", key, "value:", value)
	}
}
```


# Custom Fucntions
```
package main

import (
	"fmt"
)

func main() {
	result := sum(16,14)
	fmt.Println(result)
}

func sum(x int, y int)int {
	return x + y
	}
```

### Go functions can have multiple return value
```
package main

import (
	"fmt"
	"errors"
	"math"
)

func main() {
	result, err := sqrt(16)
	if err != nil {
		fmt.Println(err)
	} else{
		fmt.Println(result)
		}
}
	
func sqrt(x float64) (float64, error){
	if x < 0 {
		return 0, errors.New("Undefined for Negative Numbers")
		}
	return math.Sqrt(x), nil
}
```

# Struct (collection of fields)
```
package main

import (
	"fmt"
)

type person struct {
	name string
	age int
	}

func main(){
	p := person{name: "shaik", age: 28}
	fmt.Println(p)
	fmt.Println(p.name)
	fmt.Println(p.age)
}
```

# Pointers

```
package main

import (
	"fmt"
)

func main (){
	i := 8
	fmt.Println(&i)
	inc(&i)
	fmt.Println(i)
}


func inc(x *int){	// Prefixing type with Astric
	*x++		// Referncing Pointer
}
```
