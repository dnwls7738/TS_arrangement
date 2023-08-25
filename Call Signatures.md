## Call Signatures

프로퍼티로 호출 가능한 것을 설명하려면 객체 타입에 Call Signature을 작성할 수 있습니다.


Call Signatures는 다음과 같이 함수의 매개 변수(parameter)와 반환 타입을 지정합니다.
``````
type Add = {
(a: number, b: number): number;
}
// type Add = (a: number, b: number) => number;

const add: Add = (a, b) => a + b
``````
Call(=Function) Signature란 함수의 매개변수와 반환 값의 타입을 모두 type으로 미리 선언하는 것이다

(React에서 함수로 props를 보낼 때, 어떻게 작동할지 미리 설계 가능!)