# 区块链的第一性原理

**First Principles of Blockchain**

从物质与信息的根本差异出发，逐步推导区块链的技术路线——每一步都是前一步的逻辑必然，而非立场选择。

## 核心论证链

```
物质不可复制 → 信息可复制 → 双花问题不可避免
  → 排序是唯一解 → 排序者不可信 → 去中心化排序
    → 作弊代价必须外部、物理、不可逆 → PoW 是唯一解
      → 单链全局账本 → 链上扩容 → 全球公共基础设施
```

## 文章结构

| 章节 | 主题 |
|------|------|
| 起点 | 物质不可复制 vs 信息可复制 — 双花问题的必然性 |
| 排序 | 全局排序是解决双花的唯一方式 |
| 共识 | PoW 的物理必然性 — 为什么 PoS 不是区块链 |
| 账本 | 不可篡改的公共账本 — 数字世界的"白纸" |
| 扩容 | 不可能三角的谬误 — UTXO 的结构性优势 — 链上扩容 |
| 终局 | 最终只有一条链 — 全球统一账本 |

## 目录结构

```
article/
├── 区块链的第一性原理.md    # 文章源文件 (Markdown)
├── 区块链的第一性原理.pdf    # 排版后的 PDF
├── template.tex              # LaTeX 模板
└── images/                   # 图表
    ├── reasoning-chain.*     # 第一性原理推理链
    ├── mandala-network.*     # 曼荼罗网络拓扑
    └── utxo-vs-account.*    # UTXO vs 账户模型对比
```

## 生成 PDF

需要安装 [Pandoc](https://pandoc.org/) 和 TeX Live：

```bash
cd article
pandoc 区块链的第一性原理.md -o 区块链的第一性原理.pdf \
  --template=template.tex \
  --pdf-engine=xelatex
```

## 作者

佟晓峰 (Alex Tong) — alex@tongxiaofeng.com

## 许可

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
