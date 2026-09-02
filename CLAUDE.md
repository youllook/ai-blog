# ai-blog — AI Deep Research Blog

Hugo + PaperMod（theme 已 vendored 進 repo），GitHub Pages。
正式站 https://youllook.github.io/ai-blog/
push 到 `main` 觸發 `.github/workflows/deploy.yml`（CI 用 Hugo 0.146.0 extended）。

## 開發

系統沒裝 Hugo，用 repo 外的可攜版（版本與 CI 一致）：

```bash
D:/claude_workspace/.tools/hugo.exe server --port 1313 --buildDrafts
D:/claude_workspace/.tools/hugo.exe            # 建置到 public/
```

或用 `.claude/launch.json` 的 `ai-blog` 設定。

## 寫文章

```bash
D:/claude_workspace/.tools/hugo.exe new content posts/my-slug.md
```

Frontmatter 照 `archetypes/default.md`。現有文章在 `content/posts/`。

## 這個 blog 的定位

**不寫工具教學，寫「用了 AI 之後才浮出來的問題」。**

現有四篇的路線：
- 〈AI 產出的內容，能代表個人嗎？〉— 使用 ≠ 代表，分界線在能否解釋
- 〈AI：當效率開始定義道德〉
- 〈屁話屠村：當「廢話」成為一種武器〉
- 〈放下之前〉

保持這個調性：有觀點、有論證、不做 SEO 農場文。

## ⚠️ 內容鐵律

**客戶與雇主一律不具名。**
不要出現 JTI／傑太／完美集品／LuggAgent／Dronetag／flyadvisor／彥宣／NEC／恩益禧／勞保局／台電／和潤。
技術心得要抽象化成通用題材再寫。

**flyadvisor.xyz 是雇主網域**，該站內容的作者署名不屬於本人。
但 RID（Remote ID）、圖資等領域知識屬本人專業，發在這裡或官網完全沒問題——
寫的是知識本身，不是雇主的產品或客戶資料。

**憑證與個資**：發布前掃一次。

```bash
grep -rEi 'sk-|ghp_|AKIA|AIza|whsec|lgat_|sbp_|0982[0-9]{6}' content/
```

## 與其他資產的關係

- GitHub profile README 有連到這裡，見 `youllook/youllook`
- 公司官網 https://www.intention.com.tw/ 是另一條通路，走「救援專家」定位（B2B 案源）
- 這裡走個人觀點與思考（個人品牌），兩者互補不重疊
