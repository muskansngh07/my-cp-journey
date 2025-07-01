### Question 
An elephant decided to visit his friend. It turned out that the elephant's house is located at point 0 and his friend's house is located at point x(x > 0) of the coordinate line. In one step the elephant can move 1, 2, 3, 4 or 5 positions forward. Determine, what is the minimum number of steps he need to make in order to get to his friend's house.

### Code
```java
import java.util.*;
import java.io.*;
public class Main
{
    public static void main(String args[])throws IOException
    {
       BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
       int x=Integer.parseInt(br.readLine());
       int steps = x / 5;
        if (x % 5 != 0) {
            steps++;
        }
 
        System.out.println(steps);
    }
}
