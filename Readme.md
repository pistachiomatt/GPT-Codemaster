# GPT-Codemaster

自动通过从问题中创建拉取请求来进行编程。

这是一个实验性项目，旨在自动化编程。它采用基于任务的方法，通过从 Github 问题中读取任务描述并在拉取请求中实现它们来推动软件项目的开发。

使用此工具创建的示例拉取请求可在[此处](https://github.com/dex3r/GPT-Codemaster/pulls?q=is%3Apr+label%3A%22GPT-Codemaster+example%22+)找到。

## 功能
 - [x] 修改文件
 - [x] 创建新文件
 - [x] 自动对指定标签的问题作出反应
 - [x] 创建拉取请求
 - [ ] 作为 Github Action 发布到市场
 - [ ] 为其实现自动创建测试
 - [ ] 对拉取请求检查作出反应
 - [ ] 在拉取请求中来回对话并对人类反馈作出反应
 - [ ] 实现反射（https://arxiv.org/pdf/2303.11366.pdf 和 https://nanothoughts.substack.com/p/reflecting-on-reflexion）
 - [ ] 能够处理大型项目
 - [ ] 读取每个项目的 .ai/project_description_short.json 并将其包含在提示中
 - [ ] 轻松连接不同的 LLM，包括本地托管的

## 测试
 - [x] 完成一个简单的问题，[示例](https://github.com/dex3r/GPT-Codemaster/pull/2)
 - [ ] 完成一个更复杂的问题

## 常见问题解答

### 它有效吗？
有时候，只适用于具有小文件的小项目，如此项目。目前最大的限制是 LLM 的令牌长度。

### 它真的有效吗？
这是一个实验，而不是实际产品。

### 我需要什么才能使用它？
1. GPT-4 API 访问和令牌
1. Github 仓库
1. 将此项目作为 GitHub Action
1. 在设置中启用“允许 Github Actions 创建拉取请求”
