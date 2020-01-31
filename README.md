# react-basic
리액트 기초 
<br><br><br>

> <h3>Model vs view</h3>

모델과 뷰는 양방향 바인딩 변화이다. 모델이 변하면 뷰가 변하고, 뷰가 변하면 모델이 변한다. 

이는 유지보수 작업의 비효율을 초래한다. 

이 때 변화(Mutation)하지 않고 데이터가 변하면 view를 날리고 새로 작성한다면?  

but, 브라우저는 DOM기반으로 작성되기 때문에 페이지가 그때그때 바뀐다면 성능이 매우 떨어진다. 




<br><br>



> <h3>React</h3>

: 가상의 DOM에 랜더링 해서 변화가 필효한 곳만 update!  
 유지보수와 확장성이 좋아진다 !
 
 <img width="1442" alt="스크린샷 2020-01-27 오후 12 39 47" src="https://user-images.githubusercontent.com/48245776/73149442-c2143400-4104-11ea-9135-7e7390e6da0b.png">
 
 이해를 돕기위한 영상 : [React and the Virtual Dom](https://www.youtube.com/watch?v=muc2ZF0QIO4)
 
 
 
 <br><br><br>


> WebPack 과 babel

* webpack : 의존성을 분석해 여러개의 모듈을 하나로 묶어주는 역할 
* babel : 다양한 브라우저 환경에 맞춰 최신 코드로 변환해주는 코드 변환기.

 <br><br><br>
 
> JSX란

javascript + XML 이다. 자바스크립트의 확장 문법. 자바스크립트에서 마크업 코드를 작성할 수 있게 된다. 

뿐만 아니라 변수나 프로퍼티 바인딩 기능도 제공한다.

JSX에서 지켜야 할 규칙
1) 모든 태그들은 전부 닫아줘야 한다. 
2) 두 개 이상의 element들은 무조건 하나의 element로 감싸져 있어야 한다. -> v.16에서 도입된 fragment를 사용하면 불필요하게 <div>태그로 감싸줄 필요가 없어진다. 
 
<br><br>

* ***jsx에서 style 적용하기***

기존의 자바스크립트에서는 문자열 형태로 스타일을 적용할 수 있었다.  

```js
<div style="background-color:white; padding:16px; color:green; font-size:16px">안녕하세요!<div>
```

리액트에서는 객체 형태로 적용된다. 각 요소들은 카멜케이스를 사용해야 한다. 

```js
class App extends Component {
  render() {
    const style = {
      backgroundColor : 'black',
      padding: '16px',
      color: 'green',
      fontSize: '3px'
    };
    return <div style = {style}>안녕하세요!</div>;
  };
}
```
