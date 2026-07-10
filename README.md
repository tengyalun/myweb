# 工作知識庫（GitHub Pages 版）

## 首次發布

1. 在 GitHub 建立一個新的儲存庫（Repository）。若內容不公開，選擇 Private；注意 GitHub Pages 的可用性取決於你的 GitHub 方案。
2. 將這個資料夾內的 `index.html` 和 `data` 資料夾全部上傳到儲存庫根目錄。
3. 在儲存庫的 **Settings → Pages**，選擇 **Deploy from a branch**，分支選 `main`、資料夾選 `/(root)`，然後按 Save。
4. 等待 GitHub 顯示網站網址後，即可開啟使用。

## 日常線上更新

在 GitHub 的儲存庫中開啟 `data/knowledge.json`，按右上角的鉛筆圖示，直接修改並按 **Commit changes**。網站通常會在一兩分鐘內更新。

### 新增每日摘要

在 `workLogs` 陣列內新增一筆：

```json
{"date":"2026-07-11","title":"客戶月報完成","note":"完成資料核對。\n待確認主管簽核。"}
```

### 新增程式碼

在 `snippets` 陣列內新增一筆，`language` 使用 `VBA`、`Power Query M` 或 `Python`。

```json
{"language":"Python","title":"範例名稱","description":"這段程式碼的用途。","code":"print('Hello')"}
```

編輯 JSON 時注意：每一筆資料之間要有逗號，最後一筆後面不能加逗號。
