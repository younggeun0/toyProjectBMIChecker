# BMI 지수계산기

* **2018-12-03**
  * Java 학습용 toyProject BMI지수 계산기
  * 키와 몸무게를 입력받아 해당 점수에 해당하는 결과를 출력

![01](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi01.PNG?raw=true) 



---

* **2018-12-10**
  * java AWT를 이용한 GUI 구현(Frame만)
 

![02](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi02.png?raw=true) 

![03](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi03.png?raw=true) 


---

* **2018-12-11**
  * 종료버튼 event처리 구현

---

* **2018-12-13**
  * GUI 디자인(Frame)과 이벤트처리(Listener 인터페이스들) 분리 구현
    * 키, 몸무게 입력 후 계산버튼 클릭시 라벨값 변경, TextArea에 계산결과에 해당하는 결과 
  * 클래스다이어그램과 결과창
  

![05](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi05.png) 

![04](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi04.png)


---

* **2018-12-13**
  * Dialog를 사용한 결과출력 구현
  * 패키지를 run, view, event로 분리했음
    * Dialog 작업을 위한 클래스 추가 생성(BMIResult, BMIResultEvt)
    * 계산버튼 클릭 시 연산작업 후 결과값을 Dialog에게 전달해서 결과 출력


![06](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi06.png)

![07](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi07.png)

---

* **2018-12-14**
  * Swing을 이용하여 구현
    * Dialog로 직접 InputDialog, MessageDialog, ConfirmDialog를 구현할 필요가 없어짐(JOptionPane 이용)
    * 따라서 아래 클래스 다이어그램처럼 구현 내용이 줄어진다
    * AWT에 비해 조금 더 향상된 컴포넌트를 보여준다.


![08-classDiagram](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi08.png)

![09-Swing](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi09.png)


* **2019-12-15**
  * "BMI란?"을 Label이 아닌 TitledBorder로 구현
  * 예외처리
    * 키나 몸무게 TextField에 입력이 안됐을 시 Message Dialog 띄우고 Focus처리
    * 문자열 입력시 MessageDialog로 재입력 유도


![10](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi10.png) 

---

* **2018-12-20**
  * 히스토리 UI 디자인, Swing을 이용한 다이얼로그 구현
  * 입력 내용(키,몸무게)과 실행 날짜, BMI결과값을 HistoryVO로 객체로 저장
    * ArrayList로 결과를 저장 후 BMIHistory에 전달 후 JTable로 결과 표시
    * 현재 history 결과창 출력시 빈 row가 들어가는 이슈있음(보완예정)

![11](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi11.png?raw=true) 

![12](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi12.png) 

![13](https://github.com/younggeun0/younggeun0.github.io/blob/master/_posts/img/toyProjects/bmi13.png) 


### 추가구현 과제
* Swing 구현 내용에서 JButton을 이미지로 구현해보기
* 해당 프로젝트 디렉토리에 history.dat 형태로 history정보를 저장, 프로그램 실행시 읽어서 기록 유지기능 구현
* 메뉴바를 이용 toyProjectLotto와 통합하기

