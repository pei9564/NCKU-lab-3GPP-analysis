# NCKU-lab-3GPP-analysis
Python爬蟲－從3GPP歷年會議紀錄分析企業標準化策略




## 一、Work Item分析內容

### （一）自動下載、解壓縮並爬取會議紀錄文件
![WI資料表](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/33c09f6a-254a-4a69-8f60-552d46319f64)
![爬取內容1](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/858268c5-a85b-4e15-aa3a-7db55440bf2c)
![爬取內容2](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/f88e45ea-46e2-4dfa-891c-e058b8839845)
1. 自動下載excel檔中所有zip檔案並
2. 解壓縮，並過濾pdf與excel檔案
3. 使用Excel VBA將doc轉換成docx
4. 爬取所有整理好的docx檔
5. 檢視爬取失敗的檔案

### （二）整理WI資料表
1. 新增WIR所屬企業：從WIR name, WIR email整理
2. 新增下載狀況：該WI是否有連結、以及是否有下載成功
3. 新增專案完成度：以專案是否完成取代專案完成比率
4. 新增TSG分類：分成RAN、SA、CT

### （三）合併WI資料表至SUP資料表、建立company overview
1. 整理爬下來的supporting member表格
2. 統一WI表格中WIR與SUP企業名稱
3. 統一supporting member表格中WIR與SUP企業名稱
4. 合併WI表格到supporting member表格中
5. 整理company overview表格：所有企業在不同版本參與WI次數
6. 拆分成TSG和RAN兩個版本輸出
   
### （四）建立每個release的WIR-supporting member dyads
1. Generate Dyad data (for Ucinet) - supporting member to rapporteur
   
### （五）compute reputation & status
1. 建立Dyad資料－依變數、自變數、控制變數


## 二、Specification分析內容

### （一）2023.03.08 spec analysis
1. 篩選提交至Work plan之specification資料並補上SPR企業
2. 整理表格資料
    * 設定Tech Across Type: 技術跨越型態
    * 整理Primary Resp Grp(C, S, R)至TSG欄位
    * 統一企業名稱
    * 新增Country: SPR企業所屬國家
3. 趨勢圖分析
    * 華為在不同技術時代下之資源策略佈局
    * Top 10 國家參與程度 (retired)
    * 不同技術時代與TSG－企業/國家投入程度
    * 企業/國家投入在跨技術程度
4. 其他分析
    * 各技術時代中，未提交至WP之spec數量
    * 企業投入最多之spec與次數
    * 各spec所更新之總版本數量

### （二）2023.03.08 spec relationship
1. 爬取parent spec和child spec的連結
2. 以企業名稱呈現parent & child之連結
   
![範例](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/d9e7f4bc-b1ab-47fd-9301-c2da85cd6e74)

### （三）2023.04.08 spec history
爬取SPR變更紀錄

![範例](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/bb1b3040-9b3b-4a39-8fce-c21edd47fae8)

