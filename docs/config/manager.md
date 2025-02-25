# 番剧管理设置

## WebUI 配置

![proxy](../image/config/manager.png){width=500}{class=ab-shadow-card}

<br/>

- **Enable** 为是否启用番剧管理，如果不启用番剧管理，下面的配置项将不会生效。
- **Rename method** 为重命名方式，目前支持
  - `pn` 为 `Torrent Title S0XE0X.mp4` 的方式。
  - `advance` 为 `Official Title S0XE0X.mp4` 的方式。
  - `none` 为不重命名。
- **Eps complete** 为是否补全当季番剧，如果开启，则会补全当季番剧，如果关闭，则不会补全当季番剧。
- **Add group tag** 为是否在下载规则中添加番剧组标签，如果开启，则会在下载规则中添加番剧组标签。
- **Delete bad torrent** 为是否删除错误的种子，如果开启，则会删除错误的种子。
- [文件路径以及重命名相关][1]

## `config.json` 中的配置选项

在配置文件中对应选项如下：

配置文件部分：`bangumi_manager`

| 参数名                | 参数说明            | 参数类型 | WebUI 对应选项 | 默认值   |
|--------------------|-----------------|------|------------|-------|
| enable             | 番剧管理是否启用        | 布尔值  | 番剧管理是否启用   | true  |
| eps_complete       | 是否补全当季番剧        | 布尔值  | 番剧补全       | false |
| rename_method      | 重命名方式           | 字符串  | 重命名方式      | pn    |
| group_tag          | 是否在下载规则中添加番剧组标签 | 布尔值  | 番剧组标签      | false |
| remove_bad_torrent | 是否删除错误的种子       | 布尔值  | 种子删除       | false |


[1]:   https://www.autobangumi.org/use/%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.html#%E6%96%87%E4%BB%B6%E8%B7%AF%E5%BE%84%E4%BB%A5%E5%8F%8A%E9%87%8D%E5%91%BD%E5%90%8D%E7%9B%B8%E5%85%B3