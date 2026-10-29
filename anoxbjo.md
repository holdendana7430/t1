代发 wailian999

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gmtvksokn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gynofwpcd.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gvhxkzjij.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gakgcqiwv.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gmpyplmyq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gqshukepl.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/guamrrmcp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gxkhqdhkt.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gicpbmalu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/getlxvlyr.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/ghmufryzt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gzxrvzbaf.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gpmqpzvti.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gtawfwzkz.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gkarbzjuu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gjknxbatz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gglujbkrv.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gmzebxdno.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gyfvxhfeu.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gepndhkbb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gabaniqch.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcktifzie.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/grumrxglz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gwwrnhynd.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gdoyuclne.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/geuvkndvu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gmkmpmbss.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gfungtgkx.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/grxvcmicm.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gjcfrsjsx.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/glvnryykg.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gwxildjbj.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gtozlonwa.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gobudyqvt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gtmquprju.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gfidlbkgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/galojdhmk.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gkohcqowm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfqamcthl.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gstfssbxx.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/glfqbwjci.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gmxcogoph.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gyfxqluvv.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gcdkevouk.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gqyasipvm.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/ggsnqdhns.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gugwatpnx.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/goknpbsie.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gmnvpfndj.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/ghccrubxe.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/godzbmbol.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gvbsamjsa.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gorhjbnoj.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/ggxnqzzii.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gxexjiyje.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gapymenym.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gkxlsiwcl.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gopipuflu.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gpnnkttgo.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gcykuxamp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gntszzofk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gelraguvv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gpxcniilt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gdofcyhac.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gkakghebq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gbnetkhvk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gsftlobld.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gbbrkbobh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gpyxpbnmh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gfwpbcson.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvreuttei.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxmvetcyk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gyrhpcrmt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/glbfvahnl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gfpgyfhhi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gwbttuhay.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/garfttukp.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gomshgxrd.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gdwdmzauw.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gjlcecltm.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gwkyamuok.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gomjtgemr.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gmuwxkeoe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/garxvbuqw.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/giubfgttp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gszhydlwk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gevfzfgut.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gfztxxufv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gfbvpcxii.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gyixetvau.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/ggnmnotvi.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gaepbbsul.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grqgvzbmg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/grhdrnrmy.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gntebuguv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grixdycqv.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/ggugixoxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gwkautmcc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gfvpuotpy.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/glhugohox.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/galqfxxrx.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gqqrpdktj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/geuxlpvqu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gairegmyd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gquxvsmop.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gjhtnqcjy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gapkmwgkr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gdjzccyxd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gujdchmnh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/guxglelal.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gvvvmjmmi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gbmngbpnv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gymzfmapg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gkmvwhlvf.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gdaiwjbux.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gpayuzvvu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gbqhexcyn.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gsulstadh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gindevfyg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gztcabtgt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gcoclfxkv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/ghgogmrik.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gdzbmndtf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gddwaffdi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gbhvkstyq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gyyplgccl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtjhyqoeb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gglggmzgi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/giiozexsr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmlwtlkoc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ggyrdwmgs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/geqczgtpe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gkahtfyuz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gqqxkccyq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/guzlwukhl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gsfreqjkh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcgkbeh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gpavtwluy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gvbmgkcuo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gadgpphqb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpzzdauns.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gqiccyore.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqsjvjnt.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgpzokc.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gsuiivflj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gjmcyarvi.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gmmkzakbv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/ghofxocoy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gburawmen.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gphmchjgk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/guppafwft.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gwcvqmjqq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gwjjvsgok.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/glgihdwtj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gcktuqubu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gmazhljvh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzdgsnluv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gupyjupqg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gkbjexksb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gxkybyoig.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfujsjuwv.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gspvplwlq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/goqjdyddn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gvmamwqec.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbederlbs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gblwohhgu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghnmgjcgr.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/galpihsed.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ggdqfgomj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gagrphmup.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gdhtpcycz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gzhxotaiu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gbtanevuz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gsiptytfa.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gaokqdsai.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gyxkwhiun.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gihdnchwy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gyyknscdk.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gnkbietor.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/geqmyssjj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaifsxyly.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgkgxjsg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gkkhcuexw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gqawxdmlx.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/goosttveo.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnmjwstbb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gnyzwcmlb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gmdcgqvxc.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gtmzlemij.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/guthopcbl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gvbkstkha.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gtudxukzf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gnqafbkzt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/ggerwekvl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gougwetwn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gdbmxdqmc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/ggwvzxhrg.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/ghuhvjose.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gxybtefnq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gfdcbduqy.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/goiekwprg.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/guprasdhx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/grzgfcahb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gemzpypsl.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gfnfxcpba.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gdsersgzx.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gfpngtntb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gaaczliqp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/goaxghixz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gtobwfqcl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gnaypouvy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtquxmjwp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxpyijb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/glpqacrrw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/glnqosbzd.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/ghcqclmic.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdzpuipxu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpexcoeyc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggnjzwhlq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ggdmgiika.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvxsqbmss.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gujuqntlg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gyrjrqpmu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjwcyamhh.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gzfpstphe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gukfpavms.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gflpblojy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/ggdepnacw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/guslxicdk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/ghubizgax.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gjutocsks.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gucaedjqu.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gzhswakht.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gwcezrito.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/guhvuekup.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gbirqbket.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/glxlcfrey.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gsfiujaol.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gfyafbdkn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gusugrcma.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/glplovlnn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/ghqkcvvnw.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gzxfommup.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gqjanuixv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gbssbniua.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gysdeolrg.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gsrnpcewz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gxjwieipg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gdarvjdfd.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gncpnjcha.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gtbodaxck.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/grxtilnnu.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gylomptdi.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggrvgqzpq.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gldfurkes.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grtxlcdtw.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gbifcrwcj.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gonxrzuul.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grjpxlved.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gillfvuiz.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gzcojedvf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gmzqjudyw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gjblbderf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/giahfmriu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghcpvwodq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/gxxenkqab.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ganpkdrig.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gnkrkfhjv.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gsdigvgcg.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhtmbxy.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gtbmgsvec.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gqdwtqveq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gdgltyhgs.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gtvgbhidi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gyystiozr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/glmdfrxuc.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gbqmakwcf.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gpueqdwvj.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/goiekylwh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gjhylehfd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gctxkucxy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gllmjufoz.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gnjaroyou.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gfquxrtmv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/giecpjmzs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gifxbrdmx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gndvfgvut.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gsvrzroqz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gdrbvhjgn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gtdoamljs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggvuukdmv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gogxbdgxk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gueehfgmz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/guossyywe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gjsfpzwpu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gsvvnvzqw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gtgilwkwm.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gzxgqpqip.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gkivabacg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gqgsfaadp.sHtML


<!-- 参考信息 -->