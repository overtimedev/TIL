>[stackoverflow map-has-no-len](https://stackoverflow.com/questions/36982858/object-of-type-map-has-no-len-in-python-3)
## Object of type 'map' has no len() in Python 3  
```python
arr = map(int, inout().split())
for i in range(len(arr)):
    if arr[i] % 3 == 0:
      print(arr[i]
```
`배열(arr)에 map()함수로 저장한 후 접근하려하니 오류가 발생`  
len() 함수는 배열의 **요소**의 길이를 구하는 함수이므로 map클래스는 구하지 못한다.  
## list()로 casting  
![스크린샷(27)](https://user-images.githubusercontent.com/80398170/176799130-478213bb-3de9-4d48-bf96-ec5f4cb9eb47.png)  
위와 같이 ***map클래스***로 저장되어 있기에 len()함수는 길이를 재지못한다.  
해결법은 type을 list()로 변경하거나 cnt 변수로 직접 계산하는 방법이 있겠다.
