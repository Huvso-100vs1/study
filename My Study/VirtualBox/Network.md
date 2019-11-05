# 버추얼박스 네트워크 이해 및 구성

## 가상 NIC 종류
[참고 자료](https://www.virtualbox.org/manual/ch06.html)

### 1. AMD PCNet PCI II (Am79C970A)
 - 게스트 OS의 종류에 상관 없이 호환성이 가장 좋은 일반적인 NIC
 - 성능이 좋지 않음.

### 2. AMD PCNet FAST III (Am79C973), the default setting
 - Default NIC
 - 게스트 OS의 종류에 상관 없이 호환성이 가장 좋은 일반적인 NIC
 - 근래의 최신 OS에서는 더이상 드라이버를 지원하지 않음

### 3. Intel PRO/1000 MT Desktop (82540EM)
 - 윈도우 비스타 이후 버전 호환 NIC
 - 기가비트를 지원함
 - 
### 4. Intel PRO/1000 T Server (82543GC)
 - 추가 드라이브 설치 필요 없이 Windows
### 5. Intel PRO/1000 MT Server (82545EM)

### 6. Paravirtualized network adapter (virtio-net)

|NIC 종류                                           |설명  |
|--------------------------------------------------|--|
|AMD PCNet PCI II (Am79C970A)                      |||
|AMD PCNet FAST III (Am79C973), the default setting||
|Intel PRO/1000 MT Desktop (82540EM)               ||
|Intel PRO/1000 T Server (82543GC)                 |XP 같은 시스템에서 별도의 드라이버 없이 사용이 가능한 NIC|
|Intel PRO/1000 MT Server (82545EM)                |Intel PRO/1000 T Server와 동이하나 다른 플랫폼에서 [OVF](https://ko.wikipedia.org/wiki/%EA%B0%9C%EB%B0%A9%ED%98%95_%EA%B0%80%EC%83%81%ED%99%94_%ED%8F%AC%EB%A7%B7)로 가져오기가 용이함|
|Paravirtualized network adapter (virtio-net)      |반 가상화 네트워크 어댑터|











<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc4ODYxOTAxNSwtMTI0NjAxNzQzMV19
-->