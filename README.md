# Benchmark of Swift extensions compilation times

This benchmark compares compilation time of class with N method vs. time to compile class and N single-method extensions in Swift.

## Usage

```
rake benchmark
```

## Results

On my machine (Macbook Pro 15'' 2017) it produces the following results:

![Benchmark results](results_chart.png?raw=true "Compilation times")

| n | methods | extensions |
| ---: | ---: | ---: |
|100 | 0,55 | 0,3133 |
|1000 | 2,07 | 2,1967 |
|2000 | 4,1533 | 4,46 |
|3000 | 6,2867 | 6,9467 |
|5000 | 10,7267 | 12,71 |
|10000| 23,64 | 38,2133 |
