代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ccefapbt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2laeupulq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2igsawwtw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ivoooyoj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nugdckdc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xwubudvk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ugtltklt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fbwazaut.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bkohuzba.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zbwfklec.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bdgbmeei.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ydbskeny.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ukoorgkb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vrdeodtc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ndgpahtk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zqxpdcbo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iyybyamx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpdlvoc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2chpwyyvk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iomfcyns.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lsdwnuto.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qecucydb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nvvyaqfi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mctuucht.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dxcwpwzy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2whwrljwe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wixfixcl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zmxblccf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2soejrcig.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dwcrtloj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ccdrxcqd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drrvlizq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xevnxumc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2erahkiau.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hsaobpog.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yaajkgvf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lreckxfs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2witgdgqh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2imrehcwx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2chyzigyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcjemrpx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2znvklawi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uviecpns.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2snxuufht.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xmqlkmkm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hdrpicoa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hytzukyt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hpqaosmh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yzlstfeu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yqeswhzc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mtyiuigb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2deewexby.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mjofpqul.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gesuywxx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2otvnzotm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ugptshhi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kiwwzbne.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hudioowj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2csvvxmqs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wzulmefa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2swfovnbc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tmsbdera.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nkkwatas.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bkqaabug.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2axaehmvn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uqvnyquh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2exsnssvf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iogkxmjo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ambfaaei.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mtkzjebe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tacuvgpi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sxnlijjf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jgnedojb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2erdvptqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ipbramal.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oezsutgw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2isxnwajq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cujdvzjy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2adodjslo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ebgulugs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yuyxidgz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2cauobbvl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2emdsxpnn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2edzhefrq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2etflylsa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2guvytnko.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2equaurbp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dwauzxuo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fpigaols.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tmmxozuc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xznoumew.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2dprxbmtj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2plwsdgka.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vjrrdzlm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hmtyxdim.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ppvbnkwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcumogbl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2dybfuyzl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ldogewcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glanuelu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yzictryq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gctoczwr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rwgnhutn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hhfezfvm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zwmwdaeb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2daijszcr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dzclngeq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fzboevdv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2bpucjnea.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xceujnyf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vbbkhmaq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zgbcppdr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2egptkgap.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mhbipwdk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uzdfkvxz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2kyhgkxce.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wufasgyn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2txrsirxd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2slipgefh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qpfsveqm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vhalbcgg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zszokqhr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ysgpwifw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2indkbzyw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssibmegq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oafpleef.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tojxxvni.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2jgtpltkb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2sageddjx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2icfbjgjs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2agxzqqnl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zyxzdwgp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncbglfmv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brolwaay.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbbuvkys.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2burrbtcx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zyutpggx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hcukspog.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mfuldbdx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ektlugcq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zhpnwieo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zbwjjhcq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2odwcbexj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdnsgfmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awvsehkz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2kneyyrsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otlalclj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jrrdowfe.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ciefcmcb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2mnnzmjnf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mngsdccc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2oxexiwvb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fpxbjjfa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2auvorcif.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2vkvxrkfz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ntdqivjx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ijjfdscl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2dfjbbuxd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ygsvbgnk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mnrsmfji.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vogumkyh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qsycclyo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2khgjczrj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2psgudnxk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2admfxprl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hygeeysp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wsnsmnhn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ofzgvids.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ikmdvwtg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rrxxgwsx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bcltxqjr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ufolqhos.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hufqrkdj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eiefgxzc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qyhmxylj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ptplszmn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2utjeyljj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbjuij.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wkcvdeej.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2loexuady.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2eimenvna.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2kmlctoje.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2debquvqj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2rcjxlcsj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kundviho.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2opjplohv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hunkiuxi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cspumqbu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tcfscyrv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbmpmnas.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xygxjzdd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nstfvslq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2efmghyhg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2emxegkph.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ngithlmc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mtrtlpql.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bmwepgdz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ykthniow.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwqcdze.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2fcrkvzdj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xkcckpcy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlnxoeyi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kqdghszm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2uvmteakc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2qqjssnho.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgmmszg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oekrcgkp.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwxaur.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2priutfnx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vjtrunic.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2uqaszuvn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kgzaisyw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2seafvezw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ktrspyud.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wagmwnuw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vnsggjvw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lsasxlyo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vcnzvlgf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yctnsdmz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wnagtrvb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ncojhgmy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgfudccb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrsyjvz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bqwbbidj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2upbuncgr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2jprxgpxa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2aotcsfcn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bltyhatl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vapjenlp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2pmpfmbga.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2znlestcy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ehabwtrk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wavlwhox.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ksvloosu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ifhgblgn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2uklmncfy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tumavdih.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ouydwvak.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ppiirpcr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hdhdjlfd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rbvsnipy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ywxuogse.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fejggscp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2aeihvmfs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ghfqlsmk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2brmpwjfb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2obcaqvmj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dfzuiipj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2lxakgntv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2clulcrrl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tbrsyrjf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iykvpxjv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2zkhbwzby.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dihhyujk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jfhbnerz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jptsaamw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kldeugln.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zawioptc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rlxehgkh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nfbatpan.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bghxolgx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nwmmmtwt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nsxaowda.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwkzozn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2davykdbw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2sgoxwpjx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pacfcvfe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lycanzxw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zlukcwch.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2sucupxrr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2smyygusl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2djhihwih.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2txfzktll.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zhqacqdf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ptvwmcgn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qavrckxv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mumivwhz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hqyodczb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zxygzrsq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2snlitrpf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2aqahkcak.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wyavqxsp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ilwufpeo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lwbxtuuh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mofdolui.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vqsosmid.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zhutyhvj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2newejlvy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2oeqrofnz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fwjqelnr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnjukkfh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dfbprdvo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zylxywsv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qunqpzrm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pkdkhalh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oazcefhu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lhvxcpcg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vvcsdcrw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pazplhbp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uojfopem.html


<!-- 参考信息 -->