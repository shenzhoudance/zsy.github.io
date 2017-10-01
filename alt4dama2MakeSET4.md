# alt4dama2MakeSET4

#### 目标
  + 运行某个脚本，获得SET4指数

#### 起点
  + [3d[atl4dama]时间账单效能小队0916会议 ](https://github.com/DebugUself/du4proto/issues/229)
  + [du4proto/src/_atl2log](https://github.com/DebugUself/du4proto/tree/atl4dama/src/_atl2log)
  + [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)

#### 行动1
  + 使用zq0atl2types.py

#### 1.1参考
  + [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)

#### 1.2尝试
  + `$ cat aTLer_130201-130301_report.csv`
  + 
```
$ cut -d "," -f 1 | sort | uniq |
> python zq0atl2types.py
Traceback (most recent call last):
  File "zq0atl2types.py", line 15, in <module>
    import cbox
ModuleNotFoundError: No module named 'cbox'
```

#### 行动2
  + 查看[zq1cleanning.ipynb](https://github.com/DebugUself/du4proto/blob/atl4dama/ipynb/zq1cleanning.ipynb)

#### 2.1参考
  + [du4proto/README](https://github.com/DebugUself/du4proto/blob/atl4dama/src/_atl2log/README.md)

#### 2.2尝试
