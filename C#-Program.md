
using System;
using System.Linq;
public class HelloWorld
{
    public static void Main(string[] args)
    {
        string arr="4,1,7,3,9,2,6";
        string sortedArray = string.Join(",", arr
        .Split(",")
        .Select(int.Parse)
        .OrderBy(x=>x));

    Console.WriteLine(sortedArray);

    }
}
