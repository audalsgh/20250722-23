# 22~23일차

## 로보플로우에서 라벨링 -> 코랩, 런파드와 연결하여 모델 훈련하기
[교수님의 로보플로우-런파드 연동 자료](https://docs.google.com/document/d/14UZTOXzo2wvKDHm8MRjCrucP1JV6uojaU2NxWFSNO-A/edit?tab=t.0)<br>
[교수님의 로보플로우 자료](https://docs.google.com/document/d/1dX04LQyjvr5-s3gsnk4QqRllBLTgHZzXCGvCRgGFu7s/edit?tab=t.0)

1. 어노테이팅을 300장 이상 완료했다고 가정
<img width="1499" height="913" alt="image" src="https://github.com/user-attachments/assets/697b4e19-9175-4d19-ae3f-5dca045f2633" />

2. 모델 만들기에 들어가서 옵션 건드리지않고 버전 v1 생성
<img width="841" height="914" alt="image" src="https://github.com/user-attachments/assets/193051be-1624-4bcf-824b-ed3b85cd17fd" />

3. 다운로드 데이터셋 누르기
<img width="1461" height="932" alt="image" src="https://github.com/user-attachments/assets/c1e57a73-ca65-459a-b6ef-5b9e03f0d41b" />

4. yoloV8선택 후 show download code
<img width="791" height="409" alt="image" src="https://github.com/user-attachments/assets/5da29c8f-5bcc-4f7b-82e4-9d51e029c4fb" />

5. 코랩으로 넘어가서, api가 가려진 .snippet코드 전체를 가져오면된다.
<img width="795" height="434" alt="image" src="https://github.com/user-attachments/assets/472c1be6-8dac-49c4-bce0-30ced069c97c" />

## 코랩에서 뜨는 오류들
<img width="2560" height="780" alt="image" src="https://github.com/user-attachments/assets/4d22b0a2-270e-4f0a-b106-c51f0b959780" /><br>
현재 data.yaml에서는 상위 디렉토리(즉, ../)의 train, valid, test 폴더를 참조하고 있음.<br>
Colab 내 실제 폴더 구조인 traffic-detection-1/train/images 경로로 맞춰준다.<br>

<img width="2037" height="729" alt="image" src="https://github.com/user-attachments/assets/bb60bc9b-dd8e-41fb-865d-f24c6d341a86" /><br>
이제 오류없이 에포크가 실행된다
