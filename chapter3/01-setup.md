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
    
3. Meteor 설치
    * 7-zip 설치
        * [http://www.7-zip.org](http://www.7-zip.org)
    * chocolatey 설치
        * 참조사이트: [https://chocolatey.org/install](https://chocolatey.org/install) 
        * 관리자권한으로 powershell 실행 후 아래 스크립트 붙여넣기/실행
        ```
        PS> Get-ExecutionPolicy
        PS> Restricted
        PS> Set-ExecutionPolicy AllSigned
        PS> Y
        PS> Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
        PS> choco -?
        PS> exit
        ```
    * meteor 설치
        * 관리자권한으로 powershell 실행
        ```
        PS> choco install meteor -y --excution-timeout 10000
        ```
    * cmder 설치 (git 포함)
        * [http://cmder.net](http://cmder.net)
        * Full 버전 다운로드 (With Git for Windows) 후 압축풀기