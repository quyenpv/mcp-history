# MCP History Server

Một máy chủ Model Context Protocol (MCP) cho phép lấy sự kiện "Ngày này năm xưa" từ `lichngaytot.com`.

## Tính năng

- Lấy sự kiện Lịch sử hôm nay (TODAY).
- Lấy sự kiện Lịch sử hôm qua (YESTERDAY).
- Lấy sự kiện Lịch sử ngày mai (TOMORROW).

## Sử dụng

Trong tệp cấu hình MCP Hub của bạn (ví dụ `xiaozhi-mcphub`):

```json
"mcpServers": {
    "history": {
      "command": "uvx",
      "args": ["--from", "git+https://github.com/quyenpv/mcp-history", "mcp-history"]
    },
    "zingmp3": {
       ...
    }
}
