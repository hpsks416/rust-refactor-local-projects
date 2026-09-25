# rust-refactor-local-projects

给慢速/耗资源的本地脚本或 CLI 提速，只重写真正需要加速的那一层，Rust 是热层/服务层的首选目标。

## 适用对象

- DeepSeek Harness（DSH）用户：一个可由 AI agent 按需自动加载的 skill，克隆即用、无需构建。
- 想给慢速脚本/CLI 做 Rust 重写提速的开发者

## 目录结构

    rust-refactor-local-projects/
    ├── SKILL.md    技能入口与工作流
    ├── agents\openai.yaml
    ├── references\decision-guide.md
    ├── references\rust-rewrite.md
    ├── references\worked-example.md

## 安装

    # GitHub
    git clone https://github.com/hpsks416/rust-refactor-local-projects.git "$env:USERPROFILE\.dsh\skills\rust-refactor-local-projects"
    # 或 Gitee（国内直连）
    git clone https://gitee.com/hpsks416/rust-refactor-local-projects.git "$env:USERPROFILE\.dsh\skills\rust-refactor-local-projects"

克隆后 DSH 自动重新发现，无需构建。

## License

MIT License. See [LICENSE](LICENSE).
