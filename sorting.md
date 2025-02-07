## BUBBLE SORT

````java[]

import java.util.Arrays;

public class bubblesort {
    public static void main(String args[])
    {
        int arr[]={2,0,2,1,1,0};
        Bubble(arr);
    }
    public static void Bubble(int arr[])
    {
        for(int i=0;i<arr.length;i++)
        {
            for(int j=0;j<arr.length-1-i;j++)
            {
                if(arr[j]>arr[j+1])
                {
                      int temp = arr[j];
                      arr[j] = arr[j+1];
                      arr[j+1] = temp;
                }
            }
        }
        System.out.println(Arrays.toString(arr));
    }
}

OUTPUT:

[0, 0, 1, 1, 2, 2]

````
