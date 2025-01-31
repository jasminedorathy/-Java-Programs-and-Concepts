STACK IMPLEMENTAION USING ARRAYS:
````java[]

public class Stack {
    int a[] = new int[5];
    int top = -1;

    // push
    void push(int data) {


        if (top == a.length - 1) {
            System.out.println("Stack is full");
        } else {
            top++;
            a[top]=data;
        }
    }

    //pop
    void pop() {


        if (top == -1) {
            System.out.println("Stack is empty");
        } else {
            top--;
        }
    }

    void peak() {
        if (top == -1) {
            System.out.println("Stack is empty");
        }
        else {
            System.out.println("The top of the element" + a[top]);
        }
    }

    void display()
    {
        for(int i=top;i>=0;i--)
        {
            System.out.println("Displaying the elements present"+a[i]);
        }
    }



        public static void main(String [] args)
        {
            Stack s = new Stack();
            s.push(10);
            s.push(20);
            s.push(30);
            s.push(40);
            s.push(50);
            s.pop();
            s.peak();
            s.display();


        }

}


OUTPUT:
The top of the element20
Displaying the elements present20
Displaying the elements present30
Displaying the elements present40
Displaying the elements present50

````
