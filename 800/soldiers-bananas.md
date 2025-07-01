### Question
A soldier wants to buy w bananas in the shop. He has to pay k dollars for the first banana, 2k dollars for the second one and so on (in other words, he has to pay i·k dollars for the i-th banana).
He has n dollars. How many dollars does he have to borrow from his friend soldier to buy w bananas?

### Code
```java
import java.util.*;
import java.io.*;
public class Main
{
    public static void main(String args[])throws IOException
    {
       BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
       String []s=br.readLine().split(" ");
       int k=Integer.parseInt(s[0]);
       int n=Integer.parseInt(s[1]);
       int w=Integer.parseInt(s[2]);
       int sum=0;
       for(int i=1;i<=w;i++)
        {
           sum+=i*k; 
        }
        if(sum>n)
            System.out.println(sum-n);
        else
            System.out.println(0);
    }
}
```
#### Note
1. Demonstrates fair use of BufferedReader when inputs have to be take in a single line. 
