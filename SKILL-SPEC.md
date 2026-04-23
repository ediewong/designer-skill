# Skill Spec

这个仓库里的每个 skill 都遵循统一的结构约定，方便长期维护、发布和迁移。

## 目录约定

每个已实现 skill 放在某个工作流阶段目录下：

```text
00-meta/<skill-slug>/
02-define/<skill-slug>/
...
```

推荐结构：

```text
<skill-slug>/
├── SKILL.md
├── README.md
├── LICENSE
├── references/
├── assets/
└── evals/
```

其中：

- `SKILL.md`：必须存在，供运行时触发与加载
- `README.md`：人类可读说明，解释适用场景和安装方式
- `LICENSE`：该 skill 的发布许可
- `references/`：方法论资料、框架说明、模式清单
- `assets/`：模板、示意图、输出骨架
- `evals/`：评估题和断言

## Frontmatter 约定

`SKILL.md` 顶部 frontmatter 至少包含：

- `name`
- `description`

建议：

- `name` 与 skill 的发布 slug 保持稳定
- `description` 明确适用场景、触发意图、关键词与边界
- 不要把 README 内容堆进 `description`

## 命名约定

- 目录名使用 kebab-case
- `.skill` 包名与发布 slug 保持一致
- 已发布 slug 尽量不要频繁改动
- 仓库中的阶段路径可以演进，但安装给用户的 skill 名应尽量稳定

## 打包约定

- `.skill` 文件继续放在仓库根目录，方便直接安装
- 打包时归档根目录应当是 skill 自己的 slug，而不是工作流阶段路径
- 例：`00-meta/systems-design-advisor/` 打包后仍然是 `systems-design-advisor.skill`

## 演进约定

- 新能力先写入阶段 README 和 `skill-map.md`
- 当一个能力真正具备 `SKILL.md` 和最小可用资源后，再升级为正式 skill
- 对现有 skill 做大升级时，优先新增 references / assets / evals，而不是频繁改名
