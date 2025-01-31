## QUEUE IMPLEMENTATION USING ARRAY

````JAVA[]

public class Queue {
    int a[] = new int[5];
    int rear=-1,front= -1;

    // enqueue
    void enqueue(int data) {


        if (rear==a.length-1)
        {
            System.out.println("Queue is full");
        }
        else {
            if(front == -1)
            {
                front = 0;
            }

            rear++;
            a[rear]=data;
        }
    }

    //dequeue
    void dequeue() {


        if (front == -1 || front>rear) {
            System.out.println("Queue is empty");
        } else {
            front++;
        }
    }


    //peak
    void peak() {


        System.out.println("The top of the element" + a[front]);

    }


    //display
    void display()
    {
        for(int i=front;i<=rear;i++)
        {
            System.out.println("Displaying the elements present"+a[i]);
        }
    }



    public static void main(String [] args)
    {
        Queue s = new Queue();
        s.enqueue(10);
        s.enqueue(20);
        s.enqueue(30);
        s.enqueue(40);
        s.enqueue(50);
        s.dequeue();
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
