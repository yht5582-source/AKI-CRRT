# AKI 與 CRRT 導航

依 **KDIGO 2012 AKI 指引**與 **KDIGO 2026 AKI／AKD 指引公開審閱草案（2026 年 3 月）** 製作的加護病房 AKI 工具：AKI 分期、處置與腎臟保護、腎臟替代治療時機與模式、CRRT 劑量計算、citrate 抗凝監測、RRT 脫離與 AKI 恢復判定。

線上版：https://yht5582-source.github.io/AKI-CRRT/

> ⚠️ **僅供臨床流程輔助與教學，不取代臨床判斷。** KDIGO 2026 為公開審閱草案，正式版可能修改；CRRT 處方與 citrate 監測請依院內流程與腎臟科建議。

## 功能

| 區塊 | 內容 |
|---|---|
| 1. 分期 | 依 SCr（倍數或 48 小時上升 ≥0.3）與 6／12／24 小時尿量自動判定 KDIGO Stage 1–3；2026 草案的 C／U／B 三軸表示（如 C2U1B1）、cystatin C 標準、尿量以理想體重計算、暫時性與持續性 AKI |
| 2. 處置 | 腎毒性藥物管理、平衡晶體液、MAP >65、不用低劑量 dopamine、血糖、找原因；利尿劑與碳酸氫鈉建議；furosemide 壓力測試（1.0 或 1.5 mg/kg，2 小時尿量 <200 mL 預測進展） |
| 3. RRT 時機 | 藥物無效的適應症檢核；延後策略優於預防性提早開始（1C）；血行動力學不穩定用 CRRT 或 PD、腦水腫用 CRRT |
| 4. CRRT 劑量 | 依實際、調整或理想體重（BMI ≥30 自動用調整體重）計算目標 20–25 mL/kg/h；前稀釋校正、扣除停機時間後的實際劑量、過濾分率 |
| 5. 抗凝 | 無禁忌時局部 citrate 優於 heparin（1B）；citrate 禁忌與替代方案、HIT；濾器後與全身 iCa、總鈣／iCa 比值（>2.5 提示 citrate 累積） |
| 6. 脫離與恢復 | 24 小時尿量（無利尿劑 >450、有利尿劑 >2,300 mL）、2 小時肌酸酐清除率 ≥23 mL/min；完全（<1.2 倍）與部分（1.2–1.5 倍）恢復 |

其他功能：
- **床位列**：每床顯示分期。
- **一鍵複製摘要**：可貼到病歷。

## 使用方式

直接用瀏覽器開啟 `index.html` 即可，不需安裝或建置。

## 在地化設定

| 項目 | 位置 |
|---|---|
| 分期邏輯 | `<script>` 內 `stage()` |
| 各區塊內容與 CRRT 計算 | `render()` |
| 床號 | 網頁右側「床號設定」 |

## 資料與隱私

- 所有資料只存在該瀏覽器的 `localStorage`，不會上傳。
- 只記錄床號，請勿輸入姓名或病歷號。

## 依據

1. KDIGO Acute Kidney Injury Work Group. KDIGO clinical practice guideline for acute kidney injury. *Kidney Int Suppl* 2012;2:1–138.
2. KDIGO 2026 Clinical Practice Guideline for Acute Kidney Injury (AKI) and Acute Kidney Disease (AKD). Public Review Draft, March 2026. https://kdigo.org/guidelines/acute-kidney-injury/
3. Chawla LS, et al. Development and standardization of a furosemide stress test to predict the severity of acute kidney injury. *Crit Care* 2013;17:R207.
4. STARRT-AKI Investigators. *N Engl J Med* 2020;383:240–251；Gaudry S, et al. AKIKI. *N Engl J Med* 2016;375:122–133.
5. Zarbock A, et al. RICH trial. *JAMA* 2020;324:1629–1639.

## 授權

請依使用單位規定自行選擇授權方式（例如 MIT）。
