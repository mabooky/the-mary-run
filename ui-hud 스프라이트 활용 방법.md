### ui-hud-* 활용 방법

1. ui-hud-container
   위 스프라이트는 9분할 기법을 적용하여 사용해야 하며 적용 방법은 다음과 같다:

   ```css
   .hud { /* 컨테이너로 사용할 CSS 클래스 지정 */
       border-image-source: url('./ui-scoreboard.png');
       border-image-slice: 192 192 192 192 fill;
       border-width: 64px;
       border-style: solid;
       border-color: transparent;
       border-image-repeat: repeat repeat;
   }
   ```

2. ui-hud-egg-slots
   위 스프라이트는 ui-hud-container 내부에 별도의 오버레이로써 적용해야 한다.