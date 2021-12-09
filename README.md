# count-up

진짜 별 것도 아니지만... 디데이 카운터 위젯 마개조<br>
예시: https://phirrblossom.github.io/count-up/count-up.html <br>
소스: https://github.com/phirrblossom/count-up/blob/main/count-up.html <br>
(디데이 스크립트 참조: https://blog.shorouk.dev/notion-widgets-gallery/notion-widget-count-down/ )

# 적용법

1. 받는다
2. 수정한다
  + **문구1**, **문구2**, const myDate = new Date('**May 4, 2021**');
  + 색상변경<br>
  style 에서<br>
   h3{<br>
    color: **#50bcdf**; <br>
    background: transparent; <br>
    }

  <br><br>
  + 색상 대신 이미지 넣기<br>위에 h3 다 지우고<br>
     h3{<br>
    -webkit-text-fill-color: transparent; <br>
    color: transparent;<br>
    background-image: url(https://images.unsplash.com/photo-1550757750-4ce187a65014?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80);<br>
    -webkit-background-clip: text;<br>
    background-clip: text;<br>
    }
  <br>추가
  
  <br><br>
  + 이미지 위아래로 왔다갔다 <br>위에 h3 다 지우고<br>
    h3 {<br>
    background-image: url(**https://images.unsplash.com/photo-1550757750-4ce187a65014?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80) !important;<br>
  animation-duration: **10s**;<br>
  animation-iteration-count: infinite;<br>
  animation-direction: alternate;<br>
  animation-timing-function: linear;<br>
  animation-name: fluid;<br>
  background-size: 600%;<br>
  }<br>

@keyframes bg {
    0% {
        background-position-x: 0;
    }
    100% {
        background-position-x: 10000px;
    }
}
<br>
@keyframes fluid {
    from {
        background-position: top;
    }
    to {
        background-position: bottom;
    }
}
  
  <br>추가
  <br><br>
3.  갠홈 루트폴더나 기트허브나 Apption이나 하여튼 사이트로 변환해주는 곳에 올린다.<br>
4. 주소 따서 html에서 iframe 소스로 원하는 데에 넣기<br>
  <iframe width="120" height="110" src="위젯주소" scrolling="no" frameborder="0"></iframe>
<br>노션은 그냥 링크 임베드하면 됨
