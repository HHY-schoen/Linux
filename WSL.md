## 部署 WSL
需要使用管理員權限時，要使用 Powershell。
- 啟用 WSL : Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
- 安裝版本 : wsl --set-default-version 2
- 查看哪些 Linux 發行版適用於安裝的 WSL : wsl --list --online
- 安裝默認發行版 ( Ubuntu ) : wsl --install
  > 若無法安裝，可以自行手動安裝 ( wsl -l -o : 查詢可安裝的 Linux Distro,  wsl --install -d Ubuntu : 選擇安裝 Ubuntu )
- 啟用 Hyper-V
- wsl --l --o : 列出 wsl 可下載的發行版

## WSL 設置與使用
- wsl --help : 查看 wsl 用法
- wsl --status : 查看 wsl 狀態
- wsl -d <發行版> : 運行指定的發行版  ex. wsl -d ubuntu
  > wsl -d <發行版> -u <user> : 可指定 user
- wsl --shutdown : 關閉所有運行中的 wsl
  > wsl --terminate -t <發行版> : 關閉指定的 wsl 發行版


- sudo : 類似 unix 中以 root 身份運行


## Multipass 設置與使用
- bcdedit /set hypervisorlaunchtype off ( auto ) : 禁止 hyper-v 自行啟動
- multipass find : 列出可使用的鏡像
- multipass launch <鏡像> -n <命名> -c 4 -d 5G -m 1G: 部署鏡像、指定分配的cpu核心 / 硬碟容量 / 內存
- multipass list : 列出所有實例
- multipass info --all : 查看所有實例的信息
- multipass delete <實例> : 將指定實例刪除
- multipass purge : 刪除被標記為刪除的實例


-----------------------

refer : https://www.youtube.com/watch?v=kmmHOSHNn3w&list=PLBjZhzRvV2ChjpXW9IU_Ngh6np9gUm3TH&index=9
