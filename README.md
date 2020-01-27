# react-basic
리액트 기초 
<br><br><br>

> <h3>Model과 view</h3>

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
