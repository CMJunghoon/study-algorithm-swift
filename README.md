# study-algorithm-swift

### Level 1

문제) x만큼 간격이 있는 n개의 숫자  
예)  
0만큼 간격이 있는 3개의 숫자: [0, 0, 0]  
2만큼 간격이 있는 5개의 숫자: [2, 4, 6, 8, 10]   

``` swift
func solution(_ x: Int, _ n: Int) -> [Int] {
    var numbers: [Int] = .init(repeating: 0, count: n)
    for i in 0..<n {
        numbers[i] = x * ( i + 1)
    }
    return numbers
}

solution(0, 3)
solution(2, 5)
solution(67, 100)
```
