>[god_gil님의 티스토리 참고](https://god-gil.tistory.com/10)
## TypeError: _map'_object_is_not_subscriptable  
```python
arr = map(int, input().split())
cnt = 0
for elem in arr:
    if elem % 3 == 0:
        print(arr[cnt - 1])
        break
    cnt += 1
```
코드를 작성하는 도중 subscripable에러 발생 
`배열 arr이 list() type이 아닌데(현 map클래스) map 클래스를 인덱스로 접근하려하여 발생한 에러`
## arr배열을  list()로 casting을 한다. 
```python
arr = list(map(int, input().split()))
cnt = 0
for elem in arr:
    if elem % 3 == 0:
        print(arr[cnt - 1])
        break
    cnt += 1
```
## 티스토리에 나온 예시도 이와 동일하다. 

![스크린샷(28)](https://user-images.githubusercontent.com/80398170/176800528-2957214b-ba8b-4e4e-a9f3-1ed173eda340.png)

