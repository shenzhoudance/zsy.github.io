# SET指数在哪里

### 问题1.现成的2014年大妈SET数据通过哪个脚本生成的？
  + [du4proto/mx_set4_zq2014_data.ipynb](https://github.com/DebugUself/du4proto/blob/atl4dama/ipynb/mx_set4_zq2014_data.ipynb)
    * 本地运行该ipynb文件时，firefox浏览器崩溃
    * firefox在线查看ipynb文件，代码和运行结果皆可见
      - 2014年SET每次只能算1周，即，小明可能算了52次。
  + [du4proto/lgh3lineplotSET40918.ipynb](https://github.com/DebugUself/du4proto/blob/atl4dama/ipynb/lgh3lineplotSET40918.ipynb)
    * 该ipynb中的csv并不存在于atl4dama分支上
- 结论
  + 目前atl4dama分支上并 有 **熊本可直接使用的** **2014年第1周SET** 数据
- Timelog
  + 39mins
![screen shot 2017-09-23 at 11 10 52 am](https://user-images.githubusercontent.com/19412465/30769706-362c253e-a051-11e7-8b34-8f1f60182562.png)

### 问题2.小鹤生成SET折线图的源数据在哪里？
- [du4proto/lgh3lineplotSET40918.ipynb](https://github.com/DebugUself/du4proto/blob/atl4dama/ipynb/lgh3lineplotSET40918.ipynb)ipnb中源数据显示为`tr = pd.read_csv('/Users/liguanghe/atl4dama/src/_atl2log/atl2SET4dama_all.csv',names=['year','week','set4'])`
    + slack@mxclover回复 `atl2SET4dama_all.csv` 可通过运行[du4proto/src/_atl2log at atl4dama](https://github.com/DebugUself/du4proto/tree/atl4dama/src/_atl2log)获得

### 大妈怼
> @zhangshiying  <-- 
是也乎 ╮(╯▽╰)╭
仓库中不应放中间结果
讲真的话…最终数据结果也不应放
凡是通过程序运算获得的…
只要运算过程不是特别费电…都不该收仓库

# SET可通过运行[du4proto/src/_atl2log at atl4dama](https://github.com/DebugUself/du4proto/tree/atl4dama/src/_atl2log)获得

