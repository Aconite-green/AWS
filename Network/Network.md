# Network Study

### Date: 2022년 7월 15일

### Topic: IP and Domain

### Recall

IP, Domain 역할

IP의 단점

사실 도메인은…

나도 도메인을 만들어 볼까?

### Notes

- IP address와 domain name을 이용해서 서버에(혹으 client)에 접근 가능
- 기억하기 어려움 → domain name을 사용함(서로 대칭됨)

- DNS(Domain Name System)을 활용해서 domain 을 입력하면 IP가 대응되도록 설정함

- 도메인은 구입해서 네임서버에 등록해야 함(연간 1~5만원)

<aside>
📌 **SUMMARY: Domain server(IP 알고있음)을 중간에 활용하여 IP = Domain 대응시킴**

</aside>

---

### Date: 2022년 7월 15일

### Topic: IPv6[IP 아끼기 위한 방법]

### Recall

자신의 IP 알기

IP는 총 몇개 일까?

IPv4 와 IPv6(방법 1)

### Notes

- 검색엔진에 “my IP” 검색하기

- 42억개(0.0.0.0 ~ 255.255.255.255)

- 222.109.64.43 / 0000: * 8 → 2^128개까지 표현가능

<aside>
📌 **SUMMARY: 현재는 IPv4와 IPv6를 둘 다 사용중임 (기존의 기기들 때문에 과도기에 해당)**

</aside>

---

### Date: 2022년 7월 15일

### Topic: Port

### Recall

private IP(방법2)

통신사와의 연결 회선

공유기의 IP(공인 IP)

http:// 0000:80

mysql -uroot -p -h[IP] -P3306

### Notes

- 공유기에 연결된 내 컴퓨터의 IP

- 정액제이며 이 금액을 줄이기 위해 공유기를 사용함(연결회선 공유기)
- local로 서버를 만들어도 공유기 IP까지 밖에 도달하지 못하기 때문에 접속이 불가함

- 해당 IP 주소를 가진 컴퓨터에 HTTP 라는 프로토콜을 사용해 접속할 것이고, 80번포트에 설치 되어 있는 소프트웨어 접근할 것이다(일반적으로 웹서버는 80번포트에 설치 되어 있음)

- 3306이 mysql 상에서의 포트번호에 해당 됨

<aside>
📌 **SUMMARY: Port Forwarding 이란** Client 가 공유기의 특정 포트에 접속하면 내 컴퓨터의 포트까지 토스 하는 것을 말함

</aside>

---

### Date: 2022년 7월 15일

### Topic: 절대경로와 상대경로

### Recall

절대경로

상대경로

‘/’ ? 

### Notes

- 나의 위치와 무관하게 표현할 때 사용
- 나의 위치에 따라 바뀔 때 사용

- 최상위 directory를 의미함

```
1)
**absolute path**
"http://localhost/path/same.html"

**relative path**
"./same.html"
"same.html"

2)
**absolute path**
"http://localhost/index.php"
"/index.php"

**relative path**
"../index.php"
```

<aside>
📌 **SUMMARY: 동일한 사이트 내에 파일을 가져올 때 → 상대경로
                    이 사이트가 아닌 바깥에서 파일을 가져올 대 → 절대경로**

</aside>

---

### Date: 2022년 7월 15일

### Topic: Dynamic address

### Recall

dynamic address?

DDNS service

### Notes

- 통신사의 IP는 한정 되어 있기 때문에 기능하고 있지 않은 IP를 회수 다른 곳에 부여함
- dynamic address를 보완하기 위한 방법으로써 특정시간마다 nameserver에게 자신의 IP를 전달함으로써 유동IP 상태라도 도메인 이름을 사용할 수 있게 함

<aside>
📌 **SUMMARY: ipTime에서 DDNS 설정이 가능함**

</aside>

---
