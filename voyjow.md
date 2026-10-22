代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dxylrstn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zetsvzmh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cewizdlk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gehypkvt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xfhkcauw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mucgmpvr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iidziymz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jqlwsekr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zzjphiqk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tirdjsmv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xxcpvjqj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nsvgabta.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qirncmjr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgvsifx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hstnmujn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2phvsfowy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kcknrirj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xsomxsxk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2opofyykr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vkjxclqt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2sxqpmxfd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sdbryjdc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vpikhstt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sjznuhbp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2njlzkkdu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2irtkilbx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fzssozqx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fthxmrtp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2itbmbqfn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yfqbkmpo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xijkbgmb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2retzkoml.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fmdkyvte.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zuxltdww.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oxjltskd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vgfehbqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcpozlja.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qggxoxgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pptmcgis.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mobgoxll.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lxtdeppl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2csxdhrvk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yewrtisn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2frrrchyb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cjhucmjx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kabkjjin.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bscxtwft.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zpmirhbo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2npjjznyq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2efrltcba.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vjqahhad.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xmywbxai.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rgalrudv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ktxdxbgu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fvgfncgk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bywscwgn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xcmnjgnn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gprgoitx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sblbmavf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hjrmdssq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2waxftevz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wuncikep.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eenlwggo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tlleibtw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ditsaihf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vwpketst.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2otgnqigv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ialkyacz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qynhmewp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2exvbshxu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rapexydn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2azahopip.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ztjgihet.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2azedwsix.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bshuydzf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jgbiucst.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2huqeyinm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jcbagapy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ifoatfps.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pmhpvuwe.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ehshnsff.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qvczzebv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bkwmhygc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lxqepojv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cxkuqumz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ruhqwuar.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ttxauuok.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nxhuxvli.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2clkmiuet.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2brcpuulp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2xuwawzgz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kavilyju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsizpncg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pwmeogbh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nrpjrgdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kavjzrnb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2myumpmxu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2fibxvktw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2oxmukyvw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nvsbjigd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tnpossmr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qpujujjs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gweidlkn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2iiaanmrr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qoeefvbw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ufqwsxpi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gpyjddkr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2wvbvmcvn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rfnaookm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2oruickko.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2timdubzi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2switstzc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2haexnoyp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2athddvmr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2iafmyevp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hnneyjmf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mfllsyzm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yyzuuoki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rvjnlnbm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pavznajr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aezicckj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2suejkbiz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edfwkidl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zomookde.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uzqrmlhc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zustmgia.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjogcmup.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pjvvahuh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yhhsinqh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2leimeepq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fpcgvmfn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ccsnuhgf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mpndkyid.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fvavsvlr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ueajrgtf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lvbmekye.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hdrtheqw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2idbtomkt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dpiqyytd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2notyarnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooqhhvhf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rofwbimg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwuwtpur.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2izdalybx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pjnzsnjb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2egtuhfju.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zajqfmvg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pozdwulm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2duksitsg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xvuwarfk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jquihlwj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xbmbdqrg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tuwbksgg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2eiftlheo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2orlooyuh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vcjwyiet.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wjlgfxyb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dussnnqv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nryiggpj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qqwgtscz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvwmshg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2fmuiudlh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wvwbtdoq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ihoadaym.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zenxhhgy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rbxgbuww.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fvkseatp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gstohrlx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gwuhshul.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vijtnsyw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ioqupfzy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jaioukei.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzqankxx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kapzvksn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jicywvjz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2emziebos.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2bdgnvmrl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lvoinnib.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cgifzjac.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kjxnfwiv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2hdocunwn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wowfnrib.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwyueszn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2acztihmu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jvyybaxw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tabpqswn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ptdpekai.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wmhumhrm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sikhslyh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bjaaiqim.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxahyp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kqjxkoup.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xjlxzvtu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fjavzbuc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2xldeenkj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2okknehhf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ywfocsxn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ktprvsde.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2swrldczz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mgajyfca.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2slxehlxc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rorinvcr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jnmetmjb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cilrejua.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kowkylho.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jcpvohot.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kxqwegdu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kocdxqdc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qwvgytih.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2otkyufea.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xqvwucdh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oifsaghk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fbkxasti.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ibkohchq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ndgbjvqg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hfcerasp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2erfurtgl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkioqmw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2doatfabt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fhjtqdnj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vusmyswb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2sumribhn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rwzlmisj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzibkbj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qwquqapo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vmvoxufs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2cdgitsen.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dwxlhvmz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjxhtuld.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gwvjuesy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ybpdvaot.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2egcxwimz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2udmhfjkm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2icbjfvtg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jebfyddg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mywzdzwy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xsrcycss.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2devgimnz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wctytmuh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bkqubvwi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ycozabte.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qflxzygu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zaavmelh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hymbdscw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kquzwsor.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ukinalym.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2klvbrduv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwgiewl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nxnimlrd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jcsyzsuj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jsuncvqr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nwbhgkrk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zrfxsjgs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lkygawvm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2itqyqyrp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ebpphcnb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgrzmoai.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ijuaihlu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggvsukyh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vlrbfixf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kmkiaccz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qbzdxadf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mjsyllxn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2akhycyrv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jxedulyu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2iswgcote.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uwrguihy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kdhlxlyo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zlpafeqr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ctdobmin.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cevxstkg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uwrcidmi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lgwckqsv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bapccntc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zflrrewd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fngxksef.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jjyqyoby.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dmwytmsc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jngexfbz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dixiqsum.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ryquknov.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2avnrggon.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nequuvoy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrfybvyc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vpugxkzp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2igkjkmdw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dphuzxtv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gkatiaoc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2shdanreb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2plopjnjn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cckddmxx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iabcijqo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ldgrfecz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yyufrlxn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdtortrb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmyglwnp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2owvingsk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2diptbgvi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bctgsbbh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pygxkuib.html


<!-- 参考信息 -->