## 추상(abstract) 클래스

추상 클래스는 오직 다른 클래스가 상속받을 수 있는 클래스이다.
하지만 직접 새로운 인스턴스를 만들 수는 없다.
```
abstract class User{
constructor(
private firstname:string,
private lastname:string,
public nickname:string
){
abstract getNickname():void
}
}

class Player extends User{
// 추상 메서드는 추상 클래스를 상속받는 클래스들이 반드시 구현(implement)해야하는 메서드이다.
getNickname(){
console.log(this.nickname)
}
}
```
public: 모든 클래스에서 접근 가능
private: 해당 클래스 내에서만 접근 가능 (자식 클래스에서도 접근 불가)
protected: 해당 클래스와 자식 클래스에서 접근 가능