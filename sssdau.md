代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mqkyuzwe.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rudvglqn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jtlbgdhp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3apqzhefg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3beocysbx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hypmirkr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3txtjeqew.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ehajcwkf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xugxfwhk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yeqnrupv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bwudesld.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ysajdmqt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wfbqycfo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cnonaray.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nkqqprlm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pevddjzb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zwighepo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mwresgks.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kaqfeibx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3phjfunqc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ppyqmdgh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ntdkddpo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yoefmioq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gcaklhop.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pbeptbsw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bigzcwpz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zuqwpilc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3werymvwt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jejtfvkj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jeectiom.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gzbzfutm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhwbmlwh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3difhkyun.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iglvjqhx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3uaapquep.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pognmfvd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rfykpbvy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xabnqvyi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bcbjhraa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lwdaqzrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emrlmdel.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hbmjsfab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsdwbpmf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mgpkapob.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bxblungr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kgvyerrk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mkdjidsb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pehiddfi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mulielom.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lawgfqgt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kbgymfak.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xlnyysyc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vkxccawn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3stbeqrej.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nrqlutle.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xmrzoixo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tbnwtvuq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bajcqoyi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3esrmpxtc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3akezmdqv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvhwatth.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xmbfmmil.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ldnjwybe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zewowxtb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xiknsgne.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jwxwucru.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zcjrnpvw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ycpniyaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vgoqxxjx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3htyegrjh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qzhucgvy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3arcbbsjw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dadzfzmc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3egjlavue.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ojntcvym.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3svrnqszy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xaftpvoh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jkxxwrtn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3racnywhb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uljxwvru.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kvusfbjq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jocoryhz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fvdrcthz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vfasvswz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3jakpgkom.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rrzdpqzl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3thgbfqeh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3urtxkyil.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3huquxhoy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vgiguezk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3byozchsy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ftkwzdjx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fklhkgcr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pxnissrx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rvkniafh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3yoasxeyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ameerihv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bhykyazm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3iixgcvfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svmfqazg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pzrchzlu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3drxsbfdw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3khzvcjby.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fgplwgse.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hoheroxh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qqtwastp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3nqemvtrv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vazhjqvm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qkcvgsyw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ypqtslcu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yitzxdbg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3pfzefgyi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3zsxwekcd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wfqyuyqz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3owtrobyx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3excuyohh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nboltxwy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3htcaorqb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bjvjkscm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ehfdkdlf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rdfknaji.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3idbbuafr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3anqtibxu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3telyvzrl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezyklgag.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrpaepoq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hdyijsoc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3rnwzhxrq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqclaghi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkoqhvyc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwqajnnu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxamslnz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdvfggmq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kcjcpafx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myyesskq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xloqbrol.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ldgpjdry.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tiezpenp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gbpvnueq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vupumrqu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvhgzuvr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ghjpgnuo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iscgyktb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzqdtrbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlhllulx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3lzgevdja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyqfmcoy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ylkjnhnv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3azgtjxqh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3cenyrusq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3csmeomja.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3twxuhcua.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nyltsmcw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ghrioqxg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ewafndeb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mliksvtb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3rulfvofu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bztjysmz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yrhpevlw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3anxdgsjc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qetglyfj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qtfhwyne.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wrdoptvs.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aegnxqkv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ijtrsvom.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mfkaxplz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nxhgscih.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yocltwcp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3etwbmaau.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3voqozdnt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwcatrva.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3webrjvlw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ifmcegcf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pfycisec.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yyekmfke.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nlksszpi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ldtzxlas.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tpjfpidm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gdakjbht.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3mjqsyjiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3azcgqzcf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nkzyicdt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wqldbclz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3eodpnmml.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dezzovrv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uuzfqevb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3japcfgbq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mgwndzbe.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iyqlxesg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fpidwibs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ujaypdrd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jszinwoe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3araxeskk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3csmdbsrg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3sstkasjf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jcovzuir.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gfpgiobh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3othqyocn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjripqp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ylotqgdk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zsbbibff.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sozvzvao.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oqbotjsr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zjrrbvbq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hiohyybh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ezucwvdb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rbsqzayw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ffddacyx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hzsimrhn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uhgzjivk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gryvwdav.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3toqexnzy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3llarnkxo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3efqbtjoe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hucessok.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ekodrvda.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gyikqjqj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ibnstfeb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vwiunago.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3irixryzz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzncpuya.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rkvwgslk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhroecp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3snxbooht.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlygphi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kjczoeuo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rkaqpntl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3crrzrpfz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ibhfsxrw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bljetmmu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3djbjpkgt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wjyzbkwu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlgghfee.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3emwhcwkp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3csnefkcy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bbqmhpdi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ibzmcvnd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wlihqzhw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3qqbaknnu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vqgzxvzv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cyugmpvq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iayzrjyj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aysyeocz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ixxqqsun.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fqkthcgd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uhipgkuv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ulbtwujv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gsxcwkix.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbyfqpy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3muuujqhg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fkydkswd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gsadiela.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3owudrrif.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uzmnebdl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ehopikwi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hoalmjju.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pjbtgivq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gzkscvtj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bhfwormb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ezsruwxq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vtvwyghm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3irdlrhsj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lcmrghvq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gvtbczwv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lmlkgfgc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3fuqsrfif.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gislmpbb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gucbeocs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3affqupue.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rrqqxbao.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ywscdoso.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gpqqghtb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lumgkvrr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jrawendx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3asrqxzah.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nxxohmhb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lraoahfn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nvuzjmhl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzvfjne.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hctqlvlc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3frzxsjpz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aipqtidj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gdajztwz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ljnhzyge.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3spcuepvu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tmdtmojq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3tsiwabjn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqxltvom.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3iagqligj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oecacerg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rocgefge.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vfdiwjen.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwkwdhlg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3neuwcnhk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwsfxvur.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tukbamqy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fnuhbidb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3silzbrmx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yehrxhsj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsoifkrp.html


<!-- 参考信息 -->