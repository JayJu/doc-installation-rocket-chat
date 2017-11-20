# 환경설정

    * 설치환경
        * windows10 64bit Enterprise
        
---

1. Hyper-V 구성요소 설치
    * PowerShell 관리자 권한으로 실행
    * Hyper-V 구성요소 설치
        ```
        Enable-WindowsOptionalFeature -Online -FeatureName:Microsoft-Hyper-V -All
        ```
    * 재부팅
2. Docker for windows 설치
    * 사이트 접속
        * [Install Docker for Windows](https://docs.docker.com/docker-for-windows/install)
    * Stable 버전 다운로드 및 설치
    * 재부팅
    
    