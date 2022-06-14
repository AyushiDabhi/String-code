import java.util.Scanner;
public class a1
{
    public static void main(String args[])
    {
        String s;
        Scanner input=new Scanner(System.in);
        System.out.println("Enter the statements");
        s=input.nextLine();
        int i,v=0,c=0,d=0,sp=0,spc=0;
        char ch;
        
        for(i=0;i<s.length();i++)
        {
            ch=s.charAt(i);
        
            if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U')
            {
                v++;
            }
            else if(ch>='0' && ch<='9')
            {
                d++;
            }
            else if(ch>='a' && ch<='z'||ch<='A' && ch<='Z')
            {
                c++;
            }
            else if(ch==' ')
            {
                sp++;
            }
            else
            {
                spc++;
            }
        }
    
        System.out.println("The vowel is :"+v);
        System.out.println("The consonant :"+c);
        System.out.println("The digit is :"+d);
        System.out.println("The space is :"+sp);
        System.out.println("This is spacial value :"+spc);
    }
}
