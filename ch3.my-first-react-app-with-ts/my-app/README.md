# 타입 스크립트 적용후 에러 발생(index.tsx)

```
const root = ReactDOM.createRoot(document.getElementById("root"));


Argument of type 'HTMLElement | null' is not assignable to parameter of type 'Element | DocumentFragment'.
  Type 'null' is not assignable to type 'Element | DocumentFragment'.
```

## 해결

```
const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);

또는

const root = ReactDOM.createRoot(document.getElementById('root')!);
```
