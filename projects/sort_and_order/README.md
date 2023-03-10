# Results

## Int, 66_000
```
|       Method |     N |        Mean |     Error |      StdDev |      Median | Allocated |
|------------- |------ |------------:|----------:|------------:|------------:|----------:|
|  ListOrderBy | 66600 | 12,638.5 us | 233.96 us |   218.85 us | 12,652.9 us | 1066617 B |
|    ListOrder | 66600 | 13,422.0 us | 357.42 us | 1,036.95 us | 12,970.6 us |  800391 B |
|     ListSort | 66600 |    404.9 us |   8.01 us |    22.60 us |    393.7 us |         - |
| ArrayOrderBy | 66600 | 13,439.6 us | 256.00 us |   251.43 us | 13,315.2 us | 1067142 B |
|   ArrayOrder | 66600 | 14,073.9 us | 306.93 us |   900.18 us | 13,759.3 us |  800401 B |
|    ArraySort | 66600 |    414.7 us |   9.18 us |    27.07 us |    402.4 us |         - |
```

## int 

``` ini

BenchmarkDotNet=v0.13.3, OS=ubuntu 22.04
Intel Core i7-8565U CPU 1.80GHz (Whiskey Lake), 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2
  DefaultJob : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2


```
|       Method |     N |          Mean |       Error |      StdDev |        Median | Allocated |
|------------- |------ |--------------:|------------:|------------:|--------------:|----------:|
|  **ListOrderBy** |   **666** |     **76.541 μs** |   **1.4941 μs** |   **2.6168 μs** |     **77.423 μs** |   **10960 B** |
|    ListOrder |   666 |     67.310 μs |   0.6082 μs |   0.5078 μs |     67.286 μs |    8272 B |
|     ListSort |   666 |      3.067 μs |   0.0614 μs |   0.1596 μs |      2.980 μs |         - |
| ArrayOrderBy |   666 |     78.026 μs |   0.6792 μs |   0.6353 μs |     77.974 μs |   10960 B |
|   ArrayOrder |   666 |     67.185 μs |   0.2552 μs |   0.2263 μs |     67.171 μs |    8272 B |
|    ArraySort |   666 |      3.071 μs |   0.0596 μs |   0.1537 μs |      2.989 μs |         - |
|  **ListOrderBy** |  **6660** |    **990.423 μs** |   **9.1000 μs** |   **8.5121 μs** |    **987.813 μs** |  **106865 B** |
|    ListOrder |  6660 |    973.113 μs |   9.1449 μs |   8.1067 μs |    974.218 μs |   80202 B |
|     ListSort |  6660 |     36.839 μs |   0.7245 μs |   1.9954 μs |     37.832 μs |         - |
| ArrayOrderBy |  6660 |    973.938 μs |  19.4040 μs |  19.0573 μs |    975.553 μs |  106865 B |
|   ArrayOrder |  6660 |    932.597 μs |  17.0848 μs |  15.9812 μs |    938.707 μs |   80201 B |
|    ArraySort |  6660 |     38.012 μs |   0.2546 μs |   0.2381 μs |     38.034 μs |         - |
|  **ListOrderBy** | **66600** | **13,514.853 μs** | **264.4200 μs** | **602.2181 μs** | **13,189.411 μs** | **1067432 B** |
|    ListOrder | 66600 | 13,002.016 μs | 205.4561 μs | 192.1837 μs | 13,006.736 μs |  800870 B |
|     ListSort | 66600 |    393.418 μs |   4.0041 μs |   3.7454 μs |    394.131 μs |         - |
| ArrayOrderBy | 66600 | 13,098.111 μs | 216.3621 μs | 202.3852 μs | 13,208.046 μs | 1067357 B |
|   ArrayOrder | 66600 | 13,448.791 μs | 274.0547 μs | 808.0564 μs | 13,033.611 μs |  800331 B |
|    ArraySort | 66600 |    392.654 μs |   2.0020 μs |   1.5631 μs |    393.250 μs |         - |

## string

``` ini

BenchmarkDotNet=v0.13.3, OS=ubuntu 22.04
Intel Core i7-8565U CPU 1.80GHz (Whiskey Lake), 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2
  DefaultJob : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2


```
|       Method |     N |        Mean |       Error |      StdDev |      Median | Allocated |
|------------- |------ |------------:|------------:|------------:|------------:|----------:|
|  **ListOrderBy** |   **666** |    **422.5 μs** |     **4.69 μs** |     **4.16 μs** |    **421.6 μs** |   **18984 B** |
|    ListOrder |   666 |    421.1 μs |     1.89 μs |     1.76 μs |    421.0 μs |   13632 B |
|     ListSort |   666 |    283.9 μs |     1.73 μs |     1.53 μs |    283.9 μs |         - |
| ArrayOrderBy |   666 |    410.4 μs |     8.13 μs |    16.05 μs |    417.0 μs |   18984 B |
|   ArrayOrder |   666 |    386.1 μs |     7.04 μs |    18.16 μs |    381.7 μs |   13632 B |
|    ArraySort |   666 |    272.0 μs |     2.06 μs |     1.61 μs |    272.1 μs |         - |
|  **ListOrderBy** |  **6660** |  **5,621.8 μs** |    **29.98 μs** |    **26.58 μs** |  **5,624.0 μs** |  **186823 B** |
|    ListOrder |  6660 |  5,559.2 μs |    86.72 μs |    72.41 μs |  5,538.8 μs |  133519 B |
|     ListSort |  6660 |  3,925.8 μs |    20.61 μs |    22.91 μs |  3,919.8 μs |       7 B |
| ArrayOrderBy |  6660 |  5,603.8 μs |    22.67 μs |    20.10 μs |  5,609.5 μs |  186823 B |
|   ArrayOrder |  6660 |  5,595.3 μs |    70.98 μs |    66.39 μs |  5,609.0 μs |  133519 B |
|    ArraySort |  6660 |  3,992.5 μs |    29.65 μs |    26.28 μs |  3,996.1 μs |       7 B |
|  **ListOrderBy** | **66600** | **79,120.5 μs** |   **488.45 μs** |   **456.89 μs** | **79,139.2 μs** | **1865270 B** |
|    ListOrder | 66600 | 85,656.3 μs | 1,709.01 μs | 4,192.22 μs | 87,436.6 μs | 1332468 B |
|     ListSort | 66600 | 52,718.8 μs |   481.28 μs |   426.64 μs | 52,743.8 μs |      94 B |
| ArrayOrderBy | 66600 | 78,244.8 μs |   412.48 μs |   365.65 μs | 78,159.6 μs | 1865270 B |
|   ArrayOrder | 66600 | 76,669.2 μs |   658.76 μs |   616.21 μs | 76,582.6 μs | 1332446 B |
|    ArraySort | 66600 | 53,915.7 μs |   422.99 μs |   374.97 μs | 53,865.9 μs |      94 B |

## record (a class)

``` ini

BenchmarkDotNet=v0.13.3, OS=ubuntu 22.04
Intel Core i7-8565U CPU 1.80GHz (Whiskey Lake), 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2
  DefaultJob : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2


```
|       Method |     N |         Mean |       Error |      StdDev |       Median |   Allocated |
|------------- |------ |-------------:|------------:|------------:|-------------:|------------:|
|  **ListOrderBy** |   **666** |     **605.5 μs** |     **2.71 μs** |     **2.26 μs** |     **605.8 μs** |   **165.95 KB** |
|    ListOrder |   666 |     531.4 μs |     3.70 μs |     3.28 μs |     531.3 μs |   160.73 KB |
|     ListSort |   666 |     333.3 μs |     2.33 μs |     2.06 μs |     332.9 μs |   107.91 KB |
| ArrayOrderBy |   666 |     528.1 μs |     2.92 μs |     2.58 μs |     527.6 μs |   165.95 KB |
|   ArrayOrder |   666 |     526.0 μs |     8.79 μs |     7.80 μs |     522.8 μs |   160.73 KB |
|    ArraySort |   666 |     319.9 μs |     2.20 μs |     1.95 μs |     319.3 μs |   107.91 KB |
|  **ListOrderBy** |  **6660** |   **8,691.4 μs** |    **82.29 μs** |    **72.94 μs** |   **8,683.8 μs** |     **2339 KB** |
|    ListOrder |  6660 |   7,826.0 μs |    54.74 μs |    48.53 μs |   7,803.5 μs |  2286.94 KB |
|     ListSort |  6660 |   5,338.8 μs |    37.24 μs |    31.10 μs |   5,343.1 μs |  1549.16 KB |
| ArrayOrderBy |  6660 |   7,657.8 μs |    54.39 μs |    45.42 μs |   7,642.7 μs |  2338.99 KB |
|   ArrayOrder |  6660 |   7,731.7 μs |    45.10 μs |    37.66 μs |   7,715.9 μs |  2286.94 KB |
|    ArraySort |  6660 |   5,275.3 μs |   104.84 μs |   214.16 μs |   5,351.4 μs |  1549.16 KB |
|  **ListOrderBy** | **66600** | **107,898.7 μs** | **1,256.43 μs** | **2,099.21 μs** | **108,257.1 μs** | **30672.69 KB** |
|    ListOrder | 66600 | 109,200.6 μs | 1,422.10 μs | 1,260.66 μs | 109,299.3 μs | 30152.35 KB |
|     ListSort | 66600 |  68,158.8 μs | 1,505.61 μs | 4,439.33 μs |  65,722.0 μs | 20196.58 KB |
| ArrayOrderBy | 66600 | 106,940.8 μs | 2,101.53 μs | 2,805.48 μs | 105,973.8 μs | 30672.69 KB |
|   ArrayOrder | 66600 | 108,683.9 μs | 1,978.03 μs | 2,501.57 μs | 108,512.8 μs | 30152.35 KB |
|    ArraySort | 66600 |  65,542.8 μs | 1,066.73 μs | 1,047.67 μs |  65,901.7 μs | 20196.58 KB |

## record struct

``` ini

BenchmarkDotNet=v0.13.3, OS=ubuntu 22.04
Intel Core i7-8565U CPU 1.80GHz (Whiskey Lake), 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2
  DefaultJob : .NET 7.0.1 (7.0.122.56804), X64 RyuJIT AVX2


```
|       Method |     N |        Mean |       Error |      StdDev |      Median | Allocated |
|------------- |------ |------------:|------------:|------------:|------------:|----------:|
|  **ListOrderBy** |   **666** |    **422.5 μs** |     **4.69 μs** |     **4.16 μs** |    **421.6 μs** |   **18984 B** |
|    ListOrder |   666 |    421.1 μs |     1.89 μs |     1.76 μs |    421.0 μs |   13632 B |
|     ListSort |   666 |    283.9 μs |     1.73 μs |     1.53 μs |    283.9 μs |         - |
| ArrayOrderBy |   666 |    410.4 μs |     8.13 μs |    16.05 μs |    417.0 μs |   18984 B |
|   ArrayOrder |   666 |    386.1 μs |     7.04 μs |    18.16 μs |    381.7 μs |   13632 B |
|    ArraySort |   666 |    272.0 μs |     2.06 μs |     1.61 μs |    272.1 μs |         - |
|  **ListOrderBy** |  **6660** |  **5,621.8 μs** |    **29.98 μs** |    **26.58 μs** |  **5,624.0 μs** |  **186823 B** |
|    ListOrder |  6660 |  5,559.2 μs |    86.72 μs |    72.41 μs |  5,538.8 μs |  133519 B |
|     ListSort |  6660 |  3,925.8 μs |    20.61 μs |    22.91 μs |  3,919.8 μs |       7 B |
| ArrayOrderBy |  6660 |  5,603.8 μs |    22.67 μs |    20.10 μs |  5,609.5 μs |  186823 B |
|   ArrayOrder |  6660 |  5,595.3 μs |    70.98 μs |    66.39 μs |  5,609.0 μs |  133519 B |
|    ArraySort |  6660 |  3,992.5 μs |    29.65 μs |    26.28 μs |  3,996.1 μs |       7 B |
|  **ListOrderBy** | **66600** | **79,120.5 μs** |   **488.45 μs** |   **456.89 μs** | **79,139.2 μs** | **1865270 B** |
|    ListOrder | 66600 | 85,656.3 μs | 1,709.01 μs | 4,192.22 μs | 87,436.6 μs | 1332468 B |
|     ListSort | 66600 | 52,718.8 μs |   481.28 μs |   426.64 μs | 52,743.8 μs |      94 B |
| ArrayOrderBy | 66600 | 78,244.8 μs |   412.48 μs |   365.65 μs | 78,159.6 μs | 1865270 B |
|   ArrayOrder | 66600 | 76,669.2 μs |   658.76 μs |   616.21 μs | 76,582.6 μs | 1332446 B |
|    ArraySort | 66600 | 53,915.7 μs |   422.99 μs |   374.97 μs | 53,865.9 μs |      94 B |
