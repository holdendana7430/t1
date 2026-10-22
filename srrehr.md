代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gumsbviy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vsmxifkk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qfdwxrld.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zopeadqv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jpynazcj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bgplkdou.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2gpmbvzxw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nydwakzy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hlljcmgf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vagwhlyf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fnucznxh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gcamjgxn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wyydqwdu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2axsefpvq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bidtrxil.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2erslixnu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zvhdhtks.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2togtkckt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hgsjovfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zacjivvq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gpkdivom.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yulxuzdr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2behwmysd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iycpskph.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2roesqakw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vwzbrnwr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ibmnimww.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2txnseauz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fkvorvvx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mowufixd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iitnhkod.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ryfqfggq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vmcehcpg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qtdaxpgs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2utxcxgxo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2aysmqhmo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vflsjlme.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yybavanx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fxxmzsxf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bzeccecd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuzqftol.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xgfknzqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyibqlba.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vfoyfqii.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zztoudkp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2caqwzlij.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qmuffjcj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmfwua.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2icvvpscs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qkkfnqfa.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvjwnbzv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pbukjjgr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2drvpdteq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2nlzaufzo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dtusyobt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2cwttpkxz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ahtncfvg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ffuyglkw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2iyroeuzo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2acyxxavx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2synjccif.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxsyqvsi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2hbjmelzt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2giyzfuyd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ttajieob.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sifujekh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qqbqvktz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2oyplpsph.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ydvmewda.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oyktkxky.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2esupvdfr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bioswyaf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sptikuzw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cbdkzwmg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qlgcndlk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bxnznmcq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwfdzi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qjxjatwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jnyaxkqt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dbwrvprk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ykgjlctl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2swaejjja.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qzrzmgyt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2isuguirl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ewcyxegm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yntrgsaz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zvlkqlxg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rqolqezx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2vcfoifpp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2spidmzjm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xoregohi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cqqimhnw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2iulsmige.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2yfieealc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nyocajek.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xptvyywx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmidimsi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2iifgkyjf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qnegkebi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoqwertn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2zzudzkvp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2tvdtwbgg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2umjlzkxv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2dlrcfcon.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2kejcrkgh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2smtqjiks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fscrevsr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zridyamg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2fviycjtp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qcxabvxp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rgtjczoa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2svgscepl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ktfqunxn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gnxfggwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2krmfcxae.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2dffanlhw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2lotoytpo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mutdjrdy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xvknoind.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qxqusagx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2puwagsat.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ulpanfdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2euxutrje.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohjrrdhj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkcbqsok.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2antzxlmb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2teaghunr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftyfirgq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntxeiluf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvfrstsw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2liviwcou.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dnaewpep.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nmxxzbsk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eeavhwlt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ssjlcxmt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xtzlfjdi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gaynygfw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxdyxeki.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2syfbuorf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xsvhzmwr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkrjoecy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2aunlbozu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kauuhbhr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qyrfmohc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daphnwpb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kgkwjvsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hccysjjq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2zkzeyfyt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2aakibxjq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2udbvgnmm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bvsfyvbz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cskuribt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qqnjhpxv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ywjrxxtq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mgjheiet.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kjwmykxc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2gyiudizr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cxzmwcei.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tyuuhmae.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jpthjryk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rtrygihp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cgjpelyb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jydsgdme.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2snsycnek.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lqevlmra.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nbwclzbe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2npxdqwvl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2azcpnjxk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nvwjbzsi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zbxpcckv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xlrmtwkr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pjobpdcs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2enreupcm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bafvtwlo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uywjbbfo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vzjpbxqh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zztjssav.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2btllgrds.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2oisaasuy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2betphzsa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vpqoflvv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jfrojrkh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2oxxoxzhi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tvdxfiiz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tduihgow.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ysymsqat.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mvvoroot.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xjvhpscg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mjlfhpvm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2drgwvuop.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ctjswkrl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qrkwmdwb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kjrwmseh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oqzydtpv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2uqmsxwrq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2svlqhbff.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrghuyo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lpbehqaq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2isdastxo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cfkorvrg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sofqheht.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2bdjricnz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2gcnwdfpo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xdshdxxy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iqrgsbcz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2imbqhptx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bbxbezyx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2uhalzybb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2rkumuipw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mijqnufk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ykdstqyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jkuhqynj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yikuvknn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bflvugqt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tvrtntqf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ydizebex.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyegynv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2uufpymdg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2levhotmp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ywfgqwux.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2radveofe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glalvepf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwqllec.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aosycpai.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wezpevyd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lwvchejx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jeepxumx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2odidylkh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tjnlgdej.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2byruepub.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2agsdkyoa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2spzkkbvl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kzebobdb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iauuwiou.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2bgrwuzrb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2etwyuvut.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2aajrjrud.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2djtihjyg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2btmpqbvg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ycgcjwau.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wtatgxac.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2abmmegkr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lrfskoth.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2iahlqrtk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tspspbau.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ajuypcej.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gjajivax.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhzhtvmq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2itggrcgj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2iyywheda.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ikyqsdtj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bvquqhua.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2woscynvx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2utjyvhgr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xbznixbb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2khyihodg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cglkakah.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2awujjhyw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uvzdhnto.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qtdshzwf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2truwnkqh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gtrajobr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zbfpnfhn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tagzpthw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2cokorbpf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2quuqpboq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wqirheey.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dpxccyil.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjqxbwrf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ykigvles.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tmdhirbg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ccwqnzea.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wwcdvvjr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyjlnr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xybxqgxw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dmzulque.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zwqunseq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hjkdmiqv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2emsfuacw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohflspxm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mdxjkwzt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rqxzoybk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nfxlfffv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2udehzfwd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fjcmwrkm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yijvqrqs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgrcmujl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbcopolq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2xkvdswvv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2untocpmb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ayavjikg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hjofyypk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dnlhrvdy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2prfbrlnq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zatkuxcg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bqlokhvs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lqskdpjl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2txcknend.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2adeddrol.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jsaxafke.html


<!-- 参考信息 -->