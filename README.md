# 社群文案大師

把「每天該發的社群貼文」寫成**像本人寫的**——不是主題式 AI 文案。這是一個 Claude Code Skill，預設情境是台灣的 **Facebook / Threads / Instagram**。

核心不是套模板，是**放大你自己的聲音**：先挖今天的真實素材 → 配一個說話「姿態」（archetype）→ 寫 → 過 3 條死線 QA，確保讀起來像你本人，不是 ChatGPT 生的列點。

## 運作流程

```
① 今天心裡有沒有真的動了什麼？   ← 先找感覺，不是先找主題
② 這個感覺適合哪種「姿態」？      ← 對應 archetype
③ 這個姿態缺哪些原料？            ← 缺什麼問什麼
④ 原料夠了 → 寫
⑤ 過 3 條死線 QA → 像不像本人？
```

- **10 種 archetype（姿態）**：客戶場景診斷、反共識斷言、概念命名、撞牆頓悟、自白脆弱、生活借力… 每種各有需要的「原料」。
- **3 條死線 QA**：真細節夠不夠？節奏有沒有跟同批重複？有沒有 stakes？＋台灣社群版禁詞（寶寶們、內容農場句、罐頭雞湯…）。
- **沒有真素材就不模擬**——你的真實案例、客戶原話才是最強素材，AI 是廚師、你是原料。

## 安裝

```bash
git clone https://github.com/zenbuapps/social-copy-master.git
cp -r social-copy-master/social-copy-master ~/.claude/skills/
```

裝完後在 Claude Code 說「幫我寫今天的社群貼文」「把這個素材寫成一批 Threads」就會觸發。

## 檔案

| 檔案 | 內容 |
|---|---|
| `social-copy-master/SKILL.md` | 主流程：核心原則、思考流程、Stage 1–6、QA、禁詞 |
| `social-copy-master/references/archetypes.md` | 10 種姿態各需要哪些原料 |
| `social-copy-master/references/hooks-endings.md` | 鉤子／中段／結尾零件庫（局部抽換用） |
| `social-copy-master/references/thinkers.md` | 底層思考來源（判斷「好不好」的三個問題） |

## 授權

MIT
