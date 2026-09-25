# rust-refactor-local-projects

Refactor a local script/CLI project for efficiency, with Rust as the primary rewrite target for the hot or serving layer. Use when the user wants to speed up a slow local tool, replace a Python/Node server or worker with a single optimized binary, or asks whether a Rust rewrite is worth it. Covers profiling first and choosing Rust versus Go, C/C++, or optimizing the existing language.

## 这是什么

DSH（DeepSeek Harness）skill —— 一个可由 AI agent 按需自动加载的能力单元。克隆到 skill 目录后，DSH 会依据上方描述自动发现并触发它，无需构建。

## 安装

最简单：用 [dsh-config](https://github.com/hpsks416/dsh-config) 的一键脚本 `install.ps1` 批量安装全部 skill。单个安装：

    # GitHub
    git clone https://github.com/hpsks416/rust-refactor-local-projects.git "$env:USERPROFILE\.dsh\skills\rust-refactor-local-projects"
    # 或 Gitee（国内直连更快）
    git clone https://gitee.com/hpsks416/rust-refactor-local-projects.git "$env:USERPROFILE\.dsh\skills\rust-refactor-local-projects"

克隆后 DSH 会自动重新发现，无需重启。更新用：

    git -C "$env:USERPROFILE\.dsh\skills\rust-refactor-local-projects" pull

## 目录结构

    rust-refactor-local-projects/
    ├── SKILL.md    技能入口与工作流
    ├── agents\openai.yaml
    ├── references\decision-guide.md
    ├── references\rust-rewrite.md
    ├── references\worked-example.md

## 依赖

无运行时依赖，纯指令型 skill（由 agent 直接执行 Markdown 工作流）。

## License

MIT License. See [LICENSE](LICENSE).
