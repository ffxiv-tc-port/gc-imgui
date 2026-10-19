<!-- ffxiv-tc-port 繁體中文說明開始 -->
# Dear ImGui(台服 fork)

Dalamud 介面繪製所用的 Dear ImGui 1.88 加強版（上游 [goatcorp/gc-imgui](https://github.com/goatcorp/gc-imgui) 的 `1.88-enhanced-abifix` 分支，再往上是 [ocornut/imgui](https://github.com/ocornut/imgui)）。由 cimgui 編進 Dalamud 本體的 `cimgui.dll`。

## 台服 fork 的目的

- 讓 cimgui 的子模組網址指向本 org，建置不依賴上游 repo 是否還在、有沒有被改寫。

## 與上游的差異

- 移除上游的 GitHub Actions 工作流程（每日排程建置、每次 push／PR 觸發的建置，以及需要 PVS-Studio／Discord 金鑰的靜態分析）。原始碼與上游相同。
- [gc-cimgui](https://github.com/ffxiv-tc-port/gc-cimgui) 釘的是本分支較早的版本，分支頂端的上游更新（多視窗的透明度支援等）沒有採用。

## 誰在用它

- [gc-cimgui](https://github.com/ffxiv-tc-port/gc-cimgui)：子模組 `imgui`。
- 經由 gc-cimgui 間接使用：[Dalamud](https://github.com/ffxiv-tc-port/Dalamud)（`lib/cimgui/imgui`）。

---

上游原始說明在 [docs/README.md](docs/README.md)，內容未經修改。

<!-- ffxiv-tc-port 繁體中文說明結束 -->
