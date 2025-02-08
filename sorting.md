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

## Insertion Sort

````java[]
import java.util.*;
public class insertionsort {
    public static void main(String[]args)
    {
        int arr[] = {3,1,4,5,2};
        Insertion(arr);
    }
    public static void Insertion(int arr[])
    {
        for(int i=0;i<arr.length-1;i++)
        {
            for(int j=i+1;j>0;j--)
            {
                if(arr[j]<arr[j-1])
                {
                    int temp = arr[j];
                    arr[j] = arr[j-1];
                    arr[j-1] = temp;
                }
            }
        }
        System.out.println(Arrays.toString(arr));
    }
}

OUTPUT:

[1,2,3,4,5]

````
