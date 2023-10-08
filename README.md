# NCKU-lab-3GPP-analysis
Python爬蟲－從3GPP歷年會議紀錄分析企業標準化策略


## 一、Specification分析內容

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
爬取parent spec和child spec的連結

![範例](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/d9e7f4bc-b1ab-47fd-9301-c2da85cd6e74)

### （三）2023.04.08 spec history
爬取SPR變更紀錄

![範例](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/bb1b3040-9b3b-4a39-8fce-c21edd47fae8)



## 二、Work Item分析內容



## 三、原始資料下載
1. [Work Plan 資料表](https://www.3gpp.org/ftp/Information/WORK_PLAN)
![主資料表](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/65246b47-4837-481b-8adc-c04591d0ead7)
* Work_plan_3gpp_230110.xlsm
  * ID
  * Unique_ID: WI專屬ID
  * Name: WI名稱
  * Acronym
  * OutlineLevel
  * Release: 版本號
  * Resource Names: 所屬TSG
  * Start: 專案開始日期
  * Finish: 專案結束日期
  * %Complete: 專案完成比例
  * **Hyperlink:** 會議資料下載連結 -> WI分析
  * Status Report
  * WI rapporteur name
  * **WI rapporteur e-mail** -> 可爬取WIR所屬企業
  * Notes
  * Impacted TSs and TRs
  * TSG approved
  * PCG approved
  * TSG stopped
  * PCG stopped
  * Created: 建立日期
  * last modif: 最後一次修改日期


2. [Specification 資料表](https://portal.3gpp.org/Specifications.aspx)
![spec主資料表](https://github.com/pei9564/NCKU-lab-3GPP-analysis/assets/103319735/1e02696c-b860-4c6d-ba9d-9e1f4243dd1d)

* 2023-05-19_0651_SpecificationList_3e62b3.xlsx
  * Spec No
  * Type
  * Title
  * Status
  * Primary Resp Grp
  * Primary rapporteur
  * Initial planned Release 
  * Publication
  * Common IMS
  * Technology
