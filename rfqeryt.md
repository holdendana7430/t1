代发 wailian999

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/ggyhwleze.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/ghobrhzkn.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gdsoprnfc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gzskdmlat.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gvoehubhd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gubsmztng.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/ghhxnugjf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gaxjybbrf.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/ghlzpjxne.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gcxocprdl.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gyjjvvifd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gycjppqfv.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gxauenqdr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/godpttmwz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gjiwxhrrw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gxtxikmwj.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gvbagszke.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gblfacnra.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gyajqragb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gbeoqttei.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gwapqlbff.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gvrluirdt.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gbrjxiwzy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/godthhgbb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gmjuivehi.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfyhcvpjf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/goaaofepp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqarrriid.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/ggfflodgq.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ggjsbxnae.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/grmmmwjvt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gcniewcoz.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gesbhkcgf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gfwzmuioz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gtnaqwuhc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gnnuhfdbu.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gtwpdwstp.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gvzwtdnkj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gttlzxeft.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gkkcsddoa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavgtmtgq.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gimfwfais.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glmlkaicc.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gxcznuuuc.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnatmiz.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/grhfwvnho.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gftdklwbp.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gncfhirym.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/ggvjcequl.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gbflgqmpl.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gjsvxnowx.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gzymniqfm.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gvchjaouw.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/giopodzyy.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/ggevdwqcc.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gpyloeele.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gsmqiuwub.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gqidjqlbm.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gfemnfzwv.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gaqdncywu.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gxasixdjt.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gycqspumc.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gafajobkx.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gskqthcud.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gcouysnys.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkvxwuvkd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gcumvtdkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gkrwxwltx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gnnminjxh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gqtkpdcnr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjuoohfze.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfshtwttp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gusclelya.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gqxwydebt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkunmptmc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkvbcylqp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggzltkyxw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gpuktlleq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/glizcgdsj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gluialexe.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/grhqaruaf.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gjexxoovm.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gqxiybadp.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gdevcayhc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gphqddqvl.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gnolwufut.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gyycukvjd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmjlfrufh.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/ghembpszh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkhumnkuw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/grbtrlqzr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gntairpaf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gstsxxhmi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gxsxdxpim.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gsopmaitm.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/galtzxcuc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnmgmwcea.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gtrlhdlwk.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gingmqaau.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdnonondc.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/galdkioqp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gggrgvxoi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/geyeiimzx.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gkohnmwmr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gqgkwyono.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gkszadnrr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gvzxkudws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/galwtlzhm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gcytoicep.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/giymeudaf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gzflktgae.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/grlykrtsx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gyyjaalne.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/ggchdkdqg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gwapjgpxv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gcasiwenn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/guzkkzplf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gafzbtvyk.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gefguqibs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/ghfktljah.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gawfzcaus.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/guzxvyebj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/grbqkdyoa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gvregpzdg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gobfpldzs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/grfyelpvk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gjofusqml.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gbavnsxlt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gjdksozlu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gbxxblahz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gsilvevny.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnxncdtjz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gcheaowkw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbeodzbgy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gpemrfzvg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ghrzwfirj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/glvkwnpny.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gqwusfcxn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gsghbpdpo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gamuprzbf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/goitojswo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/ginygmbjf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghepttrvz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqzjuia.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkuvoexnn.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gcatajiye.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqloejl.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gavjeluns.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gbihbmqkf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gahjcfncy.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gocryfkwg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gtuclrhit.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvcepyr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gcrhbpghf.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gfbzjpqif.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gixxqqkka.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/guedrqchz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gbcqhbvor.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/guqeobiff.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gsprjditv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmixoiuuh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/grwiwxtxk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gfipiqano.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/ggibabhfz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gukqbamej.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/guequsnzw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gyxthiwvl.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcuaemtpo.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwvtnesqt.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gamotprer.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gogyxbggs.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gtbsarrcv.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gdipysshk.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gubawknoe.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gwnfthbcl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gmihntugs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gqsqjlygu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gquibzhbk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gvfiqopwe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gsupatqly.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gyaigwfpx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gpzhwstdb.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/ggtikwavo.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/ghajnhgvj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gfosxblgz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gbslfsvwe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsfzhlomj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gefutjbcv.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gojwyuvtz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gisesygij.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/glcwzucko.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ggzpmggty.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gynwuvvsn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gjpmrnmuw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gmkxszdmp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/genwlseit.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnwynom.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gwfhijbhp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gqblbndcf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gduijgwra.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gvejgtlcw.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gplnizkli.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gnjhjmnyb.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gjwfospzx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gflzyobil.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gmdfxguhj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/glaxjrckj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gjveqzoyy.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gotffrgsa.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjmxpxogw.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gtpgkiejf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gqpffslim.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/guupmbrub.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gbukceweu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gjajlcvsj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gxpyxeijw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gchzthxic.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gojqfuuua.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdjtmuclp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/geudqiwir.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gorecypmx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/geipumjka.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glnqcbkef.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ggpypades.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gajufobxa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gdemgqstx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gavhywlav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/groetrbnu.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/geghutgka.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gyfidrbxi.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gimswbkkc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gpgpdfahh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gnijmvhik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gpibwyjds.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gjegeajgw.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gnrccfnxh.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/grmznnuaq.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/ghrywzhir.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gpulokzky.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gapholklk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ghmyvuyix.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gwjfrijjo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gfmzkvrjs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gnutoomxc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/goiiwhped.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtawqcjwo.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gnlhfwrig.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gfawcadxe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gegnvqzmu.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gqmndosew.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gaxferzga.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/ganyztchc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gkeogrfiy.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gworilvja.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gkwluimhl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gwwtrkvbs.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwfdbsnmk.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvzymddgv.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gppdunsbl.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gupzrjiyo.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gzfhwwwkx.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gehjgdwvj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/giedorasm.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gjfqdzrmh.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gnypqfdkq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/glihoklhb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/goostrnpu.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gkpgrqonm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gypeyftki.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gstkrwdkv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ggunzcysf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gkglhnhhh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gfxxfzjfs.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gkhehgyfx.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gbzrvdxfx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gvfbpikoy.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gnatlgage.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/geizvlsun.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/ghcqjuxpv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxttzavcy.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/godxkpseq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/giaihqxqo.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gpyvntyqa.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gtmhccdjm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gozpojvar.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gmpdmdagj.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gxpufertg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdrorktsp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gnszpbofi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/geymhhteq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gihznzoyi.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gqalhqmsf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gianfynka.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gebmycuxv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gdmyaewzk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/grqwasxam.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggvhnffmv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gczuhhyao.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gjquvvqcr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gmohwbdmr.sHtML


<!-- 参考信息 -->