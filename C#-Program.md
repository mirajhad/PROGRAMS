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

====================================================

using System;

public class HelloWorld
{
    public static void Main(string[] args)
    {
        int[] a1 ={3,2,1,4,9,1};
        int[] a2 = {9,5,7,1,2,3};
        int[] a3 = new int[a1.Length + a2.Length];
        Array.Copy(a1,0,a3,0, a1.Length);
        Array.Copy(a2,0,a3,a1.Length,a2.Length);
        Array.Sort(a3);
        Console.WriteLine(string.Join(',',a3));
    }
}
