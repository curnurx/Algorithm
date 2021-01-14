```
inversion 문제가 가끔 나오는데 나올때마다 머리아파 죽겠다.
정리를 잘하고 가자구...
```

## inversion 정의
```
inversion의 정의는 i < j 인데 arr[i] > arr[j] 인 것.
[inv] 줄여서 inv라 하겠다.
[total-inv] 배열 전체의 inv 수를 total_inv라 하자.
[inner-inv] 부분배열에서 그 부분배열 내 원소들간의 inv 수를 inner-inv라 하자.
[inter-inv] 서로 겹치지 않는 두 부분배열에서 원소를 각각 하나씩 뽑아 계산한 두 구간 간의 inv 수를 inter-inv라 하자.
[inner-swap] 부분배열 내에서 이뤄지는 swap.
[inter-swap] 부분배열 경계를 넘어 이뤄지는 swap.
```


## inversion과 swap의 관계

- After inner-swap, inter-inv is same 
``` 
겹치지 않는 두 구간에서 inner-swap을 아무리해도 inter-inv는 변함이 없다.
```
- 필요한 bubble_sort swap의 갯수 = total_inv
