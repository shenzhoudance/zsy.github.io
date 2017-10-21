# atl4dama2zq0aTL2thinking

### 1.最终统一的数据结构
- 参考 地址~~
- 原始数据结构为 Y-MM-dd hh:mm
- 最终统一的数据结构为 TS_start,TS_end,ACT_type
- 解释
    + 原始数据结构可在aTL2内置功能调试 
    + TS_start  时间戳-开始(同时也是全局 UUID担当,嘦时间精度达到 4个9 级别?)
    + TS_end    时间戳-结构
    + ACT_type  行为-类别 

#### 1.1尝试:导出格式为Y-MM-dd hh:mm的熊本的s07e51的aTL2数据
- 行动:港版iphone7,ios,aTL2,1.12.11.2版本的aTL2,居然居然格式设置里没有`Y-MM-dd hh:mm`!!震惊了
- 行动:立刻去app store更新了app->但格式设置里依然木有`Y-MM-dd hh:mm`
- 行动:可能是我的aTL2语言设置为简体中文，尝试换成英文->查看aTL2帮助->居然载入不了！！！
- 行动:折腾后发现，**居然需要用户手动输入我们期待的格式** `Y-MM-dd hh:mm`
- 行动:即使在`设置/报告/Custom CSV format 2017-10-18 08:58` 却发现，明明是`08:58pm`，显示却为`08:58`，不是24小时制！
- 搜索:`Google: atimelogger2 24hours`->无果
- 行动:折腾一会，发现 **手动输入格式调整为** `Y-MM-dd HH:mm` 可得24小时制