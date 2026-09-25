# ks-pyqwa · 朋友圈文案生成器 💬

> *Human-sounding WeChat Moments copy in your own voice. Top-3 candidates, each with a harder and a softer cut.*

打开朋友圈，输入框空了十分钟。图是好图，事是好事，就是那句话怎么写都像在念稿。让 AI 写？三秒出来一段，谁都能看出是 AI 写的，比不发还尴尬。

这个 skill 解决的就是那十分钟。

## 🎯 它怎么做

你说一句**核心想法**，给一下**配图或场景**，它从内置的风格方法论库（骨架 A～N + 反检测策略）里匹配最贴切的写法，还你 **3 条候选**：

- 每条附**骨架说明**（为什么这么写）
- 每条附**更狠版**和**更温和版**
- 每条附**一条评论区补刀**（你自己在评论区接的那句）

你挑一条，改两个字，发。

## 💬 你说什么，它给什么

你说：「想发个朋友圈，三张图是周末带娃爬山，核心想法是『大人比小孩更需要出门』，力度中等。」

它还你三条完全不同路数的写法：一条自嘲、一条观察、一条留白，每条都不像 AI，也不像鸡汤。

## 🧬 先做一次个性化（强烈建议）

`knowledge/朋友圈文案方法论.md` 顶部的「账号画像」是一个**虚构示范**。把它改成你自己的真实人设（性别 / 城市 / 职业 / 家庭 / 常发什么），文案才贴你本人。骨架、方法论、反检测策略是通用的，不用动。

进阶：每积累一批自己真发出去的朋友圈，把新写法补进样本和骨架。**它会越用越像你。**

## ⚙️ 安装

```bash
# Claude Code（全局）
git clone https://github.com/KaiSky0823/ks-pyqwa.git ~/.claude/skills/ks-pyqwa
# Codex
git clone https://github.com/KaiSky0823/ks-pyqwa.git ~/.agents/skills/ks-pyqwa
```

目录结构：
```
ks-pyqwa/
├── SKILL.md
├── README.md
└── knowledge/
    └── 朋友圈文案方法论.md
```

装好后直接说「我想发个朋友圈……」，或输入 `/ks-pyqwa`。给上：核心思想（必需）、素材 / 场景、力度（轻松 / 中 / 犀利 / 很冲）、禁区（不想出现的词、要不要 emoji）。

## License

MIT © 2026 KaiSky0823
