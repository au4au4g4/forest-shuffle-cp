# 森森不息 CP 攻略

這個 repo 用來整理《森森不息 / Forest Shuffle》的 CP 計算、卡牌快表與套牌攻略。

目前重點是：

```text
快速查表、快速找套牌、避免把所有資料都塞在 README。
```

---

## 快速入口

| 想找什麼 | 檔案 |
|---|---|
| CP 怎麼算 | [`docs/cp-method.md`](docs/cp-method.md) |
| 卡牌 CP 快表 | [`docs/card-cp-reference.md`](docs/card-cp-reference.md) |
| 蒼鷹套完整攻略 | [`decks/goshawk-deck-guide.md`](decks/goshawk-deck-guide.md) |

---

## 目前已確認的重要修正

| 卡牌 | 修正內容 |
|---|---|
| 大斑啄木鳥 | 左下角是「立即抽 1 張」，不是基礎 1 分；若沒有其他玩家森林有更多樹，得 10 分 |
| 灰林鴞 | 立即抽 1 張；固定 5 分；bonus 再抽 2 張 |
| 松鴉 | 完成本回合後，再進行 1 個完整回合 |
| 紅腹灰雀 | 看昆蟲符號，不是鳥數或其他符號 |

---

## CP 計算簡式

```text
總成本 = 費用 + 本身1張 + 回合2張 − 抽牌 − bonus／額外回合收益
CP = 得分 ÷ 總成本
```

詳細算法請看：[`docs/cp-method.md`](docs/cp-method.md)

---

## 推薦查找方式

### 1. 想查單卡強不強

看：[`docs/card-cp-reference.md`](docs/card-cp-reference.md)

適合查：

```text
樹木、上方動物、下方牌、左右牌的單卡 CP
```

### 2. 想查套牌怎麼組

看：[`decks/`](decks/)

目前已有：

| 套牌 | 檔案 |
|---|---|
| 蒼鷹套 | [`decks/goshawk-deck-guide.md`](decks/goshawk-deck-guide.md) |

### 3. 想知道為什麼某組合不列出

看：[`docs/cp-method.md`](docs/cp-method.md) 的「最小達標組合」。

本 repo 會避免列出被更小組合支配的版本，例如：

```text
如果 A + B + 蒼鷹 已經 CP > 2
就不再列 A + B + C + 蒼鷹
```

---

## 目前資料狀態

| 類別 | 狀態 |
|---|---|
| CP 算法 | 已整理 |
| 卡牌快表 | 已整理為獨立檔 |
| 蒼鷹套 | 已修正大斑啄木鳥，並加入最小 CP > 2 組合與雙蒼鷹 |
| 其他套牌 | 待補 |

---

## 待補清單

- 菇類 CP 表
- 鬍鷲 CP 表
- 倉鴞 CP 表
- 全牌 CP 排行榜
- 起手保留牌推薦
- 兩人局／多人局差異
- 其他套牌攻略：兩棲套、鹿套、兔套、蝙蝠套、洞穴套
