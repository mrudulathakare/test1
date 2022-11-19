import java.util.Date;
import java.text.SimpleDateFormat;
import java.util.TimeZone;
import java.time.*;
import java.time.DayOfWeek;
import java.util.Scanner;

class NotPositiveException extends Exception 
{
    public NotPositiveException(String s)
    {
        // Call constructor of parent Exception
        super(s);
    }
}


public class Mrudula
{
    
	static double comp1(String name,int km,int mth,int dt,String time)
	{
	    
	    LocalDate ld=LocalDate.of(2021,mth,dt);
	    DayOfWeek dow=DayOfWeek.from(ld);
	    Month month=Month.of(mth);
	    
	    double sum;
	    
	    System.out.println("Day of the Week on "+dt+" of the month "+month+" is "+dow.name());
        if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            System.out.println("Your day of travel falls under weekend category");
        }
        else
        {
            System.out.println("Your day of travel falls under weekday category");
        }
            		            
        if((dow.name()=="SATURDAY"||dow.name()=="SUNDAY") && ((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00")))
        {   
            System.out.println("Time falls in peaktime category");
            sum=5.50 + (km*0.75) + 2.50 + 3.00;
        }
        else if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            sum=5.50 + (km*0.75) + 3.00;
        }
        else if((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00"))
        {
            sum=5.50 + (km*0.75) + 2.50;
        }
        else
        {
            sum=5.50 + (km*0.75);
        }
            		                
        System.out.println("Final charges under Company 1: "+sum);
        System.out.println();
        
        ld=null;
        dow=null;
        month=null;
        
        return sum;
	}
	
	static double comp2(String name,int km,int mth,int dt,String time)
	{
	    LocalDate ld=LocalDate.of(2021,mth,dt);
	    DayOfWeek dow=DayOfWeek.from(ld);
	    Month month=Month.of(mth);
	    
	    double sum;
	    
	    System.out.println("Day of the Week on "+dt+" of the month "+month+" is "+dow.name());
        if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            System.out.println("Your day of travel falls under weekend category");
        }
        else
        {
            System.out.println("Your day of travel falls under weekday category");
        }
            		            
        if((dow.name()=="SATURDAY"||dow.name()=="SUNDAY") && ((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00")))
        {
            		               
            System.out.println("Time falls in peaktime category");
            sum=4.50 + (km*0.85) + 2.00 + 2.50;
        }
        else if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            sum=4.50 + (km*0.85) + 2.50;
        }
        else if((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00"))
        {
            sum=4.50 + (km*0.85) + 2.00;
        }
        else
        {
            sum=4.50 + (km*0.85);
        }
            		            
        System.out.println("Final charges under Company 2: "+sum);
        System.out.println(); 
        
        ld=null;
        dow=null;
        month=null;
        
        return sum;
	}
	
	static double comp3(String name,int km,int mth,int dt,String time)
	{
	    LocalDate ld=LocalDate.of(2021,mth,dt);
	    DayOfWeek dow=DayOfWeek.from(ld);
	    Month month=Month.of(mth);
	    
	    double sum;
	    
	    System.out.println("Day of the Week on "+dt+" of the month "+month+" is "+dow.name());
        if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            System.out.println("Your day of travel falls under weekend category");
        }
        else
        {
            System.out.println("Your day of travel falls under weekday category");
        }
            		            
        if((dow.name()=="SATURDAY"||dow.name()=="SUNDAY") && ((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00")))
        {
            System.out.println("Time falls in peaktime category");
            sum=3.50 + (km*0.95) + 1.50 + 2.00;
           
        }
        else if(dow.name()=="SATURDAY"||dow.name()=="SUNDAY")
        {
            sum=3.50 + (km*0.95) + 2.00;
       
        }
        else if((time=="7:00" || time=="8:00" || time=="9:00") || (time=="16:00" || time=="17:00" || time=="18:00"))
        {
            sum=3.50 + (km*0.95) + 1.50;
          
        }
        else
        {
            sum=3.50 + (km*0.95);
           
        }
            		            
        System.out.println("Final charges under Company 3: "+sum);
        System.out.println();
        
        ld=null;
        dow=null;
        month=null;
        
        return sum;
	}
	
	static void result(double chg1,double chg2,double chg3)
	{
	    double max,min;
	    Double[] chgarr = new Double[3];
	    chgarr[0]=chg1;
	    chgarr[1]=chg2;
	    chgarr[2]=chg3;
	    
	    max=chgarr[0];
	    min=chgarr[0];
	    
	  /*  for(int i=0;i<3;i++)
        {
            System.out.println(chgarr[i]);
        }*/
        
        for(int i=0;i<3;i++)
        {
            	if(chgarr[i]>max)
            	{
            		max=chgarr[i];
            	}
            
        }
            		            
        for(int i=0;i<3;i++)
        {
           
            	if(chgarr[i]<min)
            	{
            		min=chgarr[i];
            	}
            
        }
            		            
        if(chgarr[0]==max)
        {
            System.out.println("Most Expensive : Company 1");
        }
        else if(chgarr[0]==min)
        {
            System.out.println("Least Expensive : Company 1");
        }
            		            
        if(chgarr[1]==max)
        {
            System.out.println("Most Expensive : Company 2");
        }
        else if(chgarr[1]==min)
        {
            System.out.println("Least Expensive : Company 2");
        }
            		            
        if(chgarr[2]==max)
        {
            System.out.println("Most Expensive : Company 3");
        }
        else if(chgarr[2]==min)
        {
            System.out.println("Least Expensive : Company 3");
        }
        System.out.println();
        chgarr=null;
	}
	
	static void make_zero(int ch,int mth,int dt,int km,String name,double chg1,double chg2,double chg3)
	{
	    ch = 0;
        mth=0;
        dt=0;
        km=0;
        name = null;
        //time = 0;
        chg1 = 0;
        chg2=0;
        chg3=0;
            		            
        System.out.println("All values reset to zero/null");
        System.out.println("Goodbye");
	}
	
	public static void main(String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		
	    int ch,km=0,mth=0,dt=0;
	    String name="",strtime="",time="";
	    double chg1=0,chg2=0,chg3=0;
	    
		
		
		
		
        System.out.print("1.Enter Usage Details \n");
        System.out.print("2.Display charges under Company 1\n");
        System.out.print("3.Display charges under Company 2\n");
        System.out.print("4.Display charges under Company 3\n");
        System.out.print("5.Show Report\n");
        System.out.print("6.Exit\n");
            

        ch = sc.nextInt();
        if(ch>7)
        {
            System.out.println("Error!! Invalid value , Pls enter valid value");
        }

		while(ch<7)
		{
            		switch(ch)
            		{
            		    case 1: try 
                                {
                                    System.out.println("Enter Name: ");     
                                    name=sc.next();
                                    System.out.println("Enter kilometers travelled: ");
                                    km=sc.nextInt();
                                    System.out.println("Month of Travel: ");
                                    mth=sc.nextInt();
                                    System.out.println("Date of Travel: ");
                                    dt=sc.nextInt();
                                    System.out.println("Time of Travel(24 H Clock): ");
                                    strtime=sc.next();
                                    time=strtime;
                                    // LocalTime lt=LocalTime.parse(strtime);
                		
                                    if(km<0||mth<0||dt<0)
                                    {
                                            throw new NotPositiveException("All numeric values must be +ve");
                                    }
            		        
                                }catch(NotPositiveException e) 
                                {
                                        	System.out.println(e.getMessage());
                                }
        
                                System.out.println();         
            		            break;
            		            
            		    case 2: chg1=comp1(name,km,mth,dt,time);
            		            break;
            		    
            		    case 3: chg2=comp2(name,km,mth,dt,time);
            		            break;     
            		            
            		    case 4: chg3=comp3(name,km,mth,dt,time);
            		            break;
            		            
            		    case 5: result(chg1,chg2,chg3);
            		            break;
            		            
            		    case 6: make_zero(ch,mth,dt,km,name,chg1,chg2,chg3);
            		            System.exit(0);
            		            
            		}
            	System.out.print("1.Enter Usage Details \n");
                System.out.print("2.Display charges under Company 1\n");
                System.out.print("3.Display charges under Company 2\n");
                System.out.print("4.Display charges under Company 3\n");
                System.out.print("5.Show Report\n");
                System.out.print("6.Exit\n");
            

                ch = sc.nextInt();
                if(ch>7)
                {
                    System.out.println("Error!! Invalid value , Pls enter valid value");
                }
		}
	}
	
	
	
}
