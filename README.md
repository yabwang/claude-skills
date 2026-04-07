# Yabwang's Claude Skills

个人使用的 Claude Code Skills 仓库，包含跨项目通用的 AI 工作流。

## 安装

在 Claude Code 中运行：

```
/install-marketplace https://github.com/yabwang/claude-skills
```

或手动添加到 `~/.claude/plugins/known_marketplaces.json`：

```json
{
  "yabwang-skills": "https://github.com/yabwang/claude-skills"
}
```

## 可用 Skills

### blog-updater

自动更新博客 AI 最新进展文章。

- `/yabwang-skills:blog-updater:update-ai-blog` - 更新 AI 博客文章
- `/yabwang-skills:blog-updater:update-latest` - 快速更新命令

## 目录结构

```
claude-skills/
├── .claude-plugin/
│   └── marketplace.json
├── README.md
└── plugins/
    └── blog-updater/
        ├── .claude-plugin/
        │   └── plugin.json
        ├── skills/
        │   └── update-ai-blog/
        │       ├── SKILL.md
        │       ├── scripts/
        │       │   └── fetch-news.py
        │       └── references/
        │           └── template.md
        └── commands/
            └── update-latest.md
```

## 添加新 Skill

1. 在 `plugins/` 下创建新目录
2. 创建 `.claude-plugin/plugin.json`
3. 添加 `skills/` 或 `commands/`
4. 推送到 GitHub

## 许可证

MIT