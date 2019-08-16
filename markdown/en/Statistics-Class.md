# Statistics Class 

Namespace: [System](https://docs.microsoft.com/en-us/dotnet/api/system?view=netframework-4.8)

__Provides static methods for statistical functions.__

```C#
public static class Statistics
```

Inheritance: [Object](https://docs.microsoft.com/en-us/dotnet/api/system.object?view=netframework-4.8) → Statistics

## Example
```C#
using System;
using System.Collections.Generic;

namespace StatisticsCalculator
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Type the data here :");
            string[] input = Console.ReadLine().Split(',');
            List<double> list = new List<double>();
            foreach (string i in input) list.Add(Convert.ToDouble(i.Trim()));
            double[] a = list.ToArray();
            Console.WriteLine("======== CALCULATION RESULT =========");
            Console.WriteLine($"Average             :{Statistics.Average(a)}");
            Console.WriteLine($"Count               :{Statistics.Count(a)}");
            Console.WriteLine($"Geometric mean      :{Statistics.GeometricMean(a)}");
            Console.WriteLine($"Harmonic mean       :{Statistics.HarmonicMean(a)}");
            Console.WriteLine($"Maximum             :{Statistics.Max(a)}");
            Console.WriteLine($"Median              :{Statistics.Median(a)}");
            Console.WriteLine($"Minimum             :{Statistics.Min(a)}");
            Console.WriteLine($"Population stdev    :{Statistics.PStdev(a)}");
            Console.WriteLine($"Population variance :{Statistics.PVariance(a)}");
            Console.WriteLine($"Sample stdev        :{Statistics.Stdev(a)}");
            Console.WriteLine($"Sum                 :{Statistics.Sum(a)}");
            Console.WriteLine($"Sample variance     :{Statistics.Variance(a)}");
        }
    }
}
/*
The example displays output to the following:
Type the data here : 5, 38, 19, 2, 54, 10  <- Input
======== CALCULATION RESULT =========
Average             :21.3333333333333
Count               :6
Geometric mean      :12.545514967211
Harmonic mean       :6.68549087749783
Maximum             :54
Median              :14.5
Minimum             :2
Population stdev    :18.7942071453473
Population variance :353.222222222222
Sample stdev        :20.5880224078629
Sum                 :128
Sample variance     :423.866666666667
*/
```

## Methods

* [Average](Statistics.Average-Method.md)  
  Returns the average of parameters. 
  
* [Count](Statistics.Count-Method.md)  
  Returns the quantity of parameters.
  
* [GeometricMean](Statistics.GeometricMean-Method.md)  
  Returns the geometric mean of parameters.
  
* [HarmonicMean](Statistics.HarmonicMean-Method.md)  
  Returns the harmonic mean of parameters.
  
* [Large](Statistics.Large-Method.md)  
  Returns the k-th largest value from data array.
  
* [Max](Statistics.Max-Method.md)  
  Returns the maximum value of parameters.
  
* [Median](Statistics.Median-Method.md)  
  Returns the median value of parameters.
  
* [Min](Statistics.Min-Method.md)  
  Returns the minimum value of parameters.
  
* [PStdev](Statistics.PStdev-Method.md)  
  Returns the population standard deviation of parameters.
  
* [PVariance](Statistics.PVariance-Method.md)  
  Returns the population variance of parameters.
  
* [Rank](Statistics.Rank-Method.md)  
  Returns the ranking of value from data array.
  
* [Small](Statistics.Small-Method.md)   
  Returns the k-th smallest value from data array.
  
* [Stdev](Statistics.Stdev-Method.md)  
  Returns the sample standard deviation of parameters.
  
* [Sum](Statistics.Sum-Method.md)  
  Returns the sum of parameters.
  
* [Variance](Statistics.Variance-Method.md)  
  Returns the sample variance of parameters.

## See also
* [Orderby enum](Orderby-enum)
