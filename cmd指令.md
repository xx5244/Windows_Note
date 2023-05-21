# cmd指令
---

+ ## 新增資料夾
    ```
    md folder_name
    ```

+ ## 刪除資料夾
    ```
    rd folder_name
    ```

+ ## 刪除檔案
    ```
    del file_name
    ```

+ ## For迴圈
    ```
    FOR /L %i IN (start, step, end) DO (command)
    都可以小寫，當中%i為循環的變數
    ```

+ ## 查看連接過的wifi的ID
    ```
    netsh wlan show profiles
    ```

+ ## 查看連接過的wifi密碼
    ```
    netsh wlan show profile name="ID" key=clear
    ID就是你要找密碼的ID
    ```

+ ## 查看ip位置
    ```
    ipconfig
    ```

+ ## 查看網路更多資訊
    ```
    ipconfig /all
    ```

+ ## 察看外網的ip位置
    ```
    curl -L ip.tool.lu
    是大陸的網站
    ```

+ ## 檢查和修復磁盤驅動器上的錯誤
    ```
    chkdsk
    ```    

+ ## 修復壞道的功能
    ```
    chkdsk /r
    chkdsk /r 命令包含了 chkdsk 的所有功能，並且還具有尋找並修復壞道的功能
    建議用這指令就要事先備份了
    ```

+ ## 測試網路連線
    ```
    ping ip
    ip為ip位置
    ```

+ ## 持續測試網路連線
    ```
    ping ip -t
    ip為ip位置
    Ctrl + C 為退出檢測
    ```

+ ## 遠端控制電腦
    ```
    mstsc
    然後輸入對方的ip與帳密
    注意的點
    1. 開啟遠程桌面功能：您需要在對方計算機上啟用遠程桌面功能，以便能夠使用 mstsc 遠程訪問它。您可以通過控制面板中的系統設置來開啟遠程桌面功能。

    2. 開啟遠程桌面防火牆端口：Windows 防火牆可能會阻止 mstsc 訪問對方計算機，因此您需要確保已經在對方計算機上開啟了遠程桌面端口（預設為 3389 端口），這樣才能允許 mstsc 訪問對方計算機。

    3. 確定用戶名和密碼：您需要知道對方計算機的用戶名和密碼，以便能夠成功登錄和控制對方計算機。    
    ```