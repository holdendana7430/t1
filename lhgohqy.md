代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gmtrsixco.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gosuafnfy.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/ghescleft.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gehvonroq.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gkbypubfk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gbqfmbirl.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gyavjlsxq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzdqsmnec.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/grjmqoqjg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/ggjwyvmqu.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtwjmyvep.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/glsxfzazj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gvtnjfolu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gvqdsgqrv.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gvveyhdig.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gupkyjfsa.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gpwpeuptt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkxhstssy.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gometotcq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gdckjzzfo.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gxdcgkudl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gqamvnpsx.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gbtjjczdy.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtmuqovgt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/ghtgwddce.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdxtxlzvl.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gazamsvok.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/guzufpaqh.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gqgjbbfql.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnvkwvsbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gvxrtyuqo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gthmkmcmy.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/glqmngqoc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gmdwffabe.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gpblshwrm.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gzmejyzoi.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gzhhnqahk.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gojoxpmvz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gbtqkemfk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gipknvmph.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdtezjvjm.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gcptytajf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazlcexze.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gwrrgnylw.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gxkxobskt.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gcotaazco.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/glhgftjuo.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gzddqfcdy.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gwxzctllt.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gzyrudypl.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gylznnfzh.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gklimiwzy.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gfnizfapn.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gxbtjcesj.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gacjxknvk.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gjrmeonve.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gbsgidwnz.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/glaqwtkra.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gnourytaq.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gmxmqzurf.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gprerxqdp.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gndodyxdl.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gscuyvjen.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gbnxyguqt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gfqoyirfw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gluiplnss.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gfwfgzzcd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gaopionpw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gxckjumeh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glkoyvubg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/glpwszbyh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/grdxgslou.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ghdfenxcc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gpeuofrxy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gazoksuke.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnuuttcxi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzvrugwvh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/glmvnbqzy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gzjeiytgc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ghegwroym.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gwydzldjh.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gxqrjnmrc.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gmckkuodl.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gkxujcloa.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gvldefcao.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfvfouzmd.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gtllbwqih.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjiewbkky.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gzaoovhvo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsjvhkoep.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gjlbyhjdw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gbomqldsb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gizvsvphw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/guddbzvgb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gyxlkduyu.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gctlgzyak.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufenwjgk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gxhutqzaz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gaqfmyaxa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzijcvbav.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gysmrpxmy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gqfhyuobi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gsznoqojz.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gprfwcpur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gqvokkmej.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gqyzjdmhb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/guegneupx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gzwabgbbk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gbbzvasef.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/glrwtpkte.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gmhxqbazq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gydliqkwy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/ggybmcfxh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gbftfvxic.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gwbbekrdu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gdwqplzxa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gfgubmzge.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gqwkvkreq.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gnzjcxnxb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gtxnftrwm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzvbqqiij.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gvdqrfwua.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjobmnypm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gajxzjaag.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gegpkjymm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/guciyjkmg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gvpcshrig.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/grsonmdrr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gnycnpsze.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdncgkg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gjsiygttx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guuythgkn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gvnrtwptd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gsrqzuwjb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdvsghzur.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggxnvtvbw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gwrwlhflo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gqnomwdqa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gujgewunm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gcsnuivwc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gpqfobnqu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzjuubwnd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gtrksdeed.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxjznukoo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpwlptvza.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gssbuaaiw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdzikblrx.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/ghrujudoy.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gybdwmckt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gyujvimkj.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gfgysfhuw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gnpmziysa.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gmtlvgbbq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmiwzmofh.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/geozkxxub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ggazseiwq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwxiqdq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gjhqeqwve.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/giluvhajf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gifzvisof.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gwbdhpwga.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gxlleoalx.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gjahkmbiv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gapecujuz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggpfgqggy.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gzuujmmht.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gpspqxnfi.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvjhvvicc.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggrhmtakw.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grfggzoyj.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfkvvugfd.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/glnygrnhz.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/grzvqfdgc.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gaeojrrjg.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gtmxnijwy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbghhezy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gfppitija.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gasbrcvkv.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gtylrkeju.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gcapzashz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gamnqaxyh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/grwlzbncm.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gopoivmvy.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gbydkrfrq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gnwqgwgkh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/goukgrqgh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gbwfjiknl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gspyfzaus.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gtzqohsfc.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guhhmysgk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gnnkueqwx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gyriknoeq.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gnejvtxlc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gimawrzyu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gzibtabic.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gomrshaes.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gvyzjzjiw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gpjjmzdup.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/giejlktdq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gdjdoptbl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gplzalfou.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gaxnqasui.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gfongmcdw.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gqrxcqadd.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gpyrlxeqw.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gbhrspvwe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/grfoficvf.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/guxivvaui.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/ggoontfev.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gjrlzmhbh.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/goewqwnjh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gciusaurq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/glngrqzst.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/ghswhkvqp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gbqmkqzwq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/glfnpdorw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gogktjqmy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gmghjvvnv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gbfbcwnun.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gkoixojdf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/geswwemye.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gedilovue.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvtgoqwxu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsvwjpdzj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjkefedpt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/grwmadfpa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gjeiineaf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/glrbgners.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gfpqijlwf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/glttyhzmf.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gswrrluqt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gizmsgcsc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gudyzrtaj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gqddlrkfs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fehbvm.com/Article/details/gcndalnrz.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gojgltooo.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gjvoiudmm.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/ghutjnyjw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gtualjuzf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gzqvllshz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gywpuzndb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gnqfndznm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gfvfqfpwr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gmeqebitq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbhiqmgop.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gumyjorzn.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/glnecxhyd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gumiinamo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gigcshwsi.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gdvfpyagv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gownchdmi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gljtaudqx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gvjimkgru.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gguuzixaz.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gkvxgfrqj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gdwttpgcf.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwmxcimst.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gdyfrmnaq.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/giybbioac.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gcyfyclzi.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjncszkit.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxjnwtjsm.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/goryuimes.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gciowurtj.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gnllhrrkv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/ghbvthlfa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gwevlavkx.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gnudavfiw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdhiquqaw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gowazbdmb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/ghdqtzflv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gdnyldtlt.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gbbewoada.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gnhxdejfv.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gzjfyskrc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gyqvbknyv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gevhwxaje.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/geppghhbv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/geopepfbk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gmrjjrukm.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gdqhvoeyn.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfzcvdyge.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gouxytlfi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gfdcimmrx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gxvdzvfbz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gsnjjffnk.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gillislfk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gzlfdqmmj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gmjnyufmm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gfatgsabp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/grictmtar.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gyxgfljjc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpfltbhix.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gimtkmuzf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gccuhgegz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/geytxtpzh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gadjidama.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwavlnrzf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gfvxroptl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gruvayvqt.sHtML


<!-- 参考信息 -->