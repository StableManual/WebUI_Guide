# WebUI의 설명

•WebUI는 유저 인터페이스를 만들어 사람들이 보기 편하고 쉽게
  쓰게 만든 버전이다. 스테이블 디퓨전을 쓸려면 어려운 명령어를
  사용하여 실행해야 하나 txt2txt, img2img, inpainting 등
  을 쓰기 편하게 해준다. 우리는 깃허브에 automatic111이란 
  사람이 올린 버전이나 [아카라이브](https://arca.live/b/aiart/60472214)에
  애옹이도둑님이 올려준 코랩 버전을 쓸거다.
<br/>
WebUI의 장점은 다른 유료 합성 사이트들을 무료로 이용할 수 있다.
또한 더 세세한 설정이 가능하다.(이 때문이 난이도 높음) 그리고
기능이 더 세부적이고 많으며 모델을 추가적으로 이용할 수 있다.
<br/>
<br/>
**오류가 나거나 모르는 점은 텔그 이 링크준 방에서 질문하거나 깃헙 이슈탭
이용해주세요.**
<br/>
<br/>
---

# WebUI download

> **WebUI 다운을 위한 설명..**

### 코랩(Colab) 버전 WebUI

코랩을 쓰는 이유는 자신의 컴퓨터가 성능이 딸리거나 핸드폰으로
사용하기 위해서다. 자신의 컴퓨터 그래픽카드가 3000번대 이상의
VRAM 6G 이상이고 컴퓨터로 작업하고 싶다면 이 부분은 안봐도 된다.

**[코랩 버전 다운로드](https://colab.research.google.com/drive/1nBaePtwcW_ds7OQdFebcxB91n_aORQY5#scrollTo=UGSqtUJPJoOj)**

실행을 눌러 다운로드(***구글 드라이브 여유공간 5G 이상!!***)하고
오류 없이 다운됬다면 초록색의 링크를 타고 들어간다.

사진

이것이 webUI의 기본 화면이다. 
<br/>
***
### 컴퓨터 버전의 WebUI
<br/>
<br/>
<br/>
후에 추가 예정..
<br/>
<br/>
<br/>
<br/>

***

### 모델 다운(필수)

[합성을 위한 모델](https://huggingface.co/runwayml/stable-diffusion-inpainting/tree/main)
목록에서 sd-v1-5-inpainting.ckpt 을 다운받아
구글 드라이브에 SD > Models > Stable-Diffusion 에 넣는다.

사진

기본 화면에서 왼쪽위에 sd-v1-5-inpainting선택후 기다리기.
(이상한거 누르면 멈출 수 있음)
***

## 합성을 위한 기능(Inpaint)
<br/>

사진

우리는 합성만 할것이니 Img2Img의
Inpaint 기능을 사용할거다.

> Inpaint 기능은 사진에 특정 부분만 AI가 처리하도록 시키는
기능이다. 잘 응용한다면 포토샵처럼 이용가능

사진

사진

<br/>
<br/>

아래 설정들의 개념을 설명하자면 (합성때 주로 쓰는 설정은 굵은글씨)

***

**sampling steps : AI가 얼마나 사진을 검수할지 설정**

**CFG scale : 얼마나 프롬프트를 따를지 설정**

_just resize : 찌부려서 강제맞춤_

**Crop and resize : 남으면 잘라버림**

_Resize and fill : 가장자리만 늘려서 맞춤_

_just resize(Last Noize) : 마지막 생성단계 노이즈 잡아늘림_

_Fill : 원본 무시하고 새롭게 만듬_

**Original : 원본 참고해서 만듬**

**whole picure : 전체영역 생각하고 생성**

_Only masked : 따로 재생성 후 축소해서 박아넣음_

**padding pixels : 마스크 주변에서 몇 픽셀만큼 색,형태, 정보를 반영하는가**

**Denioising strength : 낮을수록 최대한 세밀한 영역만 수정 (원본에 가까움),
   높을수록 많은 부분 자유생성 (원본에서 동떨어짐)**

***

## 합성시작

사진
 
<br/>

자신이 인페인트할 사진을 불러온 후. 자신이 합성할 부분을 
칠해준다.

<br/>

사진

그 후 프롬프트 창에 Nude, Naked, (칠한 부분에 맞는 단어[가슴이면 chest 성기면 뭐뭐 등등 영어로..]) 입력

사진

그럼 실망스럽게 나온다. **포기하지마라 AI는 자신이 어떤 설정, 모델을 쓰고
인내심을 들이냐에 따라 다른 결과가 나온다..**
<br/>
그렇기에 계속 생성해준다.

사진

마음에 드는 사진이 나와도 피부 결계 자국이 나올 수 있는데 
이 경우에는 사진의 버튼을 눌러주어 결과 사진을 다시 인페인트
할 수 있다. 
<br/>
<br/>
<br/>
<br/>
## 팁

Ngrok..
