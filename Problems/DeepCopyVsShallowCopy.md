# What's the difference between deep and shallow copy?
=> Reference:  https://www.cs.utexas.edu/~scottm/cs307/handouts/deepCopying.htm
<br>
When creating copies of arrays or objects one can make a deep copy or a shallow copy. This explanation uses arrays.
Recall array variables in Java are references or pointers. <br>

=> A shallow copy can be made by simply copying the reference. <br>
 For example: <br>
public class Ex{
    private int[] data;
    public Ex(int[] values){
        data = values;
    }
    public void showData(){
        System.out.println( Arrays.toString(data) );
    }
}
The above code shows shallow copying. data simply refers to the same array as vals. <br>

=>A deep copy means actually creating a new array and copying over the values.<br>
For example: <br>

public class Ex{
    private int[] data;
    public Ex(int[] values){
        data = new int[values.length];
        for(int i = 0; i < data.length; i++)
            data[i] = values[i];
    }
    public void showData(){
        System.out.println( Arrays.toString(data) );
    }
}

The above code shows deep copying.






