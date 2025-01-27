DAY 7

STRING METHODS:

PROGRAM 1(Concatenate)

public class Main
{
	public static void main(String[] args) {
	String str1 = "Hello";
	String str2 ="World";
	System.out.println(str1 + " " + str2);
		
	}
}
_________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 2(Length())

public class Main
{
	public static void main(String[] args) {
	String str1 = "Hello";
	
	int length = str1.length();
	System.out.println("The length of the string is: " + length);
	 	
	}
}

_______________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 3(CharAt method)

public class Main
{
	public static void main(String[] args) {
	String str1 = "Hello World";
	
	char ch = str1.charAt(2);
	System.out.println(ch);
	 	
	}
}

____________________________________________________________________________________________________________________________________________________________________________________________
PROGRAM 4(Boolean)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	//String str3 = IgnoreToCase(str2);
        System.out.println("Checking if the strings are equal: " + (str1.equals(str2)));
 
	}
}
___________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 5(Ignore Case)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	//String str3 = IgnoreCase(str2);
	
	System.out.println("Checking if the strings are equal and ignoring the cases: " + (str1.equalsIgnoreCase(str2)));
 
	}
}
______________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 6(UPPERCASE AND LOWER CASE)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	String str3 = str1.toUpperCase();
	String str4 = str2.toLowerCase();
	
	
	System.out.println("Converting the strings into upper case: " + str3);
	System.out.println("Converting the strings into lower case: " + str4);
	
 
	}
}

__________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 7(indexOf)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	int ch = str1.indexOf('w');
	
	
	
	System.out.println("index of the given alphabet is " + ch);

	
 
	}
}

_________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 8(lastIndexOf)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	int ch = str1.lastIndexOf('o');
	
	
	
	System.out.println("last index of the given alphabet is " + ch);

	
 
	}
}

__________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 9(startsWith and endsWith)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	
	
	
	
	
	System.out.println("the word starts with " + str1.startsWith("hello"));
	System.out.println("the word starts with " + str2.endsWith("WORLD"));
	

	
 
	}
}
____________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 10(matches)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	
	
	
	
	
	System.out.println("check if the given arrays is matching  " + str1.matches(str2));
	
	

	
 
	}
}

________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 11(substring)

public class Main
{
	public static void main(String[] args) {
	String str1 = "hello world";
	String str2 = "HELLO WORLD";
	
	
	
	
	
	System.out.println("the substring of the given array is:  " + str1.substring(1,4));
	
	

	
 
	}
}

_______________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 12(trim)

public class Main
{
	public static void main(String[] args) {
	String str1 = " hello world ";
	String str2 = "HELLO WORLD";
	String str3 = str1.trim();
	
	
	
	
	System.out.println("trimming the spaces:" + str3);
	
	

	
 
	}
}

__________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 13(valueOf)

public class Main
{
	public static void main(String[] args) {
	String str1 = " hello world ";
	String str2 = "HELLO WORLD";
	//String str3 = str1.trim();
	
	
	
	
	System.out.println("Value of the alphabet:" + str1.valueOf('w'));
	
	

	
 
	}
}

________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 14(Reverse a string):

public class Main
{
	public static void main(String[] args) {
	String str = "hello world";
    //String str2 = "HELLO WORLD";
	//String str3 = str1.trim();
	String reversed = " ";
    for(int i=str.length()-1;i>=0;i--)
    {
        reversed += str.charAt(i);
    }
	
	
	
	System.out.print("reversed string is:" + reversed);
	
	

	
 
	}
}
___________________________________________________________________________________________________________________________________________________________________________________________________


PROGRAM 15(occurance of the Character in the string)

public class Main
{
	public static void main(String[] args) {
	String str = "JasmineDorathy";
    char ch='a';
    int count=0;
    for(int i=0;i<str.length();i++)
    {
        if (str.charAt(i) == ch)
        {
            count++;
        }
    }
	
	
	
	System.out.print("occurance if the Character in the string is:" + count);
	
	

	
 
	}
}

__________________________________________________________________________________________________________________________________________________________________________________________________

PROGRAM 16(Does The string contains the alphabetic characters)

public class Main
{
	public static void main(String[] args) {
	String str = "helloworld89";
  
    if(str.matches("[a-z A-Z]+"))
    {
        System.out.print("The string contains the alphabetic characters");
	
    }
	
	else
	{
	    System.out.print("The string does not contain the alphabetic characters");
	}
	
     }
}
_______________________________________________________________________________________________________________________________________________________________________________________________


PROGRAM 17(Convert character to a string)

public class Main
{
	public static void main(String[] args) {
	char [] charArray ={'J','A','S','M','I','N'};
	String str = new String(charArray);
  
   System.out.println("Conversion of charArray to string: " + str);
   
    }
}

____________________________________________________________________________________________________________________________________________________________________________________________________





















































