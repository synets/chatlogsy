chatlogsy/
├── main.go                # 主程序入口
├── cmd/                   # 命令行相关实现
│   └── chatlog/
│       ├── cmd_key.go         # 获取密钥命令
│       ├── cmd_server.go      # 启动 HTTP 服务命令
│       ├── cmd_version.go     # 版本信息命令
│       ├── log.go             # 日志相关
│       ├── root.go            # 命令行根入口
│       ├── cmd_decrypt.go     # 解密数据库命令
│       └── cmd_dumpmemory.go  # 内存转储相关命令
├── internal/              # 核心功能模块
│   ├── chatlog/               # 聊天记录主逻辑
│   │   ├── app.go                 # 应用主逻辑
│   │   ├── manager.go             # 聊天管理
│   │   ├── http/                  # HTTP 服务
│   │   │   ├── route.go               # 路由与 API
│   │   │   └── service.go             # 服务实现
│   │   ├── mcp/                   # MCP 协议集成
│   │   ├── wechat/                # 微信相关
│   │   ├── database/              # 数据库相关
│   │   ├── conf/                  # 配置
│   │   └── ctx/                   # 上下文
│   ├── wechatdb/              # 微信数据库操作
│   │   ├── wechatdb.go            # 数据库主逻辑
│   │   ├── repository/            # 数据仓库
│   │   └── datasource/            # 数据源
│   ├── wechat/                # 微信协议与数据结构
│   │   ├── wechat.go               # 微信主逻辑
│   │   ├── manager.go              # 微信管理
│   │   ├── process/                # 处理流程
│   │   ├── model/                  # 数据模型
│   │   ├── key/                    # 密钥相关
│   │   └── decrypt/                # 解密相关
│   ├── ui/                     # 终端 UI 相关
│   │   ├── style/                   # 样式
│   │   ├── infobar/                 # 信息栏
│   │   ├── menu/                    # 菜单
│   │   ├── form/                    # 表单
│   │   ├── help/                    # 帮助
│   │   └── footer/                  # 页脚
│   ├── mcp/                    # MCP 协议实现
│   │   ├── stdio.go                 # 标准输入输出
│   │   ├── tool.go                  # 工具相关
│   │   ├── resource.go              # 资源管理
│   │   ├── session.go               # 会话管理
│   │   ├── sse.go                   # SSE 协议
│   │   ├── initialize.go            # 初始化
│   │   ├── jsonrpc.go               # JSON-RPC
│   │   ├── mcp.go                   # MCP 主逻辑
│   │   ├── prompt.go                # Prompt 相关
│   │   └── error.go                 # 错误处理
│   ├── model/                   # 通用数据模型
│   └── errors/                  # 错误定义
├── pkg/                    # 可复用包
│   ├── version/                # 版本信息
│   ├── util/                   # 工具函数
│   ├── filemonitor/            # 文件监控
│   ├── config/                 # 配置管理
│   ├── filecopy/               # 文件复制
│   └── appver/                 # 应用版本
├── script/                 # 脚本
├── docs/                   # 文档
│   ├── mcp.md                  # MCP 集成指南
│   └── prompt.md               # Prompt 示例
├── .github/                # GitHub 配置
├── go.mod                  # Go 依赖管理
├── go.sum                  # Go 依赖校验
├── LICENSE                 # 许可证
├── Makefile                # 构建脚本
├── README.md               # 项目说明
├── DISCLAIMER.md           # 免责声明
├── .gitignore              # Git 忽略文件
└── .goreleaser.yaml        # 发布配置