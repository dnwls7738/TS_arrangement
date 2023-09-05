# Static Members
클래스에는 static 멤버가 있을 수 있습니다. 이 멤버는 클래스의 특정 인스턴스와 연결되지 않습니다. 클래스 생성자 객체 자체를 통해 액세스할 수 있습니다. static 멤버는 동일한 public, protected 및 private 과 함께 사용할 수도 있습니다.
```
class MyClass {
static x = 0;
static printX() {
console.log(MyClass.x);
}
}
console.log(MyClass.x);
MyClass.printX();
```


Interfaces
객체의 모양을 특정해주기 위해 사용합니다. 여기서는 firstName 및 lastName 필드가 있는 객체를 설명하는 인터페이스를 사용합니다.
```
interface Person {
firstName: string;
lastName: string;
}
```
