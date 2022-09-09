###  [Task 8kyu](https://www.codewars.com/kata/57cc975ed542d3148f00015b)

You will be given an array a and a value x. All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either.

Return true if the array contains the value, false if not.

### My solution
```Java
public class Solution {

public static boolean check(Object[] array, Object value) {
for (int i = 0; i < array.length; i++) {
if (array[i].equals(value)) return true;
}
return false;
}

}
```

### Fav solution

```Java
import java.util.Arrays;

public class Solution
{

    public static boolean check(Object[] a, Object x)
    {
        return Arrays.stream( a )
                .anyMatch( e -> e == x );
    }

}
```
I like this solution because I like it
