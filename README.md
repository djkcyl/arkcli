# ArkCLI
一个明日方舟的小工具

## 使用方法

直接双击打开或在终端内打开，程序需要从拉取 github 拉取资源文件，如果没有代理可能会导致访问困难，谨慎使用。

程序分 cli 和 tui 两种使用模式，如果未传入任何参数，则将自动进入 tui 模式。

账号登录后会自动保存，以免每次都得登录。

本工具最大的作用是拉取服务器 sync_data 数据，可以自行用于数据分析等其他用处。

下载地址在 Release 里，目前暂不开源。

## TUI 模式

```shell
明日方舟命令行界面工具
未检测到命令, 已进入交互模式
[?] 请选择一个账号或切换账号 A60#6660
[?] 请选择功能 (Use ↑ and ↓ to choose, Enter to submit)
❯ 计算单个干员练度及详细信息
  批量计算干员练度 (仅练度百分比)
  输出账号信息
  切换账号
  退出
```


## CLI 模式

```shell
.\arkcli-win_2.1.exe -h
2025-01-23 02:42:57.480 | INFO     | arknights.gamedata:<module arknights.gamedata>:38 - 未检测到网络代理, 但发现可用代理, 将尝试使用
2025-01-23 02:42:57.821 | INFO     | arknights.gamedata:<module arknights.gamedata>:46 - 当前游戏版本: 25-01-21-15-29-57-98ea04
2025-01-23 02:42:57.821 | INFO     | arknights.gamedata:<module arknights.gamedata>:79 - 正在获取干员表
2025-01-23 02:42:57.821 | INFO     | arknights.gamedata:fetch_data:75 - 正在加载 character_table.json
2025-01-23 02:42:57.953 | INFO     | arknights.gamedata:<module arknights.gamedata>:84 - 正在获取物品表
2025-01-23 02:42:57.969 | INFO     | arknights.gamedata:fetch_data:75 - 正在加载 item_table.json
2025-01-23 02:42:58.019 | INFO     | arknights.gamedata:<module arknights.gamedata>:88 - 正在获取模组表
2025-01-23 02:42:58.020 | INFO     | arknights.gamedata:fetch_data:75 - 正在加载 uniequip_table.json
2025-01-23 02:42:58.042 | INFO     | arknights.gamedata:<module arknights.gamedata>:92 - 正在获取基建表
2025-01-23 02:42:58.045 | INFO     | arknights.gamedata:fetch_data:75 - 正在加载 building_data.json
2025-01-23 02:42:58.075 | INFO     | arknights.gamedata:<module arknights.gamedata>:96 - 正在获取物品价值表
2025-01-23 02:42:58.076 | INFO     | arknights.gamedata:fetch_data:75 - 正在加载 value
2025-01-23 02:42:58.077 | INFO     | arknights.gamedata:<module arknights.gamedata>:104 - 数据加载完成
Usage: arkcli-win_2.1.exe [OPTIONS] COMMAND [ARGS]...

  明日方舟命令行界面工具

Options:
  -h, --help  显示此帮助信息

Commands:
  batch_percentage  批量计算干员练度
  bilibili          使用 BiliBili 账号登录
  dump              输出账号信息
  official          使用官方账号登录
  percentage        计算干员练度
PS D:\Project\py_arknights>
```
