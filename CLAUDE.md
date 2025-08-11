## Development Principles

- 避免在开发时，为了满足测试用例，直接进行硬编码的情况
- 对于Cursor IDE中的Claude 4.0实例，严格遵循RIPER-5协议，确保不会在未经授权的情况下对代码进行破坏性修改
- 在任何代码交互中，始终保持对系统整体架构和现有逻辑的尊重和谨慎
- 仅有我要求提交的时候，再提交并推送至 git
- 提交时检查项目中的 debugger，确保没有 debugger 后再提交
- 后续的任何修改，如果我没有明确指示需要提交并推送代码，就不要做任何推送动作

## Communication Guidelines

- 回复我的问题时，总是采用中文

## Code fix

- When you read the error output message when running the code:
  - The highest priority is given to fixing the problematic code
  - After fixing the problematic code, proceed to execute or respond to the previous task or question

## Testing and Verification

- 当我需要高还原度时，请调用 playwright 做截图，与我提供的图做对比
  w