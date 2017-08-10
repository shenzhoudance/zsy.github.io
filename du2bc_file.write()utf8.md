42h[LOG]新人血案之file.write()中utf8編碼
# 背景
將以下兩個變量x1與x2
```
x1 = {'卡片時間': 170525, '卡片數量': 8, '卡片名字': ['1.md', '2.md']}
result1 = json.dumps(x1)
x2 = {'卡片時間': 170525, '卡片數量': 8, '卡片名字': ['1.md', '2.md']}
result2 = json.dumps(x2)
```
用file.write()函數
寫入name.txt文件

# 案發現場（代碼和返回

```
# -*- coding: utf-8 -*-

x1 = {'卡片時間': 170525, '卡片數量': 8, '卡片名字': ['1.md', '2.md']}
result1 = json.dumps(x1)
x2 = {'卡片時間': 170525, '卡片數量': 8, '卡片名字': ['1.md', '2.md']}
result2 = json.dumps(x2)

with open('name2_2.txt', 'w') as f:
    f.write(result1)
    f.write(result2)
    
with open('name2_2.txt', 'r') as f:
    for line in f.readlines():
        print(line)

# 返回如下
{"\u5361\u7247\u6642\u9593": 170525, "\u5361\u7247\u6578\u91cf": 8, "\u5361\u7247\u540d\u5b57": ["1.md", "2.md"]}{"\u5361\u7247\u6642\u9593": 170525, "\u5361\u7247\u6578\u91cf": 8, "\u5361\u7247\u540d\u5b57": ["1.md", "2.md"]}
```

# 分析
utf-8編碼血案再次上演

- 方向1 --> f.write()函數調用問題
- 方向2 --> f.readlines()函數調用問題
- 方向3 --> str寫入txt文件缺失的知識？
