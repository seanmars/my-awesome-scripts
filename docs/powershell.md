# PowerShell

## 查詢所有 listening 狀態的 port 與執行檔名稱

```powershell
netstat -natb
```

## 更快速找到 listening 狀態的 port 與執行檔名稱

```powershell
Get-NetTCPConnection -State Listen -LocalPort {Port}
```

## Ping host with port

```powershell
Test-Connection www.local.dev -Detail -TcpPort 22
```