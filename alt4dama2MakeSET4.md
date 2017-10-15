# alt4dama2MakeSET4

# 目标
- 运行某个脚本，获得SET4指数

# 起点
- [3d[atl4dama]时间账单效能小队0916会议 ](https://github.com/DebugUself/du4proto/issues/229)
- [du4proto/src/_atl2log](https://github.com/DebugUself/du4proto/tree/atl4dama/src/_atl2log)
- [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)
- [zq1cleanning.ipynb](https://github.com/DebugUself/du4proto/blob/atl4dama/ipynb/zq1cleanning.ipynb)

## 第1轮
- 目标:使用zq0atl2types.py

#### 1.1参考
- [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)
- `cat ../raw/zoomquiet/1302--report/*.csv | cut -d "," -f 1 | sort | uniq | python zq0atl2types.py`

#### 1.2尝试
`$ cat aTLer_130201-130301_report.csv`

```
$ cut -d "," -f 1 | sort | uniq |
> python zq0atl2types.py
Traceback (most recent call last):
  File "zq0atl2types.py", line 15, in <module>
    import cbox
ModuleNotFoundError: No module named 'cbox'
```

#### 1.3行动
- 参考 [cbox 0.3.0 : Python Package Index](https://pypi.python.org/pypi/cbox)
- 终端安装`pip install -U cbox`
- 终端返回`Successfully installed cbox-0.3.0`

#### 1.4行动
- 终端输入`cat aTLer_130201-130301_report.csv | cut -d "," -f 1 | sort | uniq | python zq0atl2types.py`
- 终端返回

```
Chaos
GDG
Input
Life
Livin
O.B.P
Output
Pt0
Ukulele
上网
交流
交通
其他
娱乐
学习
家务
就医
工作
用餐
电影
睡眠
购物
阅读
```

## 第2轮
- 目标:使用zq1atl2lines.py
- 目标:使用zq2atl2act.py
- 目标:使用zq3st2sec.py 
- 目标:使用zq4uniq.py 

#### 2.1参考
- [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)
- `find path/2/raw/zoomquiet/1302--report/aTLer_*.csv | xargs -I{} python zq1atl2lines.py {} > tmp.csv`
- `cat tmp.csv | python zq2atl2act.py`

#### 2.2尝试
`cat aTLer_130201-130301_report.csv | xargs -I{} python zq1atl2lines.py {} > tmp.csv`

终端不断返回`index error`

#### 2.3行动
- 终端输入 `python zq1atl2lines.py aTLer_130201-130301_report.csv`
- 终端返回

```
2013-04-01 20:54,2013-04-02 00:35,Chaos
2013-04-01 09:18,2013-04-01 20:54,交通
2013-04-01 08:56,2013-04-01 09:18,用餐
2013-04-01 08:12,2013-04-01 08:56,Chaos
2013-04-01 03:15,2013-04-01 08:12,睡眠
2013-04-01 02:55,2013-04-01 03:15,Chaos
....#中间是3月份的每一天的数据->略去
2013-03-01 07:32,2013-03-01 08:35,Chaos
2013-03-01 00:48,2013-03-01 07:32,睡眠
2013-03-01 00:32,2013-03-01 00:48,Chaos
2013-02-28 21:56,2013-03-01 00:32,电影
```

#### 2.4问题(important)
- **完了完了，怎样才能把csv先过一遍zq0atl2types.py，再过一遍zq1atl2lines.py啊啊啊啊啊？也就是大妈说的 流水线生产**
- **比流水线生产的更低级方式是啥啊啊啊啊啊啊？**
    
## 第3轮
- 目标:比流水线生产低级的方式连续执行几个脚本


changelog
17.09.** bear init
17.10.13 bear add 第2轮(52mins)