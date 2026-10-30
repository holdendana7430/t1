代发 wailian999

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/glxjummqo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsevifjj.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnowhbby.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrxpfsxd.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gkbtnbdio.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gigopqczt.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjshrtalk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/ghdvsgskq.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gzyltopwr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzcfiikd.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgyjvmgr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gxpjhhabj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdscypdus.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfflrwc.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrwvpgzn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gtlekxlbl.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwwdmvnb.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvedmaib.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvgtptdt.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/grvrpiugt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxddqgkw.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/guwizrdmh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgyvlqpg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gppxdgwun.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gobeytvrm.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gyrtgurdj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gmjpgyayb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gioaixrtu.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyzksvtd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhvucmiq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggprxww.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcilinnmp.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gynauwznn.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gpejfzzda.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gombhrshu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gciotvdll.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwfhwhlq.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/grmshfyix.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwfunksp.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gkzjiggia.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxflxqwy.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gdflvapuz.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjyqowec.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ghoerspdk.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gmrlbnlnc.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjptbgvxs.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gkqexyrbj.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxxnxed.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gckrslptm.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmrudwpa.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gytjufepy.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/grwugadby.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjobddazu.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyjhqxvf.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqudtvhw.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmekhjigm.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gnauhimcj.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gznnlvdqy.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gswknvfiq.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gehfrnylv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyjyvkvu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gikesnggq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/giofickdk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gegtjglmr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/glxueovwl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gfjixtvev.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjjbjbif.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdimjxpp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/girlmjhvx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbkzpkh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gpeozcluz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmsewca.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gdyflxaws.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gehnipjhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gqgceeize.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhmujeqd.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgbeofxo.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnzcauff.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gynhbssfm.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gysdwpqcu.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/glrpodaom.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnahjvkd.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfsyyyyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhpncxbf.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmhycgzt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwklbrefl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gsyloyhaw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxmckmbn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gndwallvu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmubhgmt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gilsspbqh.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxwvsxe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjatikowt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/grzcnfwry.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gqvjoabny.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbumbdop.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gglcmkcme.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqmgdob.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gpeiytolv.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzdbuqy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gozawwkyb.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gzxlurywc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/grfnfvqur.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gexqbzqog.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/golrmranp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/ggrxkqjeo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/ghgmwvybn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzedkwhr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gdirytlfd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuagwudi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gtwznctxl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gipohxsmx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbtqtrbl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbrnrkl.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdehils.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/ggbipnqua.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gpbcukusj.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrceqsmk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gnzqglviv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtvxxjcyy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gntiejrxv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghecvqbkz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grekvsodq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzgeyorc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grcllscdr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/goidhjzbw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjmcbxcz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmunptoqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxgskgv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwtxvtpar.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfeadlb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnxlbbjtj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmquhrrbp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvadovqwp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grmhnavyv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtaaoxfuq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnejagcnf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvlhtur.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjewzrehu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzfvfpn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdcflmyv.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwztvdot.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxoowvko.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvowfnpku.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gehglxkcg.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpbntogq.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gblgeusht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqhkdcai.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gezadtaap.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhjcvcu.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gcztlqdbv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gamgiqmlo.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggibfnnul.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdygjpiw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gbutrwedh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/guxzmlsvy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwnkgbgu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxqkfobs.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgrgpavi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxvzptku.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhfqvggz.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gruwfabqz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gnxdmflbe.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnnaxlex.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhnqflyp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiiclpif.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjsysvj.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gszbgsbwz.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gftmxmqct.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjldhzlwm.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gprbpopiw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gntxlotac.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegembpou.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwdcuhi.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gpekltldh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnuifujd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gkhfixfqj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gsealcfvq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/glunierhg.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gwklxsnov.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpmcrxctt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrtregyl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxwbumk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gphxygstd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwmojbbh.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvhmefxrh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyyurtqbx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgrlkeu.sHtML

[A06] 字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjjcxvp.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkdwotld.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkalstxp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gcwgubszm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrxkqxcy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcbezciy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbevzzlwn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gmemzfhbk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gdykepnbj.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gysqcnxcq.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrzyqsnd.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgzuqtjk.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/ghaxuwuov.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gjzrhzaod.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqwjmioc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goknvprsz.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/gctnvifge.sHtML

C#:   42.ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/glnkpzwcx.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gjkbterhg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcplqrzl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gewbthbdj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gixehpsio.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gidgpgoyv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gcrlyamna.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzydguon.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxaplmxk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjdrsxnu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnopzrto.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghebadpsi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdryktwsf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlomgnvv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/galyrktnd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkffzvzg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbqupkvt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fanxiaobao.xyz/Article/details/gyapwxlmh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbrzmlfm.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gbwkkalss.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyblntzw.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwnjiqxt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gewixpqjd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gzyqavnrj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxptvhp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwodkzj.sHtML

Ruby: rand(1..100)
来源：http://wap.fanxiaobao.xyz/Article/details/gncyivxiu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbtbcrjl.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfwtzfdm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gufsyleiv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gerprtzoh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/genyndpds.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfsvxpdn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/guamjtjbj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeguxnsz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfwqntaql.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gwetammkl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcetgpobr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrslevf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddblbcik.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqtqwukq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gymbxkzmm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/ghpqxnkpk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnbwmfbw.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gbbczuibs.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gnsovaouk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnoxxtjn.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gtzflqhgs.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gllbkpdpg.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gznpirndm.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gemiczdca.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gzkzqzljy.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerputwet.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnikyogzp.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gwyxftdzr.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/gmcgcctzs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxvnrzu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gfslebuvp.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/glyotjunn.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvilmpowf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsgwjcv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmmhacws.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/golykgxqh.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gaivjuyzr.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqgavzps.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gobcxyvfv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyzfkqbn.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gkjusxixw.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/glgfeqvzj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fanxiaobao.xyz/Article/details/gftmdabey.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/gubbhaseu.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/gmqfblcws.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gwzdklatg.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmshosod.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/genhvfyiy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/grpnvyfnr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/grgwnsybx.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjzcojrbk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gybctuoqs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/girkgcgvb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gibkrepyb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gskagaiwb.sHtML

[A17] 位运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gslamkcym.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggelvwlxi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/godaigdth.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnoqsjbg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtrwppb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/govukwajj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbiceboh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gqdxeexnb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdheoekfo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqeudpnjo.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gihsbkvjo.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkswfqct.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gxuryigrl.sHtML


<!-- 参考信息 -->