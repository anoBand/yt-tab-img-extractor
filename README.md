# yt-tab-img-extractor

Python 언어 사용

Korean comment supported. 한국어 주석 있음

최근 주요 업데이트 03.19
***
## 추가 예정 기능

#### ~~병합 이미지를 PDF로 변환해 다운~~(완료)

#### ~~실행마다 영상 제목으로 폴더 생성 후 내부에 영상 파일, pdf파일, 이미지 파일 저장~~(완료)

#### ~~악보 이미지 구역 설정 기능 : 가로 a% to b%, 세로 x% to y%~~(완료)

#### fade식으로 전환되는 악보에도 적용 (개별파일 사용 예정)

#### 일정 속도로 움직이는 악보 형식에 대해 추출

#### 다른 악기의 악보 형식에도 적용

#### 웹 UI로 구현해 따로 코드 파일 실행하지 않고도 기능 사용

## 실행 예시

#### 영상 길이, PC성능에 따라 런타임 다를 수 있으나 1~2분정도 걸립니다.
#### 정상 실행 완료 시 "PDF saved successfully as music_file_(번호)\output.pdf" 출력되니 확인하시면 됩니다.
![image](https://github.com/user-attachments/assets/ccbcd56e-1616-43c4-b373-f48b0e5761dc)
![image](https://github.com/user-attachments/assets/897fac09-e3fd-4334-8ced-810092198fd0)


코드 파일 경로에 url 영상파일, 병합된 악보 이미지파일, 병합된 악보 PDF파일 저장됨  
이미지는 Chrome 탭으로 열고 확대해서 보기를 추천합니다.
***
### 설치 프로그램 및 라이브러리:  

**essential installation :**
ffmpeg,
python  
**essential library :**
numpy,
opencv,
yt-dlp
fpdf

### 수정 필요한 변수(v1):  
url,  
tab_region_ratio (필요시)

### 수정 필요한 변수(v2):  
url,  
start_time, end_time (필요시)  
x_start_percent / x_end_percent : 왼쪽부터 가로 몇 %부터 몇 %까지 사용할 것인지를 지정  
y_start_percent / y_end_ percent : **위부터** 세로 몇 %부터 몇 %까지 사용할 것인지를 지정  
***

url변수에 유튜브 링크 넣고 하단 악보 나와있는 영역만큼 비율 변수 설정하면 됩니다!  
라이브러리, 프로그램 설치 방법은 구글링 하시고 질문주세요  
그림판 - 선택 영역 도구 통해 픽셀 측정 가능 -> v2에서 start/end percent 지정에 활용하시면 편합니다.
