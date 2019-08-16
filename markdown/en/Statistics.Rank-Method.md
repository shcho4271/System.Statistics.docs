# Statistics.Rank Method

Returns the __ranking of value__ from data array.

```C#
public static int Rank(double value, params double[] a);
public static int Rank(double value, Orderby orderby, params double[] a);
```

## Parameters
* _value_ `Double`  
  A value for which you want to find the rank
* _orderby_ `Orderby`  
  The sorting order of a
* _a_ `Double[]`  
  A real numbers array.

## Returns
`Int32`  
The rank of value about _a_.