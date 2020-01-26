# active-directory-overview

## Active Directory 
Windows Server 2000에서 기존의 NTLM(Windows NT LAN Manager)를 대신하여 도메인 기반의 사용자/호스트 인증 방식으로 Kerberos v5(RFC1510)을 채용함. 
(NTLM은 도메인 Join되지 않은 standalone 시스템에서 계속 사용됨) (https://medium.com/@robert.broeckelmann/kerberos-and-windows-security-history-252ccb510137)

Active Directory에서 Kerberos 동작 방식은 아래 참조
https://ammarhasayen.wordpress.com/2011/02/05/kerberos-in-ad-101/

Ref) 
https://medium.com/@robert.broeckelmann/kerberos-and-windows-security-kerberos-on-windows-3bc021bc9630

## [gMSA(group Managed Service Account)](https://docs.microsoft.com/en-us/windows-server/security/group-managed-service-accounts/group-managed-service-accounts-overview)
- sMSA(standalone Managed Service Account)는 managed domain account로 Windows Server 2008R2 및 Windows 7에서 지원되기 시작하여 암호 자동 관리 기능 및 
- 간편한 SPN 관리 기능 및 타 관리자들에 management를 delegation할 수 있는 기능을 제공.
- gMSA는 sMSA와 같은 기능을 제공하며 해당 기능을 복수의 서버에 걸쳐 확장할 수 있는 기능을 제공. 서버팜, 또는 로드발란서 뒤의 백엔드 서버들에서 구동되는 서비스에 단일 identity 솔루션 제공
- gMSA가 service principal로 사용될 경우 관리자가 암호를 관리하지 않고 Windows OS가 해당 account의 암호를 관리. 
- member 호스트들은 도메인 컨트롤러로 부터 최신 암호를 얻음




