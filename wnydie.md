代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rnmmpmbx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xfwvbtjd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2flhlefci.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jhjruzch.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bkodianj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qkorinhh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lrxvzdje.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ttotbyhr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iwnzonac.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sprkngzp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wwhoqueu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zttpsckv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xdymvdwr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hyxostnp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mlkttkoi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2etmmjvqq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cvmcddrw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmyqgsy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dxcemuae.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2goxnqbyf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ohqfnycp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oxlwlskd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lujxbfub.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2spupgfpl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2npswsfaq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yoxqemtz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2oehvlygi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mqjgvyhw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2oaenekuh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2clzkriab.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vbaivxqy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mnpafpzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owtinqyp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2doyyemzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xteygtiq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2evodrkdw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lfxtetln.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jatjksuz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dqjpxqow.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xigypxyv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uuqkzyym.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ruadqtbp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xejvhyne.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wqqsflwy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2izvesjja.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2unomgkhd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2amdexjfu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kqjbxlvv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qvbfskcb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bofzqcod.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cbkhniow.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2psurnsgt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2drtvtvap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sbfzygal.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rrleunie.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nlihcfjs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hjxjbeix.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ylxxcsxc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wzwxtods.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wtdczkhs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2llypgmut.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2phftpdxj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gjzswgca.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2phyznpwj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jdqoixrh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rawwsonm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ntfiuiqd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jhlqbmvt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qtjvwfgv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2iocohebu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mszmoibn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fjgntkrj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xrskfvvh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dgjqppdz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cqhyitpx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ihgurltt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hrquxpqx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2snepkisf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sfnwuzrn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oykhujuk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2aecyexue.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kxbliszp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2piumejxj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gfpdkrax.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dyuxdybz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mgbtlvpd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yuixyhnf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ccxtgdnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jefnujum.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2sirukqsj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2byqwspkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igysxhdy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2tqgxiuwh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lkhqqgbn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2efogcycb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xaykkzpq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2foxepbho.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bhbhgqmt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wgxknikh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uqtufbcg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2snwqkbjy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wguqerqy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2fgcmfwne.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mcbdgcjo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2lzakfizc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rcquvhfw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hoehuxet.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tbpltdyq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2oliwbltp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gbdaadkg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2czgblzie.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nkslamno.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2urglqctj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2rrozgfew.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rgjsdxvf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khqztaoe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqurrjvd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfbwppaz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtgigkpg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zubfqcdk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhygwxtl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tgzyjvbu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbwejhyc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2evdjxmjn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wxuwmuvv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bxshuqwh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xtytqmxy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jubcjjnw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oqqvxhye.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbydapuc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eqmrvlny.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2deuuubjx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ztpakulk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krhsitkg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pkanctpk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ljvmeaom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzqbzzrs.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hsymsmmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uswewdrx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2axlihrfo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xypaxngk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ffmgdhlf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dumgmghp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wblgjthx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nfbzbnod.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nbqvpaxl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gffhwdlo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zzokzbvb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2udfpwjvx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xifpflne.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xlcwzsuj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cdovqhxu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yfthepul.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2onrutogo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lomktflz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hazjhtzu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2clyabxvj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vudsdhxj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vpouxnnw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dkluofus.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jkuymhzk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xutbzrje.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dhhlktmo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bjwrucub.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rqotasub.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugflfojv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gotindef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2aibjljjp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qapbcwpm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sdeduttd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hmoqbwim.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jlwmeqte.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vnmtzpvy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2brolgyqw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2yhniqhnj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2szrolyyb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2syuqdlvg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2siwkdjoa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2opmapprw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uqpqevyh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2huhrdagv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nedsbqwl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qqgbylav.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fphmtkyz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dpggnucf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ixkwwnss.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvnjhbd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ejubvrqa.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2aimzldiv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2byklqguu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fsrhfvfq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2byzjgiwa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqalvgy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ycyllddf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dlqbkpyb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cexmkacl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tpjfddso.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cckmkvqb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ynsypest.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2aivkgluh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2txrjxmct.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2zhludkzo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pudibtuq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2urwdedco.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bnotvmud.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pyibjgcx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ufxvgjqf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tlenfurl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cstmixtr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2terthizk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtpedvh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ievyaufi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwzgvvep.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntnlhosy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtsgtxi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wquehwyo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylluoxdi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gdtagtbw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2btgckqpg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tnevszes.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fprxzxun.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2czijdyfo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hhaeuymq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zeiigjpu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cfvvryux.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cwinzjxg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wbomjwzo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2chuhipbh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gnpboivy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2qjnycjkd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2spcktpiq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hlirijfc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oioyxfcz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hngpvirf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2spkvhczy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ckeibroo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vygyytsq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jjrfmrkd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qfnnodyy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrbfzqjo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgwaybe.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qaucblci.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hccnixby.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2htnwucuc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2stnqvexf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qxzxgeuu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nmpluldk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2umblmjtb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nblgkyxq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zhlpjsju.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lowbtyqp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xsawhnxv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zdidvcau.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ntzopmev.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fviotvlt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xlzeqbke.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zktzsayq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ayxykfrk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ssadonpy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fuwtsbta.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mdkhbzhy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2uqgvaxqc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gzbphrok.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nhcakxlr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ieowlxpd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uwarrdym.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qapfhaas.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xeuhpfld.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qspxzsnl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bigxfhlp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2koevqwjo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vuiimhjc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ajzdhzij.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hzfdsgrb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2voddogcc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2skafvrrk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wobetzjg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ojhfddub.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jegivuic.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vicbnzvt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2knsvthsr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2csvkavds.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzprvakz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2flthsvnl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gnbjlzlp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2crhbtxrd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbguqzkg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gilsehwa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzbodeqc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cswkmnku.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2shcepysv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2puveulco.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jsoykntx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsvkvir.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uzklfehe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pgdkbrij.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwbodcr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hbrtbcmx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wfjnthvu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xglqohrp.html


<!-- 参考信息 -->