✅ polymorphism(다형성)
❓poly란?
- many, serveral, much, multi 등과 같은 뜻
❓morphos란?
- form, structure 등과 같은 뜻
❗polymorphos = poly + morphos = 여러 다른 구조

concrete type
- number, boolean, void 등 지금까지 배운 타입

generic type
- 타입의 placeholder

``````
type SuperPrint = { (arr: T[]): void }
type SuperReturn = { (arr: T[]): T }

const superPrint: SuperPrint = (arr) => {
    arr.forEach(i => console.log(i))
}
const superReturn: SuperReturn = (arr) => arr[0]

superPrint([1, 2, false, true])
console.log(superReturn([1, 2, 3, 4]))
``````