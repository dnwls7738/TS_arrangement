# Class Polymorphism

//Storage는 이미 정의되어 있어 여기서 Storage를 선언하면 오버라이딩이 일어나게 될 것이다.

```
interface SStorage{
[key:string]:T
}

class LocalStorage{
private storage:SStorage={}
set(key:string,value:T){
if(this.storage[key]!=undefined)
console.log("Error: already exist!");
else
this.storage[key]=value;
}
remove(key:string){
delete this.storage[key];
}
get(key:string):T{
if(this.storage[key]==undefined)
{
console.log("Error: Dosen't exist!");
// return default;
//자동으로 undefined가 반환되며 에러도 없음.
//받는 쪽에서 undefined인지 검사할 필요가 있음.
}
return this.storage[key];
}

clear(){
this.storage={}
}
}

const stringStorage=new LocalStorage();

console.log(stringStorage.get(""));
stringStorage.set("hello","How are you?");

const booleanStorage=new LocalStorage();
booleanStorage.get("xxx");
booleanStorage.set("ready?",true);
```
