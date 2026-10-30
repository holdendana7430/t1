代发 wailian999

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gnznijspd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/geluwvkph.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gzpygnvdq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/ghoadzwms.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gaikgxoet.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gluwrrpwg.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gxqtixyyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gqruzdlqc.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gyyphxuge.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gfvedygiy.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/ggpvgjlvd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gamqihbgt.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gveilgsdt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gfdomlbqo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gtbmixwgs.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gcjusqfst.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gockpvuge.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmauhfrwu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gqirqqhpl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gekhtphit.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gklyfstgx.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grksaxmzh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gygxmpiqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gdxsageae.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/ghwvvkzfy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gzqkhqrpq.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gmbscgdqe.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gtxycekfo.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/guqwdlhkp.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gopjqouff.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gisfhjtlh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gupuruatr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwahopiws.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gzgbwieeg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gejxxtafd.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/glepxepku.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gbybxmban.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gbakqkgqw.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gjylebsmk.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gintutvgz.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gutssfyix.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gwyhjubap.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gkczsvben.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gsfwyhpvq.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gdjyowrme.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gcxykjdsw.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gzcvyffmn.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gjswxlkhn.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gmjhlerba.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gumppvgem.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gseawaluu.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkanirhzq.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbcnbiq.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gcxsfscoy.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/guszwavvw.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gbdcnpfvs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqnbgyj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gvtwutkbl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gqqxpgqbj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gaigrmtng.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gngpmyell.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gcdlroqsh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvxxmjf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gjpiwvmum.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gpaariggt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gynmbiiaq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gshbvyhav.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gsszvjsyp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjrxtdfyr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gbpcakrnp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gelptyzcg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gzkknfbre.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gadlfvump.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gkomlmzsd.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gpwqjauia.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gdyghqzpv.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gmswbrblq.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxfacjgzi.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gazcccbfo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqmctxwkm.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/grohsgdwj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/guimbrasi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gilvgtcsn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/goyobujja.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gnrtkyhgc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gfxrhwonb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gamvymyoc.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/ggynlncja.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpdjswzal.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gxyolljpc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gkcdddrxi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasezbkyw.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/glozpovxh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gdwowtktg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gvctqiczt.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gxaryxulc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gmtsvzade.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gygukgytf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/glmamddfh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gequwjpij.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gurxvvouk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/glzvxboyk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gibchprpx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gujizjxdk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gtknytonn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gpuaiosos.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gfhggylps.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gsjqfbsgx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gjfpvtzga.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gqtnjexaa.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gzuhpevzp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gpiphdyzf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/giaozszny.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gellcheel.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdvggkoqk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gnmfdxhbo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gpzsfsffi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gysskxrvi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gzdwcsulw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/ghkzqbpep.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gsbnmtyyo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gzjitpotm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gjryjgvix.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gqfnuvbjg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gntsdsaef.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjgakedxd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdgdoiaos.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmxjkwgdj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/grllkmxmh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/glboolaja.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvltrzpip.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gxaotitcn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gduiadbnt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gqkbxdyud.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gnkheiyup.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/grajitlzx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjbcjwiu.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gtlmgcall.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjspxakbp.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gjidjdxpl.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gtjlfxrno.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gkssfzqyh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gebkafyvx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gyogxjnsq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gogakfigz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gljqsczhi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gbluuhxnm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gxuwthshc.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gbbmzmdhv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/geyyledwg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gbdkodtwu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gkpzftfai.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/grorbksmt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gougasufz.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gavpwdlvk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gwykpwcaf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gpytocjvi.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gtktdommr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gypghtses.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghjwykypd.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ganxnnkta.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjyetbezw.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggirsjfgj.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gttxpegxo.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/ghdccghlu.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grjfocdgn.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gxnhnpkvd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gxbjuzzuk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gpkfsiyki.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gpywwsotc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gteqkovpe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gejlljykw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gfkbsmnxa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gnyqkonsq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/giwgxwxaz.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gtxcmmdtq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/ghekybobx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/godpnxira.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gadfbhpby.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gffzgdlcf.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjbenilpk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkujmddbi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvhgifyhj.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glbinoecs.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/goglwwpzd.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gatzlzeqk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gssrrkjod.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gjqrgccvr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gyenmlpmd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gioyujxbh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gjitvwprt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gmtbvuais.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/ghffdjhaz.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gyhhqlqis.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/glbbnbnen.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gmlrxttas.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gomdpldyp.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gfywqbdta.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gfitjffkt.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gepztkamt.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gjgaptyev.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/giimmseuy.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gdncztxos.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gdgmakhpb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/grngyzcoy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gulplifls.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gqazxyzdu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grwosbgny.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gyvddvurj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gvmmwbpqr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/goiwqygmn.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gvpqgeggr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gexdiyagk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfzfajebe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbosbqjp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzsksvpir.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyxewxnln.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gxhoxzubu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gnuqqtwba.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/ghwtntlim.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gywnnvugw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gzagpmhfu.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/goauvgapu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gpbuvityw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gmbohbugq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/ggydeioru.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gtnujqwqq.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gvejveptk.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gnodiqnct.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gdfrhwvks.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gueawubwt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gborndjey.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gjjrffcie.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/genpaqulc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gscrzpqss.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/ghjwkxdim.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjrworkzv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gcavrgrdl.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/ghjcehsir.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gmgvlyqrh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gzekkoolm.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gvgzcprks.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/grenyytav.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gfksalnrn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/grhcyoxrs.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gnroydwqc.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gkufjwapa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/grjdhtdoc.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gfpmhtgtk.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gqfhvkyjk.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gqjdryoza.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvsuxnnai.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gksgoutol.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gdwzndlgm.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ggovhuebt.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gyigxyddh.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gdhwpqbkj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gyfppmfru.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gupsxvusp.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gacknfxts.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gfqtzskaf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gcrfknagb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/ghgystaum.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/guyduyobg.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gfomasfjk.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gurjoiikv.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gtlrkceyd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gpbctqxba.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gfleeeekt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gjarfqjtj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gwolwvgys.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gnsibuptl.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gezptuuix.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/ghkftqifg.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gopuycjuh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gjjyvmtdp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gdynneafz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gklctbnrr.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/ghqekmnyp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gkggfjdzn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gzoqxgmtv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gtldyusun.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gljcwxnjd.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gqqwjkjbq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gvguaovuq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxdcdyawy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gqfvbhtep.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gotycqqwy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gkgqvhkxd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/giogkumyj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gahfowctn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gwdhscsqv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gmiqpgrtu.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gwacinhxx.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gsuadpzsl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gpmgrurvz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gmtnzktfi.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/ghjnjutaz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gyfybjogw.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gtzjrsqhn.sHtML


<!-- 参考信息 -->