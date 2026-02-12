
# 借助AI工具安装CC
 打开 Cursor / Trae ，在聊天框中输入如下提示词：

请自动完成 Claude Code CLI 的环境检测与安装流程，整体逻辑如下：
## 环境与安装状态校验  
- 识别当前操作系统类型（Mac / Linux / Windows）。  
- 执行 `claude --version` 判断 Claude Code 是否已存在。  
  - 若已安装：输出当前版本号，并提示“Claude Code 已就绪，直接运行 claude 即可使用”，随后终止流程。  
  - 若未安装：进入下一阶段。

## Node.js 依赖检查  
- 通过 `node -v` 判断 Node.js 是否已安装。  
- 若未安装，根据操作系统给出对应安装指引：  
  - Mac：`brew install node`，或前往 nodejs.org 下载。  
  - Linux：`sudo apt install nodejs npm`，或前往 nodejs.org 下载。  
  - Windows：推荐使用 `winget install -e --id OpenJS.NodeJS`，或前往 nodejs.org 下载。

## Claude Code 安装  
- 执行统一安装命令：  
  `npm install -g @anthropic-ai/claude-code`  
- 针对不同系统的处理说明：  
  - Windows：在 PowerShell 或 CMD 中直接执行，无需 WSL。  
  - Mac / Linux：若出现 EACCES 权限问题，提醒使用 `sudo` 重新执行。

## 安装结果确认  
- 再次运行 `claude --version` 进行校验。  
- 若验证通过，提示用户可直接输入 `claude` 启动工具，并继续完成 OAuth 登录流程。


