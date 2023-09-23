# -Searching-an-Element-in-Array-Binary-Search
 
public class Main {
    public static void main(String args[])
    {
        int a[]={1,2,3,4,5,6,7,8};
        int key=10;
        boolean flag=false;
        int l=0;
        int h=a.length-1;
        while(l<=h)
        {
            int m=(l+h)/2;
            if(a[m]==key)
            {
                System.out.println("The element is found");
                flag=true;
                break;
            }
            if(key>a[m])
            {
                l=m+1;
            }
            if(key<a[m])
            {
                h=m-1;
            }
        }
        if(flag==false)
        {
            System.out.println("The element is not found");
        }
    }
}
