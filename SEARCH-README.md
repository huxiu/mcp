# 虎嗅搜索 MCP

## 什么是虎嗅搜索 MCP 服务？
虎嗅官方搜索 MCP 服务，现提供搜索虎嗅快讯工具。
注: 虎嗅快讯「24小时」是虎嗅出品的短新闻, 用于获取传入实体的最新动态、快速概览、要点提取，为智能体回答注入时效性和独家视角。

## 如何使用虎嗅搜索 MCP 服务 ?
您需要前往虎嗅官网:  [https://www.huxiu.com/member/developer](https://www.huxiu.com/member/developer)

登录后获取 API Key，替换配置文件中的 ${API_KEY}

## 配置示例
### Cline
```json
{
    "mcpServers": {
        "huxiu-mcp": {
            "type": "streamableHttp",
            "url": "https://api-ms-assist.huxiu.com/search/mcp",
            "headers": {
                "Authorization": "Bearer ${API_KEY}"
            }
        }
    }
}
```

### Cherry Studio
```json
{
    "mcpServers": {
        "huxiu-mcp": {
            "type": "streamableHttp",
            "name": "虎嗅MCP",
            "baseUrl": "https://api-ms-assist.huxiu.com/search/mcp",
            "headers": {
                "Content-Type": "application/json",
                "Authorization": "Bearer ${API_KEY}"
            }
        }
    }
}
```

### Trae (内置智能体选择 Builder with MCP)
```json
{
  "mcpServers": {
    "huxiu-mcp": {
      "url": "https://api-ms-assist.huxiu.com/search/mcp",
      "headers": {
        "Authorization": "Bearer ${API_KEY}"
      }
    }
  }
}
```

## 常见问题解答
Q：虎嗅 MCP 服务是否需要付费 ?
A：目前没有费用。
