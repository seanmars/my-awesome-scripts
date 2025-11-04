# Windows Registry

- Disable automatic folder type discovery:
  - `HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\Shell`
  - String Values > FolderType = NotSpecified

- Disable Bing search in Windows Search:
  - `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Search`
  - DWORD Value > BingSearchEnabled = 0
