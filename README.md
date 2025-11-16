import java.util.*;
class Marks
{
   public static void main(String args[])
   {
   	Scanner sc=new Scanner(System.in);
    int totalmarks=0;
    System.out.println("enter the number of subjects");
    int subject=sc.nextInt();
    System.out.println("number of subject entered:"+subject);
    for(int i=1;i<=subject;i++)
    {
      System.out.println("enter the marks obtain in subject out of 100"+i);
      int marks=sc.nextInt();
      totalmarks+=marks;

    }
    double per=(double)totalmarks/subject;
    char grade;
   	if(per<=100)
   	{
   		grade='A';
   	}
   	 if(per<=80)
   	{
   		grade='B';
   	}
   	 if(per<=50)
   	{
   		grade='C';
   	}
      if(per<50 )
     {
      grade='F';
     }
   System.out.println("******RESULT******");
   System.out.println("totalmarks obtain:"+totalmarks);
   System.out.println("the percentage obtain:"+per+"%");
  

   }
}





