# 소플의 처음 만난 리액트 실습 프로젝트 (미니 블로그)

웹 애플리케이션을 개발모드로 실행합니다.
```bash
$ npm start
```

이후 [http://localhost:3000](http://localhost:3000)에서 접속 가능합니다.

---

### 변경사항 업데이트 (2023.07.17)
styled-components 6버전 이상에서 작업하시는 분들은,
CSS에서 사용 된 `& > *`를 `&`로 변경해서 아래와 같이 코드를 작성하시기 바랍니다.

```jsx
// 예시 코드
const Container = styled.div`
    width: 100%;
    max-width: 720px;

    & {
        :not(:last-child) {
            margin-bottom: 16px;
        }
    }
`;
```

참고 링크:
https://styled-components.com/docs/basics#pseudoelements-pseudoselectors-and-nesting
