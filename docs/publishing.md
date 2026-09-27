# GitHub 上傳說明

建議倉庫名稱：`ai-to-agent-enterprise-architecture`。
Description、Topics 與版本統一取自根目錄 project.json；About URL 留空，不填未建立網址。

## 上傳前

1. LICENSE、COPYRIGHT.md 已定為保留所有權利（All rights reserved），法律權利人為 AI Coach 益力康陳董；文字與圖卡授權範圍如 COPYRIGHT.md 所列，Logo／人物另列排除項。
2. 確認目標帳號與倉庫可見性。
3. 解壓縮套件；應將內層專案資料夾的內容上傳至 repo 根目錄，不上傳 ZIP 本身作為唯一專案內容。

## 網頁方式

建立指定名稱的空白倉庫，選定可見性；為避免衝突，不另外自動產生 README 或 LICENSE。以 Add file → Upload files 上傳解壓內容並保留資料夾結構。若網頁不支援整個目錄，使用 GitHub Desktop 選擇此資料夾。

每張 PNG 小於 25 MB，可個別上傳。不要把電腦上其他工作目錄或憑證一併拖入。

## 本地 Git 方式

在解壓後的專案根目錄執行 `git init`、`git add .`、`git commit -m "Prepare methodology v1.0.0"`。再從 GitHub 新建倉庫頁面複製真實 remote 指令。不要猜測帳號或 remote URL；已有 repo 時先確認差異，不強制推送。

## 發布驗收

確認 README 顯示封面、docs/cards.md 顯示全部八張圖、相對連結可開啟。

如需建立 Release，以實際提交建立 v1.0.0 tag，採用 RELEASE_NOTES.md 內容。
