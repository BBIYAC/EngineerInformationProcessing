## 2020년 1회 오답노트
**4. 애플리케이션 테스트의 기본 원리 중 살충제 패러독스(Pesticide Paradox)의 의미를 설명하시오.**

동일한 살충제의 반복 사용시 벌레에게 내성이 생기는 것에 비유하여, 동일한 테스트 전략, 기법을 적용할 시 장애가 도출되지 않음을 의미한다.

```
• 완벽한 테스트 불가능
• 결함 집중: 파레토 법칙(20프로의 코드에서 전체 결함의 80퍼가 발견된다.)
• 오류-부재의 궤변: 결함 모두 제거해도 요구사항을 만족시키지 못한다.
• 테스팅은 정황(Context)에 의존
• 테스트와 위험은 반비례한다.
• 테스트는 점진적으로 확대하며 진행한다.
• 테스트는 별도 팀에서 수행한다.
```
</br>

**5. 데이터 마이닝이란 무엇인지 설명하시오.**

많은 데이터 가운데 숨겨져 있는 유용한 상관관계를 발견하여, 미래에 실행 가능한 정보를 추출해내고 의사 결정에 이용하는 과정

</br>

**6. 프로토콜을 구성하는 대표적인 세가지 요소를 적으시오.**

구문, 의미, 타이핑

</br>

**7. 다음에서 설명하는 해시 함수는?**
```
128비트 암호화 해시 함수로 RFC 1321로 지정되어있으며, 주로 프로그램이나 파일이 원본 그대로인지 확인하는 무결성 검사 등에 사용된다. 1991년에 로널드 라이베스트가 예전에 스이던 MD4를 대체하기 위해 고안하였다.
```
MD5

</br>

**8. 비선점 스케줄링 HRN의 우선순위 계산식을 작성하시오.**

(대기시간+서비스시간)/서비스시간

</br>

**10. 다음에서 설명하는 서비스 거부 공격(DoS, Denial of Service)은?**
```
패킷의 출발지 주소(Address)나 포트(port)를 임의로 변경하여 출발지와 목적지 주소를 동일하게 함으로써, 공격 대상 컴퓨터의 실행 속도를 느리게하거나 동작을 마비시켜 서비스 거부 상태에 빠지도록 하는 공격
```
랜드 어택(Land Attack)

```
• Ping of Death(죽음의 핑)
Ping of Death는 Ping 명령을 전송할 때 패킷의 크기를 인터넷 프로토콜 허용범위 이상으로 전송하여 공격 대상의 네트워크를 마비시키는 서비스 거부 공격 방법이다.

• Smurfing(스머핑)
Smurfing은 IP나 ICMP의 특성을 악용하여 엄청난 양의 데이터를 한 사이트에 집중적으로 보냄으로써 네트워크를 불능 상태로 만드는 공격 방법이다.
각 네트워크 라우터에서 브로드캐스트 주소를 사용할 수 없게 미리 설정해 놓는 것이다.

• SYN Flooding
TCP는 신뢰성 있는 전송을 위해 3-way-handshake를 거친 후에 데이터를 전송하게 되는데, SYN Flooding은 공격자가 가상의 클라이언트로 위장하여 3-way-handshake 과정을 의도적으로 중단시킴으로써 공격 대상자인 서버가 대기 상태에 놓여 정상적인 서비스를 수행하지 못하게 하는 공격 방법이다.

• TearDrop
데이터 송수신 과정에서 패킷의 크기가 커 여러 개로 분할되어 전송될 때 분할 순서를 알 수 있도록 Fragment Offset 값을 함께 전송하는데, TearDrop은 Offset 값을 변경시켜 수신 측에서 패킷을 재조립할 때 오류로 인한 과부화를 발생시킴으로써 시스템이 다운되도록 하는 공격방법이다.

• DDoS(Distributed Denial of Service, 분산 서비스 거부 공격)
DDoS 공격은 여러 곳에 분산된 공격 지점에서 한 곳의 서버에 대한 분산 서비스 공격을 수행하는 것으로, 네트워크에서 취약점이 있는 호스트들을 탐색한 후 이들 호스트들에 분산 서비스 공격용 툴을 설치하여 에이전트로 만든 후 DDoS 공격에 이용한다.
```

</br>

**13. 애플리케이션 성능을 측정하기 위한 요소**
```
(가) - 일정 시간 내에 애플리케이션이 처리하는 일의 양
(나) - 애플리케이션에 요청을 전달한 시간부터 응답이 도착할 때까지 걸린 시간
(다) - 애플리케이션에 작업을 의뢰한 시간부터 처리가 완료될 때까지 거린 시간
자원사용률 - 애플리케이션이 의뢰한 작업을 처리하는 동안의 CPU 사용량, 메모리 사용량, 네트워크 사용량 등
```
처리량, 응답시간, 경과시간

</br>

**15. 데이터베이스 성능 개선과 관련하여 '데이터베이스 반정규화'란 무엇인지 설명하시오.**

시스템의 성능 향상, 개발 및 운영의 편의성 등을 위해 정규화된 데이터 모델을 통합, 중복, 분리하는 과정으로, 의도적으로 정규화 원칙을 위배하는 행위