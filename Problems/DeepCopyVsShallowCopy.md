# What's the difference between deep and shallow copy?
=> Reference:  
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

