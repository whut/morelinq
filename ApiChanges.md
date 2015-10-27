# API Changes #

## [v1.0.16006](http://nuget.org/packages/morelinq/1.0.16006) ##

This release contains minor internal implementation changes. There were no changes to the public API.

## [v1.0.15631](http://nuget.org/packages/morelinq/1.0.15631-beta) ##

  * `MoreLinq.MoreEnumerable`
    * `public static TResult Fold(IEnumerable<T> source,Func<T,TResult> folder)`
    * `public static TResult Fold(IEnumerable<T> source,Func<T,T,TResult> folder)`
    * `public static TResult Fold(IEnumerable<T> source,Func<T,T,T,TResult> folder)`
    * `public static TResult Fold(IEnumerable<T> source,Func<T,T,T,T,TResult> folder)`
    * `public static string ToDelimitedString(IEnumerable<string> source)`
    * `public static string ToDelimitedString(IEnumerable<string> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<bool> source)`
    * `public static string ToDelimitedString(IEnumerable<bool> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<sbyte> source)`
    * `public static string ToDelimitedString(IEnumerable<sbyte> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<byte> source)`
    * `public static string ToDelimitedString(IEnumerable<byte> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<char> source)`
    * `public static string ToDelimitedString(IEnumerable<char> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<short> source)`
    * `public static string ToDelimitedString(IEnumerable<short> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<int> source)`
    * `public static string ToDelimitedString(IEnumerable<int> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<long> source)`
    * `public static string ToDelimitedString(IEnumerable<long> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<float> source)`
    * `public static string ToDelimitedString(IEnumerable<float> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<double> source)`
    * `public static string ToDelimitedString(IEnumerable<double> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<decimal> source)`
    * `public static string ToDelimitedString(IEnumerable<decimal> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<ushort> source)`
    * `public static string ToDelimitedString(IEnumerable<ushort> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<uint> source)`
    * `public static string ToDelimitedString(IEnumerable<uint> source,String delimiter)`
    * `public static string ToDelimitedString(IEnumerable<ulong> source)`
    * `public static string ToDelimitedString(IEnumerable<ulong> source,String delimiter)`