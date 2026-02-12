

# 自动生成 
  输入如下的提示词：
 检查项目中是否存在 .gitignore、.dockerignore 等忽略文件：                                            
  - 若存在：读取其内容，参考并扩展为 .claudeignore（增加 IDE 目录、虚拟环境、日志、临时文件、敏感配置等）
  - 若不存在：根据项目类型直接生成合适的 .claudeignore


# IDE 相关
/.idea/
.idea
*.iml
*.ipr
*.iws
.vscode
/.lingma/
.eclipse
.settings
.metadata
.recommenders
.project
.classpath
.factorypath

# 构建工具
.gradle
gradle-app.setting
build
out
gen
**/target
*/.flattened-pom.xml
.flattened-pom.xml
**/pom.xml.versionsBackup
rebel.xml

# 操作系统
.DS_Store
Thumbs.db
*.swp
*.swo
*~

# 日志文件
*.log
logs/
log/
*.log.*

# 临时文件
tmp/
temp/
*.tmp
*.temp
*.bak
*.backup
*.old
*.orig
*.cache

# 敏感配置
.env
.env.local
.env.*.local
*.key
*.pem
*.p12
*.pfx
*.jks
*.keystore
secrets/
credentials/

# 测试覆盖率
coverage/
.nyc_output/
*.lcov
.coverage

# Node.js (如果项目包含前端)
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*
.pnpm-debug.log*
dist/
.cache/

# Python (如果项目包含 Python)
__pycache__/
*.py[cod]
*$py.class
.pytest_cache/
.coverage
htmlcov/
*.so
.Python
venv/
env/
ENV/

# Claude 相关
/.claude/
!/.lsp.json

# 其他
*.pid
*.seed
*.pid.lock
