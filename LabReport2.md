Part 1:
```
import java.io.IOException;
import java.net.URI;
import java.util.*;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String x1="";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            x1+=parameters[1]+"\n";
            return x1;
        } 
        return "404 not found";
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("no string");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```


<img width="774" alt="截屏2023-01-29 下午11 22 39" src="https://user-images.githubusercontent.com/122562034/215562008-d0b7587e-cdae-40fd-b077-bdee16ad8c3d.png">
1. The method handleRequest is called
2. The argument is  [http://localhost:4001/add-message?s=and] , and the value is "and"
3. The value "and" is added to the list, so previously there's only one value in the list and get returned, but now there are two values which includes "and"


<img width="735" alt="截屏2023-01-29 下午11 22 50" src="https://user-images.githubusercontent.com/122562034/215562780-e1b2da36-47cb-4874-8123-66919ecc70e6.png">

1. The method handleRequest is called
2. The argument is http://localhost:4001/add-message?s=hihi, and the value is "hihi"
3. The value "hihi" is added to the list, so previously there are two values in the list and get returned, but now there are three values which includes "hihi"



Part2:
The bug I choose is the method reverseInPlace in ArrayExamples
A failure-inducing input: 
```
public class ArrayTests {
   @Test 
	public void testReverseInPlace() {
    int[] input1 = { 3,4,5,6,7 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 7,6,5,4,3 }, input1);
	}

}
```

An input that doesn’t induce a failure:
```
public class ArrayTests {
   @Test 
	public void testReverseInPlace() {
    int[] input1 = { 1 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 1 }, input1);
	}

}
```


<img width="990" alt="截屏2023-01-30 上午10 43 18" src="https://user-images.githubusercontent.com/122562034/215566696-6e407e18-489a-4ab7-8597-0adf80500ca9.png">

The Bug:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }

```

After fix it:
```
static void reverseInPlace(int[] arr) {
    int [] newarray=new int[arr.length];
    for(int i = 0; i<arr.length; i += 1){
      newarray[i]=arr[i];
    }
    for(int i = 0; i<arr.length; i += 1) {
      arr[i] = newarray[newarray.length-1-i];
    }
  }
```

I create another array called newarray to store the arr. So that if we change arr, we won't change the original order of the arr. We can loop from the back to the first in the correct order.

Part 3:
I learned what is a bug and what is symptom, and what's the difference between the two. I also learned how to create a local web server, and how to distinugish between path, domain, port. 







