# 虎嗅 MCP

## 什么是虎嗅 MCP 服务 ?
虎嗅官方 MCP 服务，现提供「虎嗅视界」原创视频内容集。包含: 美食类、科普故事类、前沿科技类、商业消费类、泛财经类、汽车类、3C数码类、时尚生活类、旅游类、健康医疗类、人物对话类等。各栏目下视频内容实时同步更新。

后续将提供图文资讯类、效率工具类服务，敬请关注。

## 如何使用虎嗅 MCP 服务 ?
您需要前往虎嗅官网:  [https://www.huxiu.com/member/developer](https://www.huxiu.com/member/developer)

登录后获取 API Key，替换配置文件中的 ${API_KEY}

## 配置示例
### Cherry Studio
```json
{
    "mcpServers": {
        "huxiu-mcp": {
            "type": "streamableHttp",
            "name": "虎嗅MCP",
            "baseUrl": "https://api-ms-assist.huxiu.com/mcp",
            "headers": {
                "Content-Type": "application/json",
                "Authorization": "Bearer ${API_KEY}"
            }
        }
    }
}
```

### Cline
```json
{
    "mcpServers": {
        "huxiu-mcp": {
            "type": "streamableHttp",
            "url": "https://api-ms-assist.huxiu.com/mcp",
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

