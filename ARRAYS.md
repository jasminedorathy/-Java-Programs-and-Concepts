ARRAYS

##PROGRAM 1:
''''java[]
 

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        int a [] = {11,23,3,14,52};
        for(int i=0;i<a.length;i++)
        {
            System.out.print(a[i]+ " ");
        }
         System.out.println();
        
        int max = a[0];
        int min = a[0];
        for(int i=0;i<a.length;i++)
        {
            if(max < a[i])
            {
                max = a[i];
            }
            if(min > a[i])
            {
                min = a[i];
            }
        }
         System.out.println(max);
         System.out.println(min);
        
    }
}
````


##PROGRAM 2:
````java[]

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
        boolean found = false;
        
        System.out.println("enter the target element: ");
        int target = sc.nextInt();
        for(int i=0;i<n;i++)
        {
            a[i]=sc.nextInt();
        }
        for(int i=0;i<n;i++)
        {
            if(a[i]== target)
            {
            //System.out.println("True");
            found = true;
            }
      
        }
        System.out.println(found);
        
        
        
        
    }
}

````

##PROGRAM 3
````java[]


import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
       
        
        for(int i=0;i<n;i++)
        {
            a[i] = sc.nextInt();
        }
       
        for(int i=0;i<n;i++)
        {
                for(int j=0;j<n;j++)
                {
                    if(a[i] < a[j])
                    {
                        
                    
                    int temp = a[i];
                    a[i] = a[j];
                    a[j] = temp;
                    }
                }
            
             
        }
        
        System.out.println("Elements after sorting");
        for(int i=0;i<n;i++)
        {
            System.out.println(a[i]);
        }
             
    }
             
}
````

##PROGRAM 4

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
       
        
        for(int i=0;i<n;i++)
        {
            a[i] = sc.nextInt();
        }
       
        for(int i=0;i<n;i++)
        {
                for(int j=0;j<n;j++)
                {
                    if(a[i] < a[j])
                    {
                        
                    
                    int temp = a[i];
                    a[i] = a[j];
                    a[j] = temp;
                    }
                }
            
             
        }
        
        System.out.println("The second Largest Elemrnt is : " + a[n-2]);
             
    }
             
}


_______________________________________________________________________________________________________________________________________________________________________________________-

PROGRAM 5

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
       
        
        for(int i=0;i<n;i++)
        {
            a[i] = sc.nextInt();
        }
       
        for(int i=0;i<n-1;i++)
        {
             if(a[i] == a[i+1])
             {
                System.out.println("The duplicate Element is : " + a[i]);
             }
           /
               
             
        }
        
      
             
    }
             
}

___________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 6


import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
        int b [] = new int[n];
        int c [] = new int[n+n];
        
       
        System.out.println("Enter the elements in the first array: ");
        for(int i=0;i<n;i++)
        {
         
            a[i] = sc.nextInt();
        }
       
        System.out.println("Enter the elements in the second array: ");
        for(int i=0;i<n;i++)
        {
         
            b[i] = sc.nextInt();
        }
        
        for(int i=0;i<n;i++)
        {
            c[i]=a[i];
        }
        
        for(int i=0;i<n;i++)
        {
            c[n+i]=b[i];
        }
      for(int i=0;i<n+n;i++){
    
        //System.out.println("the Merged Array is: " + Arrays.toString(c));
        System.out.println("the Merged Array is: " + c[i]);
       
      }
             
    }
             
}
______________________________________________________________________________________________________________________________________________________________________________________________

Program 7

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the number of elements: ");
        int n = sc.nextInt();
        int a [] = new int[n];
        
        for(int i=0;i<n;i++)
         {
             a[i] = sc.nextInt();
         }
        Arrays.sort(a);
       
     
       System.out.println("After removing the duplicates: ");
       for(int i=0;i<n;i++)
       {
           if(i==0 || a[i] != a[i-1])
           {
               System.out.print(a[i]);
           }
       }
       
        
             
    }
             
}

___________________________________________________________________________________________________________________________________________________________________________________________________


PROGRAM 8

PASCALS Triangle

import java.util.*;
import java.lang.*;
public class Main 
{
    public static void main(String [] args)
    {
      Scanner sc = new Scanner(System.in);
      int n = sc.nextInt();
      for(int i=1;i<=n;i++)
      {
          int value =1;
          for(int j=1;j<=i;j++)
          {
              System.out.println(value + " ");
              value = value*(i-j)/j;
          }
          System.out.println();
          
      }
      
       
        
             
    }
             
}

O/P:
5
1 
1 1 
1 2 1 
1 3 3 1 
1 4 6 4 1 


___________________________________________________________________________________________________________________________________________________________________________________________________


