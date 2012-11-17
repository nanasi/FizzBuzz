// FizzBuzz
// ========

// Test Code

class FizzBuzz
{
  public static void main(String[] args)
	{
		int end = Integer.parseInt(args[0]);
		
		for(int i = 0; i <= end; i++)
		{
			bool bThree = i%3 == 0;
			bool bFive = i%5 == 0;
			
			String line;
			if(bThree && bFive)
			{
				line = "fizzbuzz";
			}
			else if(bThree)
			{
				line = "fizz";
			}
			else if(bFive)
			{
				line = "buzz";
			}
			else
			{
				line = String.valueOf(i);
			}
			System.out.println(line);
		}
	}
}
