# ad-drama-director

短剧广告导演：一个用于 Claude Code / Codex 的 Agent Skill。

为商品策划剧情化短视频、微短剧带货广告和创意中插：从创意方向走到故事分镜、画风、资产图、逐段视频提示词和视频生成。适用于即梦、Seedance、可灵、MiniMax H3 等视频模型。

## 工作流

| 步骤 | 产出 | 确认点 |
| --- | --- | --- |
| 1 产品简报 | 产品事实、卖点、人群、时长、画幅 | — |
| 2 创意方向 | 3 个差异明显的方向，各带开场钩子 | 用户选定方向 |
| 3 故事与分镜 | 完整故事、卖点对镜表、逐镜分镜 | 用户确认 |
| 4 画风 | 画风方案、可选样张 | 用户确认画风 |
| 5 资产图 | 角色身份板、场景图、产品与道具图 | 用户确认资产 |
| 6 生成方案与提示词 | 生成段、生成方式（多参考/首帧/首尾帧）、逐段提示词 | 用户确认 |
| 7 生成视频 | 视频片段 | 用户批准花费 |

总原则：把错误挡在花钱之前。文字里能发现的错，不留到图上；图上能发现的错，不留到视频上。

## 文件

- `SKILL.md`：主流程与确认规则
- `references/creative-angles.md`：创意玩法、题材、产品删除测试
- `references/story-ideas.md`：可选的剧情原型库
- `references/prompt-rules.md`：剧本、分镜、生成方式与提示词模板
- `references/assets.md`：画风、角色、场景、产品资产图规范

## 安装

Claude Code：

```bash
git clone https://github.com/1ce404/ad-drama-director.git ~/.claude/skills/ad-drama-director
```

Codex：

```bash
git clone https://github.com/1ce404/ad-drama-director.git ~/.codex/skills/ad-drama-director
```

## 使用

在 Claude Code 中输入 `/ad-drama-director`，附上产品、卖点、目标人群和时长。
