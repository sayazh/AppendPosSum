# AppendPosSum
PrintPositiveElementsandSumOfThemattheEnd
import java.util.ArrayList;

public class appendPosSum {
	
		public static void main(String[] args)
		{
			 ArrayList<Integer> list =new ArrayList<Integer>();
			 list.add(-4);
			 list.add(3);
			 list.add(-3);
			 list.add(5);
			 list.add(3);
			 list.add(-2);
			 
			System.out.println(appendPosSum(list));
		}
		//create your method below
		public static ArrayList<Integer> appendPosSum(ArrayList<Integer> numbers){
		  ArrayList<Integer> newList = new ArrayList<Integer>();
		 int sum=0;
		  for(Integer num :numbers){
		    if(num>0){
		      newList.add(num);
		      sum+=num;
		    }  
		  }
		  newList.add(sum);
		  return newList;
		}
	}

