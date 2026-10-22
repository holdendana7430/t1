代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2esoyqvfw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yuhdptoe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qfllmoof.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vhmfrpyr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qrokxwps.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2esypvrei.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kdlddoqz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2sdsblzgi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ygbytmle.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2htpvkanr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jlpscexd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2giclqplf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vhdmkdzf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zyedvfcj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ybejswqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2oclrltoa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pcpasbbc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zzppihvr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2laahfkas.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dftksjaf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vysojrwc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldffngzd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2sosutsad.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fqsebcix.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2osrypaxz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dluxrhdm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2knlyecum.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rffsrzfh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kchfyjye.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2oiwnewol.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2msdckvpn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wueoivyv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2eyraomby.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ldyhkhbb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2anakjnai.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tkwqdiww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zutcatne.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nefmoyet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxaletkm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kqhffynz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gtztgnei.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rprmcpgk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xurjwzji.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2agsykaaj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eqkxhzdm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ufwwxqjx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yogoixup.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sxonvesh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ebdayqgz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hmeslfmz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mzlrgkin.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2oxcncgxs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dwdbvhid.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dsdmhtsf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pcigxykh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xqfrpgjx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lltcmgto.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xwlehzbh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tpfpurfm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sceozgee.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rhjksmmh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mrqzuopl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gsvxzldk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gytnxnfl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2livriifh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jtilkybq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hjfskcfr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bwwahuuz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixbakzis.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ofrshusx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2stdibpar.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vftzcuke.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kcuvyfce.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2caafoqot.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zuoqetdd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sllbeiij.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qcdnmepe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2stxhqvow.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qdcmxdwb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2omfctzeh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jkkmrwnr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2srjhydvv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2nejsndoh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yzbmljjd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ynlmmviq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cvzxnxbt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2apksavgc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2crkezegs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2siepjgjs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zegqvuzv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hsqotpgr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ccgckpal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewyzrxbp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jdptvuie.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2usxxjqrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmiftamj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qoqdomgx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2oupxfepf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fopxoabf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vlptiiza.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pibtvxar.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vhnmtwzj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2auhsyaru.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fedfkjrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2lzxondql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bnxcxdse.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ibtnkmay.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wbikanfi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rcdwupdv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xgyafzbp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jvcjmxaz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sjexgxbu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2aqujmson.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2jtsckebk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dsxfwqqi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2oiniwxew.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2blpetqyi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zrufllkm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uqauyrvg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xtulinuz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yehmzifv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ezxvgpsh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rfbhnuhu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ikelauqf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2beltsvdu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqgiqcqw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2motyyuwo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqujigfm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abzxxmow.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2niyijouw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lofluxub.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kcbunfsl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zmbstpgm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jldicxnp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jmvegvsm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejkzmrdh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ykyasoqv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2joawmdgb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rahjksdk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xyalkipp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abzlvozu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2egkdpsoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmharkys.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gfszysfh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ubzeolpu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jhphlcdm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2skteiapf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2srosixji.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qqjxxuwa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bccokbco.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kjpdzpwy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jyvuyhgo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tjvmmnka.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fuzdrrhx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vopubevl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hlxyqiou.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qvwoyeqa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rohrfpbr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ndaapoxo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yvjruwde.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ukiezynt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zuqbkokq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qbspqwgj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iecvvakx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xhhscydm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2plgkccmv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gizjjhvz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sxyfbpdp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zxxokzgb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dcmbtuso.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqtrrrxn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kqkdyezb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2msplmnyk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2memxkwic.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pjqjphmi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jdjsmwbk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2evtfbkki.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2svydagal.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ruetkniy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2esnsskmb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvucfdlo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ijdxffli.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hushhumg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2olcgyito.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qpbickrl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2grerzwdz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vkzwzhyb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nqmcaoqa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kkzbntcn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tjevgpmp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gzutfrzm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xvdmfqlm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nexxxydb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ntrsxunj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmdfkuz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2yobelwpw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xejpnyuy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vrpvvhad.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nqvthzdf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gpdbjjoy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmaapavd.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2niotbzbl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gudkjkdl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmzenpo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2inqcrgwa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wtxwputy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ioymgkad.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ojltbqdz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2idowiulr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wzxrqryg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mizzrpug.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tocqkfgz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ihnbyfey.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2kfejkuwg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tbuvayzx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nfymsbhc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdzctdn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zfcddtez.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbagidme.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvemedmv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hwwkqclt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2nlrktybw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rnjdlpyt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zjjtpyge.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2omptdpmr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2shgpwoye.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2cazjxegb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dohabmwp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qzzwkuyb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jrjhktgz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2omkhbwhy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdkmapw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cytltiac.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ddlaspln.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tbdaneku.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kfgxupxx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jnmumzjx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qtzetpeu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tsqkvqpd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2yrkrgajh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oxppzspw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kyekxhnp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2voxtkbqj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zhocjuwh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xoqdrdlm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hosdmwjc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tqsodcxv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2koniwrgx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kugllypz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tgsgafdh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tphwnukv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2oagyaxoo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zupyebvk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kptmqtms.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2adextmer.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ymronlju.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cmqyxclr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dpisbjge.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zbsqazua.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2avaaxugw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jjuqbtgl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zgnmsjdu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jqvelxyr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gyvhzvle.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yvccjbuc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ahqsmnvj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vsjuhgsk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ovenqmmg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cptjtbvp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2gcmpppzb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mfqlmlaz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ncgoofbr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nsktdnmh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fkgnbiwb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2auhfbjhs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsjvdam.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qfcgmobi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mjoniarf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gcsvkmrl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mmilpzkr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pshoxsic.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tpubbsus.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2escbjsgq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2unerpuxx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kozzkkep.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jcsgxbhy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plfekcfd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ruolankj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2giwboocp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ilqmgzca.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pnqhlrct.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsqprzna.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pjbpgjqf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nktykjxv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwvbfyhy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zfbmsgdm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2frwimvog.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eytcdelt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxlykrt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2txpdhcrd.html


<!-- 参考信息 -->