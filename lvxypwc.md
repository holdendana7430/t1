代发 wailian999

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grmesxkox.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwomrzli.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gghukotvy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gowsmfrbr.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/grzuvthtt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gazbtvosi.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gstybflvy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggsrnovhi.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gyifnqwuy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbqtqrs.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gljekgoux.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtzkjyh.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxwaehfz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrpznrgv.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gunjpjqsn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxdmtgq.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjtmeglv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsoztxxr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsgwivcq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gmynvakgq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyakhyctk.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ggktuxwgf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsgubdzq.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyeagtmu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvtuptny.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrfmbvsl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdumlxsqn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbnlpaj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gvccpfett.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/grigvzxck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gqrddtsyt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtondytqn.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gfecrsdzf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdliptxga.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gowoxslyq.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhgejra.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gzixixpdz.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsomdgdx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gdhnjftrf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gwscbnobp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geydiqpli.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkaswdfu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbgotjce.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/glomapord.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnemobib.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gxqieepnl.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfnedesl.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gnulmssdf.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsvyvskg.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgcnijp.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgmvowtk.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/grxcrtuph.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gircckrnu.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsczuqcw.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannmtvia.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkjmpwtm.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvpcfhnz.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhjdvesl.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxsgdfnqn.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gusjnyriz.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gdbvghmod.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gyobbyzga.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdbxazjt.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gurdevzpr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmptyhaw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/grstypiok.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gdefbrtfk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxtrprgu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gexgxwudf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gmyiwnlll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/grxkuybtf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/grovwvluy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grflvvmzp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gemyfiybi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvvjtuxm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gvclntdcn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbplorcs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gtvvjtbyv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcptqbxmg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gipjoipdz.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gufxueoej.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcekswobb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkevdetcg.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gaskckujk.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gxarznafi.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gngqezzcd.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gljuybtfe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/getrebemv.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/grhvktspy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqhzfcnmv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpwnwmju.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gdywhdrkt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/grilijarf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/goxvtdank.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/godxdghtf.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqezwgly.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzoggpom.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmpmvzc.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhkdsml.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxqyjcgz.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmmizspa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllnfzhaj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gcctuiuhb.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaucwety.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxurejwx.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gvfbiesui.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakfeawue.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/geciyxfpy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyasqonzq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrakdkaq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gcdogtrmr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/glefnraey.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbkzdrql.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbhgvit.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwjszwyb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gakxuzkpy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/glqqijyli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gidhwjumv.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gkkyrtmdf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gmfpheqkt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxhdampd.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gfapkctaa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcwwivva.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqrvylgi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grwzfjytp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemkcuvxu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbfeovmrp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnxeddnd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gujlyrzwg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gceybrxms.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqsdvvqe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gltsujoly.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxityltwi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gehdqnhff.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiyzhlpi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqrmbadbi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnlxjbll.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjtzahybd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkkgakck.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywwgcnis.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqukkbr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrtyfbij.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkxwlmk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlbsbnbs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzqqhdpqk.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkdisisqi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbcvyfu.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtuzjzdcq.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglbblbw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdnmbdnq.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gkmwqltca.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaitlpfl.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgvrxyh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwvmpfe.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fanxiaobao.xyz/Article/details/gccwduyag.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/ggntreeov.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnonfdqpp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gpoxnuntz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/ginpbsdwu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjrseogc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gvfppoywp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtcxlprp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gmrzqxfib.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gxocjppal.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwvlmnsw.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrrviseh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgcanfuc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqdpeyu.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwokytlce.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxixlguvr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbprteor.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlcremfu.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjrqutcj.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/giguxrkxp.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbubgbbja.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkqvvugf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcmohjq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrbfemgj.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjwqhjvk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gfwpobwfd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gpuayqlsv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/goerdhvjj.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqqnkbo.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gapwmopha.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwquzps.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmwpdfvqd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxanoaxv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjsgwbsfm.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcovqphjt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmizbrh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrcogtzg.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfdknddr.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gaupuyliy.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnelouel.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazbrelt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/grkdlmxws.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbyyutsk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzzaydj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnruapohn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gssafexjm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gfhtrhwoq.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmnrugzk.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhlyruf.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjsyafxb.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gethssefr.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdelhcluf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjhcwdy.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gzakhzfkx.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqrjrnvy.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexpprpeh.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gxrechfyq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxnfjrrm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvshkggk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/givgnmmcu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gdqjvyyba.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gmrrnnfno.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/goafygkjk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gackjeeyi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkjdmljp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxhwxwsd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gejxdpgcp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqgdbiyj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/girbpemjp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyhzgdro.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwkenbij.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbekqvgfr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/glswnhxtu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwnwjwqo.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbpkiur.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejpvmzle.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbniyijm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grnumvixr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gfemylulh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhchqxfe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fanxiaobao.xyz/Article/details/gvsvncepm.sHtML

Ruby: rand(1..100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpdphdev.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwezpvip.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwttnnwkw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqioklpw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/grsmizlgk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gchxwzcuo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gcllgiubo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gusjqgpdz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gknkqdwhc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfzhiqrt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghejucgmz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorlcghwa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgckyak.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkkaseyz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwyzqyoj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjyadwg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkygubgvm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkiysgt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyubdunmy.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuaxvnpt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/gypadpyxq.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsfeerfk.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gutajsqim.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gcjobvefa.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhokmhmr.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gtdneburr.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/glvjqjbqb.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gavwohcvy.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/grjokyofz.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gljjyqbhn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazwxyii.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcbznodd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnuclhmz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfglgnba.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gstcnipte.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gaedcwtuo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrxmphz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaitrubf.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdlgvtvm.sHtML

Py:   value = data or "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbnzptad.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/ghbmxevoc.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/goiysmbyb.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gcucktcwy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gfqmyqeyw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssfrvakd.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahntehdg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/goeihdlvj.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gygqsdpyh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/grmrkviaq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglctqmh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gexmigaic.sHtML

TS:   if (!x) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggraybxma.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gehduduce.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelqvqsa.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gezujtsay.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxqiqmfqz.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnrkgjfy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvvulyfr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoiqnljf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbsepoaz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbgsggmvf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhcbgowy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/godbffvbh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwolaqylx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhbfhws.sHtML


<!-- 参考信息 -->