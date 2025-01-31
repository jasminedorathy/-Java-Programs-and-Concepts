##DOUBLY LINKED LIST
````java[]
import java.util.Scanner;

class Node
{
    int data;
    Node next;
    Node prev;

    Node(int data)
    {
        this.data = data;
        this.next = null;
        this.prev = null;
    }
}
class Dll {
    Node head, tail;

    public void InsertAtBegin(int data) {
        Node newNode = new Node(data);
        if (head == null) {
            head = tail = newNode;
        } else {
            newNode.next = head;
            head.prev = newNode;
            head = newNode;
        }
    }

    public void InsertAtEnd(int data) {
        Node newNode = new Node(data);
        if (tail == null) {
            tail = head = newNode;
        } else {
            tail.next = newNode;
            newNode.prev = tail;
            tail = newNode;
        }
    }

    public void deleteAtBegin() {
        if (head != null) {
            head = head.next;
            head.prev = null;
        }
    }

    public void deleteAtEnd() {
        Node temp = tail;
        tail = tail.prev;
        temp.next = null;
        tail.next = null;


    }




public void insert(int data, int pos) {
    Node newNode = new Node(data);
    Node temp = head;
    for (int i = 0; i < pos - 1; i++) {
        temp = temp.next;

    }

    newNode.next = temp.next;
    if(temp.next !=null){

    newNode.next.prev = newNode;
    }
    temp.next=newNode;
    newNode.prev = temp;

}
 public void reverse()
 {
     Node current = head;
     Node next = null;
     Node prev = null;

     while(current!=null)
     {
         next = current.next;
         current.next = prev;
         prev = current;
         current = next;
     }
     head = prev;
 }




            public void display()
            {
                Node temp = head;
                if(temp == null)
                {
                    System.out.println("List is Empty");
                }
                if(temp != null)
                {
                    //System.out.println("<->" + temp.data);
                    while (temp != null)
                    {
                        System.out.print(temp.data + "<->" );
                        temp = temp.next;

                    } System.out.print( "null" );
                    //temp = temp.next;
                }

                System.out.println();
            }
        }





public class Doubly {
    public static void main(String args[])
    {
        //Scanner sc = new Scanner(System.in);
        Dll doub = new Dll();
        doub.InsertAtBegin(100);
        doub.InsertAtBegin(200);
        doub.InsertAtBegin(300);
        doub.InsertAtEnd(400);
        doub.InsertAtEnd(500);
        doub.InsertAtEnd(600);
        doub.deleteAtBegin();
        doub.deleteAtEnd();

        doub.insert(23,3);
        doub.reverse();


        doub.display();
    }
}
OUTPUT:
500<->23<->400<->100<->200<->null

````
