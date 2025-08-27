# Taiwan Stock AI Analysis

本專案是一套整合技術面、基本面與籌碼面資訊的台股分析系統，
利用 OpenAI GPT 模型每日自動生成選股建議與市場觀察報告。

## 模組結構
- prompts/: 存放每日分析的 Prompt 模板
- data_fetcher/: 擷取或模擬台股數據
- analyzer/: 將資料轉為 Prompt 並呼叫 GPT API
- reports/: 儲存每日分析輸出
- .github/workflows/: 自動排程設定（GitHub Actions）

## 執行流程
1. 擷取每日股市資料
2. 組合 Prompt 並觸發 GPT
3. 產出 Markdown 格式的選股建議報告
4. 自動儲存並可搭配 GitHub Pages 或推播通知
