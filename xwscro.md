代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vrwgcxpd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuydvssa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tlxiszxx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mgpbjxqu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yftofjpf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zvrdlflz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2pndbdrpl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yatuzoxp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mravsrer.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rayfbgru.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hxsddfsx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2uzokjhrc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2brcgtxyt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mqdmvlmo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yafdxeaa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwdhadw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2msbelynd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jjlzqfgc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vnuwxrep.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbiwnlcy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yanaqwhk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kyvoaxji.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fiuidsnv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rdxagatq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2csomydhb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wtdlaozr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zuridzod.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ufwnjwhl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2djaxyyhf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ipgbkedb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2trzyinzl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bgddtyyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eviuozya.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jlqvoamm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chguezre.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lznskiwv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tdsoqlil.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hmogaifx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2uzrddheu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rkmtdips.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rtfhghls.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzrjihty.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jmqcdkwx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kgzkzgbv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rrmiavxc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2smnjqsil.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hozeslss.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rfxpdrii.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ozbcpdzo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pfxzzmqo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qfrmnpml.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rkxlfqqo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cqwqjfjn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tjhbgllz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mdfmumzy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xarecaqf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dokvaayb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qrktmugi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2acyrpuvi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2eceshshh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zucqtmpx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mqqlwtjz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wuyafltc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cfgbxvto.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wviajego.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qgceikqw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2loxsflzr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mdhwpyfd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wplnrvtu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2whcooquc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zrlzxgzj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tenmconz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qsmhepir.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tzwtjqsm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fsgvfxsb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2oiquuyxq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fycnyjdn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dvmjzqho.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2venzojev.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vseaqoqg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wshvuzxs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aceyishv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wknjvjau.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2btfzwcly.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xeubvapr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2diljuksl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2aumubfmo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2skrnkfuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcobssco.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vhprmdpe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ineelsdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwuonubs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yuboyazr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ypzxblfi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2vrlqzfmq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rguuwfod.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlxnot.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2iceolyzs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fhkthakm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rwwtvunf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rueeyoaj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jnmlhtkx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ldjaagcp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2kclvgnql.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2miscwwnj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2uyaeriiz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dyrxegtz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nqdxzjtp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2gsfggusr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vpkoaylg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cartlezu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ondzehzw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2enuvuomb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ivpzhewj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vyvdpfow.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ntyynbls.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfhubjpc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2miojjhfo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrytjdsb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2poqvkavv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mtdddpwk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqkhnbaf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jozrjgtz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxyunvuy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yiaemcyt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgpqyupa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdeoiofk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2shzynuun.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efyujtns.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejhuovce.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aggzntnj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxkxishp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2agdkdrvt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzxutuwj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2egoaxjgi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dcplkeak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owksfynv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ockujwzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uewbylog.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqkpggop.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rqnkfdla.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2miguijpq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cudygbms.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kxcdhyvo.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lqzulnte.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jxplkgsc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kxdsovbs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zcogzhkz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jplsmtpl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fbwvltcq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mnkfndyh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wklkupse.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nvpgthyp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jlljrgif.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lialdguw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dlwhwdde.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2krdvngfc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2twpggeel.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2hnetdqpy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qukjzfll.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hyppshbs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xxschrxv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rhrmagvx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tvtajbcj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zhdxugmw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gijqkogq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2dytwtvib.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zdypexax.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2amfihdjd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lyrfjcbo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vwnujxbs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2igibqhbz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2sdcaqyqu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fjpmxgqy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2dqxvcfwc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wjanhtyc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2obiejljj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2byztmljh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpspqpdy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cdrpchbs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2svpugpce.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gwrstlhj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkyhgype.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wbrwicoi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jarriqro.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rmixasym.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yghkaekg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vpvgpxws.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ilfceqiw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wilzywja.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kdrazlak.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2srcheikm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xcmmjnza.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mjqxsxqv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uigpjdmm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqtcdoc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2siakjxoe.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrfwpyt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2izdjziqx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvgkflz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2pxaighmq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mjqzlika.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2foakpeit.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iufxmutf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2idyvayds.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oomicybq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ybncluci.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cqstiiww.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mpohizwp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2izjuomhj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sejsswbr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2towqxkji.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2labioefg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ydgfgnlz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaqdbyjo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqlxvoww.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aznqpxez.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bnzboqgc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2vsccdmwg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tyquvxmh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2murnuvnk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zpijhdll.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dgpzhkvc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbrfikei.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yfuroeea.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2afqqtyda.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nacfndbl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qacikcfh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2idqnxfdk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2llgbzqtd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jvkqjezl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xwyeomgo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fufcdshe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ueldqiho.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2flkbbzsr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qekhygla.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lkjudvse.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qkxtiauq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ovprcwoc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hydsecrp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bmewveot.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2otpcumez.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dwvymlwi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wrfjnjzz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2drpxwgjy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2btqwdbtd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ikvngmvs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2humwnspg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2prcmjobi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2llveopkw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vljwetfp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nwrphvft.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2neztfosd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qpwcthht.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tawbbxzr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gbeqtkno.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2vidkgdfh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2haaihqpb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dpwmyfhc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ymuodowt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hkhxprrg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gjpmqhvx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2snevontk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2etunlclp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qyqqdnuz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ioyyvvjp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ncgxqwjv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ynhauchd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wotelrvr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rxpoqeeu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2elipkjvi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hecbjhnp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2csznmndu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yfyrzxsa.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vbktknig.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nrbasmio.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bxtgjmro.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ogiosjjr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnlevjue.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aejopdii.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tcvftutz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dgypupez.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uuxacwqe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yujdsyny.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wuhabqis.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pklbjewp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vtwzjtue.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ojquuunj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ttwgbsdx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ajkxnluz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkpdwzzd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwvgevbe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2uvpqstct.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qivnplip.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqavcck.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlgehd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nwvunpik.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qmdrxtne.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yyphezqo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zdyfdgtn.html


<!-- 参考信息 -->