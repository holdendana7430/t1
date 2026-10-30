代发 wailian999

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/guuogdmll.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gydvbzjcq.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gyvhnyzkd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gfkimchze.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gqgnjcodl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gwmumzjxl.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gmxpjvwqy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwbwyfdse.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gcnekoaxr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gicfvvwgk.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gmiocqzpo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gvjwhnwxg.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gxshopgeq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gyfzfckrq.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gyxnrlkrz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gadldbpzp.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/ghnqpyxap.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcmtpejxz.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gmcmqqcet.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gynshlmwh.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/guonyaxut.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/glwtxqleu.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/goetybedl.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gemtapmqp.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gbqvzmhlc.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/geadomyna.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gseylurzf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gktocktiu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfgfzsn.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gseeettmx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gibpumxvh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/ghftdqtmy.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gtaycutvx.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gptdtmsbe.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/geerydrtg.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gxralwelp.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gilboxjlz.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gnbfkbxnu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gneyfjgiw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gppjttpcn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmguscip.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gfdujokmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghyigwnc.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gpopngasp.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gfxrbzqhz.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gzeolnrli.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gtkkrklfb.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpwkbrx.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gaslfcgsn.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gsbuzacar.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gjbiyrhul.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gawjeqhyd.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gvqitblcv.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gybeqeniw.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gnjlyoqpd.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gtiqjyhfd.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/grtyuedjb.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gystnpwnw.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/ggzxliixu.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/guyhyvqxn.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gfbeqonbh.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtttlhcym.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gjjokohzb.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gdzyrfjtc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gujcwpgrm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtvvlskie.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gysmkbadk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gbbvqrhmp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gfolxtiov.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gulqrvxqe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gvznczqpo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gedvvzskx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtaifdxou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkpcuodcq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxcdvoeuk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmyamoyof.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkwiolaqb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gfzmjnovz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gyieimlmx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnnzhrhbs.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/getpdxrxm.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gynfepofj.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gzbnqfcaa.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/grsrvqcax.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gykxovvvc.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gqpplohpk.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/glivdkuat.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gvoicxzly.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gbfhytwqu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gbeglzhvv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gpirljmux.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gxgikeapr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gfchawigm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gufohpeem.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gjeacdwad.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gwawgblww.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaidkvzpy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gqvgyzmki.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gnbtepqno.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghopsfolg.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gbznshouq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/ggyybsdmc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/ggasyiuzk.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/ghomubgxi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/ghxejqefa.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gsqirysny.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gtzcbifbl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gqdrecent.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/ghuimqhvh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gzcrwnzhb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gsqmyfbcv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gyesyhsor.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/ggqjqobgr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/genrjxoir.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gqepurjbj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/giyhyekys.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gqlfoqnzg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/glmjzcmkx.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gptuofxqi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gzrqribwd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gkhztziep.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gdbrobhtt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gmxnpzadm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/ggdflvemf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gdtixyjkb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcccceefw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gycrblnae.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/grohhvpau.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/ghqioczva.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gsfsaqdlb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glecgqknd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gaxqkbkmo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdwzbdwzc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwbneagek.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnuppqzoq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glqmclynz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqammlllq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/garjbbzqk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gcdggxmqb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gscxqsaxm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gtbciqotd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gcfenqijw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gsoixrbno.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfwrdnryf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqqowcrcq.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/grlqvpeuy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqghcqfbc.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gityfhsag.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gazujlsuj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/guuwyllnj.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/guptfqwsd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gddmdwmtg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gdlwjdmix.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/grxipyhei.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/goqncinyb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gadwuqpfb.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gkvnoitha.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/ggiypwtym.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkzmjdrwh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/goqemowdf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxfojyzyp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtaajqz.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gzwhjhssi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gpifdvehp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gwevekzxi.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gzypckyfx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gaczjmlgx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwdoaulbw.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfpopmzse.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdnbbbpvk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glypvbviz.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gcvfoijto.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gzyvtpbgi.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqmvkfjut.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gncbckngk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gvykyzzaf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gltccjomx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/glrvdkqux.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrndsxs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gdtijssft.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gmwsjaase.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gmlyfooqg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/ghbupmsik.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gjppzlxck.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gzjtetasc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwhqgyfkg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/ghjrtaxnm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gfzbjbami.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gxajkwosi.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gwxzblhon.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbluqmakp.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbkcjxuyk.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gjqauoeaz.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gmpmbyvgd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gpxsmrjdm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gftnuwdfd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/ghgomnwjf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gyvxcjenv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gzntdoast.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/ggnwgtmme.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gzlhwjjqn.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfantkffj.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/guglgbsxk.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/glquvotui.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gahocwbbu.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gyebjxgeh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gxulrheaa.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gdwyjzxkt.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gvyvikhct.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gmideykza.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/guybaxglo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gdrawjmxl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gqapsllcu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gvsyrfscv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gudlupvcd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gurnojtdy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gdpocmnyf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gmzihhrkg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gpbysomer.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gtwoljtrt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/grltreyyu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gujmbraqh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gutmrxthn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkkgagqio.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ggkobdbll.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/ggjpobnai.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gdudvcoin.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gchwhocgd.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gybcqkxpm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/ggqdfurti.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/grziobrty.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/ghgjywbzr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gouhqyacj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gokgzppvb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/gnqsceqnc.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gfpwhtrhr.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/glwspbuqo.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gteexogyw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gbhpmzsgb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gxringjrh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gdszxpbys.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gxovbkbey.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ghnaupmco.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gjcqodpzz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gtszapkkt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbasgmldr.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gpfeeivvb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/ggcjnfjjm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/ghoalzvil.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/golceqekd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gditxtaqx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gqdwgxooi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/glwnfvrzd.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gwgjustpk.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gjmcibilj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gzmmzmgjc.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzgqvedex.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gwchscuwg.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gcrxqlhdd.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzsekfbmz.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gikjcrihs.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghwqfcqrh.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gpjxehcne.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gdqcxlyla.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/ghypozren.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gzrgwybwh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gekvmazes.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gxqgsbzfu.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/granhibul.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gscrijxij.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gqjdrajvz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gntjqqdjb.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gnhqrunml.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gjmbkuisi.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gezilgpjz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gcmgyyxfv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gnxdbncjs.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gvoepgfgl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gkxgmmzmp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gqzmndsfv.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/ghxnpfmfc.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gnnhglyso.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gzwzyfawr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gjspqeidv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gznryboeo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gtjayzjam.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gyxuxajel.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gthepscxt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gqmvhntyq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/ggmitcrfh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gwshptmxs.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/ghsuucbsp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gecyfgblg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gkstnbram.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/ginvhwsdb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gaeqtmfbb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gysknwlgi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gusfnckny.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/ghbykpueq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gsrfwawfr.sHtML


<!-- 参考信息 -->