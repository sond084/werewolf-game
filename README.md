# 10 人狼人殺 Online

單一 HTML，適合部署到 GitHub Pages。

## 功能
- 10 人基本局
- 3 狼人 / 預言家 / 女巫 / 獵人 / 4 平民
- 房主建立 6 碼房號
- 玩家用房號加入
- 真人不足 10 人，房主開始時自動補 AI
- 每位玩家 30 秒發言
- AI 自動產生簡短發言
- 簡易投票介面

## GitHub Pages
1. 建立一個新的 GitHub Repository
2. 上傳 `index.html`
3. Settings → Pages
4. Build and deployment 選 `Deploy from a branch`
5. Branch 選 `main` / `(root)`
6. 儲存，等待 Pages 網址產生

## 連線說明
本版使用 PeerJS 公開 signaling server，GitHub Pages 本身只負責靜態網頁。房主是遊戲連線核心，所以房主關閉分頁後房間會中斷。

若要做到正式產品級房間、斷線重連、永久房間、語音、帳號與戰績，需要改用 Firebase / Supabase / WebSocket 後端。
