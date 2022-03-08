# A closer look at Internet structure
- Network edge : host, data centers</br></br>
- Network core : routers
    * circuit switching : 출발지에서 목적지까지 가는 길을 예약 해놓고 특정사용자만 이용하는 방식 (ex. 유선전화망)
    * packet switching : 한 라우터에서 다른 라우터로 들어온 순서대로 내보내는 방식
    * Two key network core function
        - Routing  
            > 받은 패킷을 목적지까지 빠르게 전달하기위해 최적의 경로를 판단
        - Forwarding
            > 포워딩 테이블을 보고 적절한 라우터 출력으로 판단
        - Packet delay : four sources
            > **processing delay** : 비트 에러체크, 출력링크 결정 -> 데이터 처리에 걸리는 시간 </br>
            > **queueing delay** : 전송을 위해 출력링크를 기다리는 시간 -> 큐 안에서 나가기 까지 걸리는 시간 </br>
            > **transmission delay** : 하나의 패킷의 모든 비트를 회선에 올리는 시간 -> 큐에서 링크로 모든 비트를 내보내는데 걸리는 시간, **L/R(패킷의 길이 / 전송속도bps)** </br>
            > **propagation delay** : 출력링크에서 다음 라우터까지 전달하는데 걸리는 시간 -> d/s(라우터간의 거리 / 전파속도) </br>

            d<sub>proc</sub> : 라우터를 업그레이드하면 성능향상가능 / d<sub>trans</sub>  : 전송 대역폭 증설을 통해 성능향상가능
        - Packet loss 
            > 용량이 다 찬 큐에 패킷이 들어오면 버리게 되어 패킷을 잃어버림 </br>
            > 손실된 패킷은 출발지에서 재전송 될수 있음 

</br>

- Access networks, physical media : wire, wireless
