# Achro-em_device-driver_switch
2020 2학기 임베디드시스템 팀 프로젝트, Achro-em FPGA 보드 디바이스 드라이버 분석(딥, 푸쉬 스위치, 버저)
# 팀
2018152010 김지안  
2018152011 김채리(팀장)  
2016156021 이기웅  

## Dip Switch
Dual In-line Package switch  
![dip switch image](https://user-images.githubusercontent.com/59948918/135041790-21c4d8c9-3855-4302-9d4d-85b21dab45ba.png)   
- Dip switch는 DIP 안에 설치한 일련의 토글 스위치로서, 컴퓨터 시스템의 기억용량이나 모니터의 종류 등 여러 가지 정보를 부호화하는 데 사용   
- 컴퓨터와 주변기기를 정상적으로 작동시키기 위해 작동 환경을 설정하는 용도로 많이 쓰임   
- 전자 장치의 동작을 ON/OFF하는데 사용   
![dip switch circuit](https://user-images.githubusercontent.com/59948918/135041983-3a9775ee-f4eb-48a5-8b8d-05ce996457f0.png)   
딥 스위치는 풀업장치로 회로가 구성되어 있어 딥 스위치가 연결되면 LOW(0)값을 가지고, 딥 스위치가 비 연결 상태이면 HIGH(1)값을 가진다.   
![dip switch description1](https://user-images.githubusercontent.com/59948918/135042159-6c78e82b-1981-4223-b6ba-ce5a68ec7260.png)   
![dip switch description2](https://user-images.githubusercontent.com/59948918/135042238-c1b080da-719e-4628-ba49-386e4ebea774.png)   
![dip switch description3](https://user-images.githubusercontent.com/59948918/135042271-46493cae-e01a-4798-8dce-cd701f4306bd.png)   
![dip switch description4](https://user-images.githubusercontent.com/59948918/135042292-f579bafc-dbf1-47ee-840d-d81c11a20058.png)   
## Push Switch   
![push switch image](https://user-images.githubusercontent.com/59948918/135042381-2637e8ff-b7ab-4f94-9069-9c8dafd44e6c.png)
- 외부의 입력을 받아오는 장치, Read 관련 동작만 진행됨   
- 9개의 스위치로 구성됨   
- 자주 값이 변경되거나, 즉시 한번만 사용하는 경우에 이용   
- 입력이 발생하면 값을 버퍼에 담고 device driver가 읽어오는 과정을 수행    
![push switch circuit](https://user-images.githubusercontent.com/59948918/135042494-a1a783f2-5f8d-4175-902a-327dfff20b72.png)    
Push Switch는  누르고 있는 동안 1의 값을 유지하게 되고, 놓으면 0으로 설정하도록 구성되어있다.   
![push switch description1](https://user-images.githubusercontent.com/59948918/135042552-2577e4ac-a401-488d-9ee4-9849b8ed3f1b.png)
   ![push switch description2](https://user-images.githubusercontent.com/59948918/135042564-411b3f9b-c6eb-4023-a755-5c0f35edb3b3.png)
   ![push switch description3](https://user-images.githubusercontent.com/59948918/135042580-aa6da7d4-09c5-4ac0-b3ed-55ebb1dd0f4e.png)   
## Buzzer
![buzzer image](https://user-images.githubusercontent.com/59948918/135042668-87a8d73d-57e8-430b-ba90-f5cce305499a.png)   
- 부저는 피에조 효과를 통해 소리를 출력   
   피에조 효과   
   힘을 가해 변형을 주면 표면에 전압이 발생하고 반대로 전압을 걸면 소자가      
   이동하거나 힘이 발생하는 현상
- 피에조 현상을 일으키는 소자는 움직이면서 주파수 2만Hz 이상의 초음파를 발생시키기 때문에 살균을 위한 초음파 발생에도 사용   
![buzzer circuit](https://user-images.githubusercontent.com/59948918/135042767-769315c3-34ee-48a2-ad84-4412100d2e8c.png)   
부저는 JP1을 연결해야 하는데 연결하면 디바이스 드라이버와 무관하게 항상 소리가 난다.   
![buzzer description1](https://user-images.githubusercontent.com/59948918/135042839-ee47d778-1439-4004-9c06-036777acb1e3.png)   
![buzzer description2](https://user-images.githubusercontent.com/59948918/135042859-031cacc7-89ee-44bf-8f19-b47d190c526f.png)   
![buzzer description3](https://user-images.githubusercontent.com/59948918/135042891-7ed6e51d-25d3-417c-9add-d19c4c59f17f.png)   



