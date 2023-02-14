# 공유 금지
<br/>

**목록**
* [WebUI 다운로드](https://github.com/StableManual/WebUI_Guide)
* [합성 강의 시작](https://github.com/StableManual/synthesis-steps.1)
* [외국 포럼 합성 팁](https://github.com/StableManual/Forum_synthesis_tips)
* [얼싸 강의](https://github.com/StableManual/faceshot)
* 팁


<br/>
<br/>

# WebUI의 설명 

•WebUI는 유저 인터페이스를 만들어 사람들이 보기 편하고 쉽게
  쓰게 만든 버전이다. 스테이블 디퓨전을 쓸려면 어려운 명령어를
  사용하여 실행해야 하나 WebUI는 txt2txt, img2img, inpainting 기능 등
  을 쓰기 편하게 해준다. 우리는 깃허브에 automatic1111이란 
  사람이 올린 버전이나 [아카라이브](https://arca.live/b/aiart/60472214)에
  애옹이도둑님이 올려준 코랩 버전을 쓸거다.

<br/>

WebUI의 장점은 다른 유료 합성 사이트들을 무료로 이용할 수 있다.
또한 더 세세한 설정이 가능하다.(이 때문에 난이도 높음) 그리고
기능이 더 세부적이고 많으며 모델을 추가적으로 이용할 수 있다.

<br/>
<br/>

**오류가 나거나 모르는 점은 텔그 이 링크준 방에서 질문하거나 깃헙 이슈탭
이용해주세요. 정보도 계속 추가합니다**

<br/>
<br/>
<br/>

# WebUI download

> **WebUI 다운을 위한 설명..**

### 코랩(Colab) 버전 WebUI

코랩을 쓰는 이유는 자신의 컴퓨터가 성능이 딸리거나 핸드폰으로
사용하기 위해서다. 자신의 컴퓨터 그래픽카드가 3000번대 이상의
VRAM 6G 이상이고 컴퓨터로 작업하고 싶다면 이 부분은 안봐도 된다.
코랩은 구글에서 운영하기 때문에 컴퓨터 사양을 잡지 않는다.(그림 너무
많이 생성하면 코랩 일시적으로 사용불가.)

**[코랩 버전 다운로드](https://colab.research.google.com/drive/1nBaePtwcW_ds7OQdFebcxB91n_aORQY5)**

* 사본 만들기 꼭 해줘야된다

[Ngrok 터널 사용하기](https://dashboard.ngrok.com/get-started/your-authtoken)
이 사이트 로그인 후 왼쪽 get-started 에 your-authtoken 의 토큰 복사 후
코랩에 NGROK_API_TOKEN 칸에다 붙여넣기 하기 (Ngrok 이 로딩이 더 빠름)

그 후 터널링 서비스를 gradio 에서 ngrok 으로 변경

코랩에서 실행을 눌러 다운로드(***구글 드라이브 여유공간 5G 이상!!***)하고 기다려라.
오류 없이 다운됬다면 초록색의 링크를 타고 들어간다.

![20230129-174828_Chrome](https://user-images.githubusercontent.com/123804566/215316943-43432151-daa3-4e6b-bf9a-0865158e629f.jpg)


이것이 WebUI의 기본 화면이다. 
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

### 모델, VAE 다운(필수)

[합성을 위한 모델](https://huggingface.co/runwayml/stable-diffusion-inpainting/tree/main)
목록에서 sd-v1-5-inpainting.ckpt 을 다운받아
구글 드라이브에 SD > Models > Stable-Diffusion 에 넣는다.

![Untitle11_208182548](https://user-images.githubusercontent.com/123804566/215317239-c52db694-c459-4481-8e37-9b73a07502d4.png)

![Untitle10_202829182415](https://user-images.githubusercontent.com/123804566/215317287-c76089a7-b9c0-48ba-ab9b-0db01fd9585a.png)

그 후 기본 화면에서 왼쪽위에 동그라미 친 부분 클릭 후
sd-v1-5-inpainting선택후 기다리기.
(이상한거 누르면 멈출 수 있음)

<br/>
<br/>

[VAE 다운 사이트](https://huggingface.co/stabilityai/sd-vae-ft-mse)
Evaluation COCO 2017 (256x256, val, 5000 images)에
ft-MSE  840001 다운 후 구글 드라이브에 SD > Models > Vae 에 넣기

그 후 setting의 user interface가면 quick setting list 있음,
거기에 sd_model_checkpoint, sd_vae 입력하고 다시시작하면 상단에 vae 선택할 수 있음
![230129201747](https://user-images.githubusercontent.com/123804566/215322807-c9080826-3209-49a6-93ad-791de62035ac.png)
사진 표시된 곳 눌러서 적용합니다

**이렇게 하면 모든 세팅은 완료 됩니다..**

<br/>
<br/>
<br/>

# 다음강의..
[합성 강의 본편](https://github.com/StableManual/synthesis-steps.1)

<br/>
