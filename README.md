# Web-Application-IA-Hong

https://github.com/hmoongi94/exam
tag v0.0.1

*11주차 주말시간에 애플리케이션 완성할 예정
*문제점: 모듈화를 시도하면서 함수안에 함수를 넣는 '콜백함수'의 개념을 아직 제대로 몰랐다는 점을 깨달음
-> 콜백함수의 개념을 이해하고 콜백함수를 만들어내는 연습을 할 예정.
-> 그 이후에 json파일에 데이터를 자유롭게 넣고 빼는 연습도 같이 진행할 예정.


*gitbranch 현재까지 진행상황 및 활용방안
- public
    - (static)
        - html,css → gitbranch indexlayout → html레이아웃, css설정
        - js
            
            →git branch JSopentoggle → 메뉴눌렀을 때 메뉴나오는 기능 추가 (addToggleClassOnClick 함수)
            
            →git branch inputdata -> input의 데이터값 fetch를 사용하여 서버로 요청함 req.body값을 데이터로 서버에서 받음
            →git branch jsondata -> 서버에서 json데이터에 옮기는 작업과 json데이터에서 데이터를 뽑아오는 작업을 함.
                                  -> 서버에서 응답해줄 데이터를 정해줌.
            →git branch jsondata  -> fetch에서 await response.data로 서버에서 작업들을 기다렸다가 데이터 응답을 받으면 데이터값을 보여줄 태그들을 생성하고 데이터값을 태그에 넣어서 보여줌.
            
    - (data) 
        - basicData.json ->
        - styleData.json -> script에서 fetch로 post요청했을 때 서버에서 응답한 데이터에 styleData.json 데이터도 넣어줘서
                            질문과 답에 대한 글씨에 스타일 값을 적용.
        - questionData.json -> 사용자가 input에 친 데이터값을 데이터에 저장
        - answerData.json -> 사용자의 질문에 대한 대답을 데이터에 저장
- app.js(server) → git branch server → 서버가동
- route.js -> git branch route -> 서버에서 라우팅부분 모듈화
