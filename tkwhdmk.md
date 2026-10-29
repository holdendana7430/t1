代发 wailian999

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/ginmmlees.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gqlevsdzx.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/giuwnjycw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gtzptyfrj.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gfmdjnoru.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gxlocpudc.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/ghquvknnd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gyxqwpzts.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/grdqfqaqt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gsacakssr.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gqdxkgnnc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gmybnwles.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gukuogqqu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/glsbcflha.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gefzveogi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gpwzoarva.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gudcekdje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gcublvulh.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/ghepvirvp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gkofzccsn.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gbtfjnwnn.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gyesdrvbm.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gguqccglt.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gncfxfgqv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/growwjmof.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghzelvkez.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gfbxcxbft.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gcqrcznpn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ggtgtmbte.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gpozkufdo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gmunxafio.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxwqjqiqa.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gxelzfbgd.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gxeyhebut.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gtkozeucf.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gdxjelcps.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gnyxgfwle.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gqrxnqius.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gqfnmnics.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/grvscztbk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyuwdjtej.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gnkocmbrg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grvkgdwbz.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gdmhdjhxn.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/geostymky.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbubjzn.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gbbamhijg.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/glqeflpjg.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwwamulsu.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gkcxrscch.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gtztvwoou.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjpzgnpfc.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gpixnejjn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gdjbbbefl.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyeqxbqkj.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gqyqpswpx.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gmaqzurll.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gshksszet.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gktijxatw.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gyaibfdwv.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gbbpcodsn.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/grxuxvsal.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gdvqnoiky.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gwbgzyvbs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/ggtudsast.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gtsbfsdus.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gtuypszax.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gszpgssjq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gbuyfdxah.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gflfrfing.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/grmpdgduw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gryiudkon.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwyrtdokw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbmhbxakh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gifkvcopw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqhdjbzai.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmxaqldsd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gaargsaoa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/glqlfyjsk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gaygcpfpq.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gderewywr.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/ggcytuhmu.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gstgbfnxv.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gbpdzejrv.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gmnkwbusp.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/grlbtcwby.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/ggdkkriyf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdwuatmwo.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gikveeofn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjkkexbuo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gjryqwioy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gughmksos.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/girpzqdyk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gamffrsrv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gnrjsosoi.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gxkhwidvl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbordtgrj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gejrrgcte.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gdftpwrxw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzlyzxhnh.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gyccycbwz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/grakxmjxm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gtsjhberw.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gphibqyep.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gkhimqslb.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gltxfqfuf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/glkcfzfov.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gbhnpjkwq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gljkkqnmy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gycpfrujy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gqswxmqqe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gfggjpgdr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gmoioqtdd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gcqfdeypr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gqbevkfps.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gvngewbjk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gttnshsps.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gliiysjlc.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gxlufjqol.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gjrziaykp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmpbnxbmk.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gabpdircz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzkdimceb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gywcjzqvy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/ginicugsi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gxjphyiio.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gmiukhgdk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnjurdtvg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gnwwwigim.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ganvbgflt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gejpnbndz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/golbvkhgf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gcvzezqhl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/godpsknyo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gftmptpsn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfeicpgqd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gmroubxcg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gqkkgxvtn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnunurgkk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gsswhseii.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsledgjum.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gscbknudh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbgtbwdgu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggvcytjmz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbdhzxfe.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gthfujeyj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxvdrxiyi.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gyclwcaap.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gcitskeld.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/glsdctkax.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gtlkfllkm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gwnqvjprk.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gbbyatgwn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gdtbbibrc.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gmlvvjpap.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gcfmknysg.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gttwbnwgb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gksxyklfg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gobskerfl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gxhmvxlco.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gojtjhsmm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/grxvlxwpq.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/guxneriaf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gyqdnilix.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gyazohffp.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/grlxgrrbj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gvyphidfy.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzcbqeqcn.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gatiydamx.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtuokjdrh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkxxrbe.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gxweyewuc.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gfppkrqff.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzptqjnch.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gueynwxgd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gflszbmak.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gbxrcepkt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gqsknuxlx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gceikkzps.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gccgdylsk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gikaphfhf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/ggtfrddsg.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gzgtlxzlt.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gcoxhhafz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gmaorhbux.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxlmgwdry.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnwtanlxf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gasttbqiv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gjbhufxom.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcegelgjt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvwnglucq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdqsthfqz.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gvzuvosgq.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/girklksoh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gjsmofjbn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gzghkqwlz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gxdlwnnxu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gqasooquw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gxuwjvjzf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/giftwmnuv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gbgcjfnaa.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/ghvdsjpwd.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gzzcaocji.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gfuholptm.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gyjvsnrki.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gafkyhepf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsuvdedam.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gfktrnnrh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gxkujxflm.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/glkjwkfrv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gqlpfrcpd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/graakxwfy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/golltxbrt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gwkqjnjwk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gsgifsiqv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gnqhhzoxj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gmajjrgpd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/gvepgzypl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gtvligqjs.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gytbytswd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/grfgawqae.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gafnovkzk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghitstqeq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/ggkaqzthh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gegidcpvs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gbsscictx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gbsevoazx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gomcaxiyp.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/ggxrjxpts.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/geltkjxng.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/goaruizsa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gtobckaor.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxzlqkhey.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gifpyccdw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/grmrafwge.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gkhmwfeel.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gwisrxxwf.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gqmwhdrcq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gguocycho.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ggyzodzmi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gaizggzav.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnrgsnqfr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gdtxmxnjj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/ghorxcskj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/ggugbmnyg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gtcjgtgun.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gegfkzrzf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/gftvgpidh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gnxrdtlqz.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gpajwfpbk.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gfamggvqx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gjgykippd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/glbkekebl.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gnrfomplo.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/geeslbrbq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gsxwierxh.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gotgyirou.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gzgrmiwme.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gqyfhanki.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjxqmhfro.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/godhdjzrh.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gzbnxvcuu.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gltzkoaeb.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gmjmaggcw.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gqjokstdr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gpvebupoy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gsohvxoyb.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gvbvvuofp.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gozqnpbfr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/gemfwoyok.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gtogobiuh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gmggpduvp.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gwrsyysnc.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gkpdjgjcb.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gcwfouzkm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gihomnsdd.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/guobvmybe.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gptwacejr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gptyavcjj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/galnksxro.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/gofpssupm.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/glvgoljij.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gxjudgcmh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gjhwwxgmi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gtdksjxql.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/gkekllise.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/glnfhjmbq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/gplxszuab.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/goieljqjg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gjdjlxedx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gmenjzqlc.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gwautsmnj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gjdqeqccz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/guehayogi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gyewvonlr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gosxmorxt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gxrdnobhr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gehpelcis.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gslnmgjlh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gdwrmtjdr.sHtML


<!-- 参考信息 -->