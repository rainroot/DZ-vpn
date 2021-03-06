# 반가워요. Drizzle VPN입니다.!


안녕하세요. **Drizzle VPN** 개발자 **#rainroot**입니다. **Drizzle VPN**은  **OpenVPN**의 **프로토콜**을 사용하고 **OpenVPN**의 소스 구조와 유사하게 개발하였습니다. 

**Drizzle VPN**은 다음과 같은 특징이 있습니다.

- 멀티스레딩

  > Worker Thread : 암호화 / 복호화 및 라우팅 담당
  >
  > 최소 1개에서 최대 [ CPU core 수 ] * 2

- 리눅스 전용

  > **Drizzle VPN **은 리눅스 전용 프로그램입니다. 윈도우나 기타 OS는 지원하지 않아요.
  >
  > 하지만, **OpenVPN**과 통신이 가능해서 MS윈도우,MAC,안드로이드등의 **OpenVPN** 앱을 그대로 사용할 수 있어요.

* 아직은 미완성

  > 현재 32st 버전은 시험단계에요. 아직은 미완성이죠. 
  >
  > VPN 기능은 안정적으로 동작 하지만,  관리 유틸을 지속적으로 개발 진행 중이에요.
  >
  > **앞으로의 계획**에서 자세히 볼 수 있습니다.



# 성능 비교 [ Drizzle VS OpenVPN ]

- Drizzle VPN [ Bridge Mode ]   ( 단위 : Mbps )

>|          |    74 |    128 |    256 |    512 |   1024 |    1280 |    1420 |    1500 |
>| :------: | ----: | -----: | -----: | -----: | -----: | ------: | ------: | ------: |
>| SEED 128 | 76.56 | 124.23 | 248.14 | 510.04 | 640.72 |  994.54 |  935.01 |   996.8 |
>| ARIA 128 | 64.46 |  89.56 | 248.14 | 525.48 |    896 |  993.33 |  690.92 | 1241.07 |
>| ARIA 192 |  64.6 | 123.37 | 248.14 | 524.96 | 672.12 | 1025.04 |  996.04 | 1164.71 |
>| ARIA 256 | 52.21 | 124.34 | 233.56 | 525.47 |  960.4 |  857.45 | 1118.08 |  996.77 |



- OpenVPN [ Bridge Mode ] ( 단위 : Mpbs )


>|          | 74    | 128   | 256    | 512    | 1024   | 1280   | 1420   | 1500   |
>| :------: | ----: | -----: | -----: | -----: | -----: | ------: | ------: | ------: |
>| SEED 128 | 40.05 | 70.69 | 104.34 | 138.04 | 155.82 | 171.59 | 171.87 | 172.28 |
>| ARIA 128 | 40.1  | 70.65 | 75.84  | 123.07 | 141.02 | 156.78 | 156.49 | 156.94 |
>| ARIA 192 | 40.05 | 57.35 | 75.87  | 122.03 | 140.63 | 155.22 | 141.71 | 155.45 |
>| ARIA 256 | 40.1  | 57.33 | 75.83  | 108.3  | 125.56 | 140.56 | 126.45 | 126.58 |



- Drizzle VPN [ Route Mode ] ( 단위 : Mbps )

>|          | 74    | 128    | 256    | 512    | 1024   | 1280    | 1420    | 1500    |
>| :------: | ----: | -----: | -----: | -----: | -----: | ------: | ------: | ------: |
>| SEED 128 | 40.1  | 97.58  | 186.86 | 465.47 | 732.79 | 994.53  | 782.44  | 996.78  |
>| ARIA 128 | 40.1  | 110.96 | 191    | 359.93 | 747.97 | 1025.01 | 1072.31 | 1012.05 |
>| ARIA 192 | 52.23 | 97.48  | 152.23 | 465.94 | 687.29 | 993.6   | 736.71  | 1073.08 |
>| ARIA 256 | 62.12 | 70.75  | 162.04 | 422.81 | 747.56 | 993.56  | 1057.07 | 1118.9  |



- OpenVPN [ Route Mode ] ( 단위 : Mpbs )


>|          | 74    | 128   | 256   | 512    | 1024   | 1280   | 1420   | 1500   |
>| :------: | ----: | -----: | -----: | -----: | -----: | ------: | ------: | ------: |
>| SEED 128 | 40.01 | 30.68 | 75.95 | 123.24 | 155.81 | 171.92 | 172.03 | 172.11 |
>| ARIA 128 | 27.92 | 57.34 | 61.51 | 122.48 | 140.84 | 126.18 | 156.52 | 156.75 |
>| ARIA 192 | 40.04 | 30.68 | 75.83 | 108.38 | 125.77 | 126.13 | 126.5  | 141.77 |
>| ARIA 256 | 40.08 | 44.06 | 75.92 | 78.8   | 125.36 | 111.09 | 111.25 | 126.53 |





## 내부 멀티스레딩 구조





## 컴파일 방법



## 사용방법



## 설정파일 추가 옵션




# 앞으로의 계획


