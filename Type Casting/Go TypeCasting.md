# Go Type Casting

### Casting

- conversion of a variable from one data type to another
- value may be lost when large type is converted to a smaller type
- Implicit type conversion is not there in go

```go
//Example 
package main  
import (  
   "fmt"  
   "strconv"  
)  
func main() {  
  
   var i int = 10  
   var f float64 = 6.44  
   var str1 string = "101"  
   var str2 string = "10.123"  
  
   fmt.Println(float64(i))  
   fmt.Println(int(f))  
  
   newInt, _ := strconv.ParseInt(str1, 0, 64)  
   fmt.Println(newInt)  
  
   newfloat, _ := strconv.ParseFloat(str2, 64)  
   fmt.Println(newfloat)  
}
/*
Output 
10 
6
101
10.123
*/
```

---
