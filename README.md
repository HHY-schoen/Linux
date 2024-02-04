## linux-command

### Navigation
- pwd : 目前位置
- explore.exe <路徑> : 打開某個資料夾
- open / : 打開根目錄
- ls : 列出目前所在資料夾中的檔案
  > ls -a : 顯示包括隱藏檔案的所有檔案 ( 隱藏檔案開頭為 . )
  > ls -l : 列出資料夾中檔案的詳細資訊
  > ls -la : 顯示所有檔案 ( 含隱藏檔案 ) 的詳細資訊
  > ls <路徑> : 查看指定路徑下的所有檔案

- man <指令> : 查詢該指令用法 ( press "q" to quit )

- cd <路徑> : 進入指定路徑
- cd .. : 回到上一層


### 檔案操作
- mkdir <資料夾名稱> : 建立資料夾
- cat <檔案名稱> : 印出檔案內容
- cp <來源> <目的> : 複製檔案
- cp -r <來源> <目的> : 複製資料夾  ( recursive )
- rm <檔案> : 刪除檔案
- rm -r <檔案> : 刪除資料夾
- rm -rf <檔案> : "強制"刪除資料夾
- mv <原路徑> <新路徑> : 移動檔案 ( 剪貼 )   ( move )
- mv <原檔名> <新檔名> : 重新命名

**按 " 上 or 下 " 可選擇之前打過的指令，不用重新輸入**
**ctrl + R : 搜尋用過的指令 ( crtl + S : 往後搜尋)**


### vim
vim 是一個文字編輯器。
- vim <檔名> : 打開檔案 ( 若檔名不存在則創建 )


### Package-manager
package-manager 就是拿來安裝東西的工具。
> 每種系統對應的按裝指令不太一樣 ( mac: brew install, ubuntu: apt inatall, manjaro: pacman -S )


