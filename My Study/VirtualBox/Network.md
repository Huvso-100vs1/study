# 버추얼박스 네트워크 이해 및 구성

## 가상 NIC 종류
[참고 자료](https://www.virtualbox.org/manual/ch06.html)

	1. AMD PCNet PCI II (Am79C970A)
	2. AMD PCNet FAST III (Am79C973), the default setting
	3. Intel PRO/1000 MT Desktop (82540EM)
	4. Intel PRO/1000 T Server (82543GC)
	5. Intel PRO/1000 MT Server (82545EM)
	6. Paravirtualized network adapter (virtio-net)

|NIC 종류                                           |설명  |
|--------------------------------------------------|--|
|AMD PCNet PCI II (Am79C970A)                      |하위 운영체제에서 크게 무리 없이 잡히는 호환성이 가장 좋은 일반적인 NIC이나, 성능이 떨어짐.||
|AMD PCNet FAST III (Am79C973), the default setting|하위 운영체제에서 크게 무리 없이 잡히는 호환성이 가장 좋은 일반적인 NIC. 근래의 최신 OS에서는 더이상 드라이버를 지원하지 않음|
|Intel PRO/1000 MT Desktop (82540EM)               |근래의 시스템에서 가장 기본적으로 제공하는 NIC이며 기가비트를 지원함|
|Intel PRO/1000 T Server (82543GC)                 |XP 같은 시스템에서 별도의 드라이버 없이 사용이 가능한 NIC|
|Intel PRO/1000 MT Server (82545EM)                |Intel PRO/1000 T Server와 동이하나 다른 플랫폼에서 OVF로 가져오기가 용이함|
|Paravirtualized network adapter (virtio-net)      | |









<!--stackedit_data:
eyJoaXN0b3J5IjpbMTUxNTcxMDA0NSwtMTI0NjAxNzQzMV19
-->