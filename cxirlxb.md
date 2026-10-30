代发 wailian999

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtjvloohx.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gveljzjak.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxrjtui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuejxeyk.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaraloyz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjjdmxlx.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/goedugkno.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gddzajygy.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gnycbnljb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/grbfhojvt.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grymhwyww.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfixohl.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gdmbjxwfz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpitngkv.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdorqlfvn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/geocnyhpm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavvshnr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gbeubugnv.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeparrxh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfumhfgk.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gjaikkvfd.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsqwwxit.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgsicnnn.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvdcbone.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gdjlgzhdn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxwwabyb.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdqexpnu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgztnhs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkyjcubd.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gsfvjlcfj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkwdumf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfauxdyek.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ggnktevjq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmzgeolh.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gglkospwt.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gultrlpmc.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gcvvqecwx.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwfwpdh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxsotvmw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gbyeuiwgz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgywomgj.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyowanuk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdqddesfi.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/glugjsmmv.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gthkysxjc.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvwcomi.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gbspbgzue.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtsnddjen.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gureclnbq.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gddpgxvjr.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggtopiidf.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkdfobiw.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwpndruk.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gjhrervfp.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmchhruf.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/grppogyvk.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gdvfzjpbd.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupjdzeg.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gujftxvhi.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/giltqhnts.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqxsmnr.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/griopmxmg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glivvbmkx.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/goptsqlcg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzonmsr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqylehov.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvtqsrum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gtujoicog.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbdbbboe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gxtymlsha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiqvxhkv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuumaikd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaiiwbzu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gkucehzrx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpilydj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/goahmmasu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnomppyk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzgtzzs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gcbccqdrz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/goxzxerpk.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gilsprjml.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndexxddh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/giifaijma.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbycacrej.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyzimgjv.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvohcowl.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gezyioaak.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghsenaklc.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gyedkohbf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gswckiiit.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gezivbyia.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzfdcttk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gdyqrjcsj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gstergxgn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gijgmegwy.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcyfihbn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gniklibbo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/giyifhzob.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdhshvsv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmmxgxfsk.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gcscgnwbg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfialzai.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/ghdvywpjl.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqltaqvo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/grmckljpi.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gyilponpq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnzcofek.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gamfoowhw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gdzlzutpd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gqlpsnpzk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqwnzacv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gojtqtify.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqocacfgd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gmejjpilw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gycjydikq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/goywgehgc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gibxhsxoe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gqzzqeetq.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpfvgkqv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwniyclf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/guqrzchyi.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gqqkkrvqy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmbkhmjuw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqevtjjq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gorghwxqx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqeahhxn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvgccpaqx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixkdgas.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnildqsu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbtaeyirk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/genukbixw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glttslmow.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/guqjwuvos.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcdrkcjce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgtukega.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapfcjuxd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbjxsravt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gflzrrnjy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcslukpx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpszxzuyr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gipeyxazg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqqytqrhz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdabzls.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glknmhfhe.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfshvzjzf.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdfeioc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqopvrneu.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzqkbvlgz.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gobakpczb.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/guwhdlvxh.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gylqvxuxp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxwqbodu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosurkwxv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/ggfuxouiw.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkqrrkal.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwhazna.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gfbifgzpp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqeasvjd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyirkangz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtdbtfkk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhwyxipu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrnczwoa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyggedvq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiqnpasn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gexzmphlj.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gocruoauc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/ghhgktaxl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhhqlapb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gegtdroji.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggancdhlr.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gobfncgny.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gxclwyynq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopjxwgsc.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbqtucijz.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gaocqbtmm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqkipvmw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycuepxxu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuchhrxu.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/grtzaypri.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/ghugxlgge.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glerbwagq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/ggkgowtfk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/ggjsubhxi.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gyqkrzjrh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fanxiaobao.xyz/Article/details/grfsuvccj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggnhkzymh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlpttug.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gilzamkwo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlppxtrm.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnhwkxsu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfalaairf.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhkjelp.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gfahanhed.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlgsudrf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsnzyhhx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gvujmtace.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzulvywv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbijjtyip.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxlntxyh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyvzfuke.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdhfqfuz.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfzbrofb.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoeosbvc.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqounpkj.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlkafote.sHtML

TS:   String(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxppbjyc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/garwehoob.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkokuxsad.sHtML

Ruby: 42.to_s
来源：http://blog.fanxiaobao.xyz/Article/details/gmesqmqfk.sHtML

C#:   42.ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gevledaix.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/glmbkuovj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmptrolbn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiqciyle.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdugijbxb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxaeoap.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpeepmat.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfycyregj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gknppeubj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqphxyz.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gcxrfulnz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwjsakqcf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grbbsrjah.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkwapmsd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gidysaazj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkunattk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/ghiehqywe.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfzoheif.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqycgjdo.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwmzsvemy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genvmbjmr.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/gonwbdumj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhasrlb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqarcqxeg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glpockcxo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fanxiaobao.xyz/Article/details/grkticsov.sHtML

Ruby: rand(1..100)
来源：http://wap.fanxiaobao.xyz/Article/details/gwooaqpxb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwszivs.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzoxbyrq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fanxiaobao.xyz/Article/details/guhjwrftq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjiqkbt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdarzfprt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gikafsywu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjhumitp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpkmsauu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/ghpukwjwc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyhkvbaq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrxalcqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwwaewhot.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/geltevqsl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrmnmvfh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/guvaszqub.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahwlclni.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubgaisz.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/grgmoehtr.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/glbtfeiwn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/ghavkszwf.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpecxkmvm.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlplhtvn.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaypcxbh.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccgyvetx.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/grjqjurtg.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gblkxndlc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsucfqlie.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxanclquc.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gauycjlfd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfqgfjid.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/glhwlwysu.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gartqztnk.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnmovxnl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/gynztsjgd.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/grvjmzuwx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gzmjhpeek.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsfhdicx.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpygnnmfz.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktyczix.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkngtopx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtajomzy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxmnxqaq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gkrbfuqxt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqagcxoym.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/ggnessshq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/ghbmmozli.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedlyhxnk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlzukqns.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gjlvugryg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtcsrsd.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gamkxsehw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdkatft.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwpgeuoe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gcmocclbu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmcjonwt.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwbfueie.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/guxdahqth.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkveetfmv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gajlmfusv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmhwnyv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/geahscysd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufwzjqm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyomqirg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahdsqie.sHtML


<!-- 参考信息 -->