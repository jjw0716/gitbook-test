# Server

### 개요

CPU, 메모리 등의 리소스를 할당 받아 Application을 동작할 수 있는 가상머신(VM)을 의미합니다.\
네트워크 기능을 통해 다른 VM 또는 외부와 통신할 수 있습니다.

### Server Action Flow

<figure><img src="../../.gitbook/assets/server-action-flow.png" alt=""><figcaption></figcaption></figure>

### Server Status

| Server Status | Server Action                                                           | 비고      |
| ------------- | ----------------------------------------------------------------------- | ------- |
| BUILD         | <p>DELETE<br>FORDE_DELETE</p>                                           | 진행중인 상태 |
| ERROR         | <p>DELETE<br>FORCE_DELETE</p>                                           | 진행중인 상태 |
| ACTIVE        | <p>REBOOT<br>HARD_REBOOT<br>STOP<br>PAUSE<br>DELETE<br>FORCE_DELETE</p> |         |
| SHUTOFF       | <p>START<br>HARD_REBOOT<br>DELETE<br>FORCE_DELETE</p>                   |         |
