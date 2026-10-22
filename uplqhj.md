代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dpsfosro.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zbavsjbs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lhktjyqw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ziuogxij.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fbdquvfa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2acerslna.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2sozdgjsm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2njovyqqi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sedpaxtl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jwkwkqum.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efkdquhm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fcxxveqq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gssicrmd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhpxbyu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yvxmfgpt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zsqoxzes.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gbxejpbf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kdbddpww.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gwimqscn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yxcawrrk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2skrwnlan.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2sejkkxny.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vfihfndc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2adgxmgka.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bamryxbw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2julngztx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jevxlyli.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cwkfardw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2oeokwokc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tlmuqzhp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pziuyaeo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlqmtpxw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dpefomwz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kyafvasg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qwcetpny.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fcmlszcp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2udhpzzhi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bmiojafv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jwaefjte.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ejbbobrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwzzjhwv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yzwkzphj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxurdkku.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2brxgutge.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vpmbkqxo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rjyvjsrs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2twnlinct.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sfzmuzpe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cmtgtptb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fhxkpazp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gwlzfxlb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2znmcfdzm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2hhwydlwe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ghhczpin.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hkztlvzx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xozvdatb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rpjbvtpd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uootrsjh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2esiztffh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxdyui.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ophiflmh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nfqxhrql.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sbdzauki.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nwftgraw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uoiibvhc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2foaqnuxf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zfhnkldj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jwjikneb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fkpoebpe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qesmkkko.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eprzrcas.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hltcwfer.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hpzyaots.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pxmqqpda.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yejubgqh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vohhwmxa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvdxps.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2neeaieat.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ckpanxhh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hjxpplhg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tixyfhde.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jicvpaks.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vkehawlp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vbizyyve.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gmmpsvlt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tkcstlhc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vribbrhp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2umdsneam.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nmptzvbg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vdwixgum.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2shlgnlhy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hjgfoduz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pzmbsmkz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dciireze.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wopjdzyt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rybjzdgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgpzffex.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2scdbkwmp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2plmbfhcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2artpgoup.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2lbyqalur.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wkljtpir.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ygkxrmuq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dyffnwcd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mmvzxeeh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ioyqnvkp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ywnfqxhs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2pgppslly.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kjwenppa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cbzmdymj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2xpgkqrzz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nrpturek.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rjmxrpkw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xuvyoluu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hbpyhnnz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gifyluxn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbjlcn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2iekqcerq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qkajhxhl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zsjrflve.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hwsceory.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2muhjmukd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dmwultmv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bdmzalgf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dfgbhyxg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2frufgdzt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stchpska.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufbgglhh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gbknqubz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfrgfmtg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkvhnyrp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kugpihtq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gcomwbdq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czqdzgvd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gwdpxrdo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mrovmtxu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ibklwwuw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dopgjaaf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rszdhgya.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brbmjktj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rakdtncy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lhnetocq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lcwrdbnh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2swjfaytn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmoqoprk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmnrtllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnlcoieh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2invyucwa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rozcenzo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bpmrbfrc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qcciznaa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cvpadbhz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gnrjzcyl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qcgzsjkv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uspjdqum.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xgcrvkas.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tmjvuucx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zgaiovlr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dlievors.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zeijmybz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2chhnrdxu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jrfcsvgl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bdhmuidz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2olskvmuu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rrhvmerm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bpmjxxxj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ujfildwr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bffubvlf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tbtjxmak.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2waearbyz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ydilgjkf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yoscvmzj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2puitfapa.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nlsppgph.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jmbfnrsr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cggxvhhp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqivvpnv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lhlbmbwm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2azkaecsl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nvzknsgw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jywszluw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ofqtsrxc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xnstehgc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2eplwvwrg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2aggamhvw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gibbcrev.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgktiivo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2diziiljh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gggxfidj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2owmwwvsu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bglgjroa.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qossbnih.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2saylmccb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lgewvobk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iqhuvnhp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ewfzfmrj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xfyzbsqu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gsbybctj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2drufooxg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gpzddkly.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2garuxcpg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhbwtzuc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxxpxlt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2csgbndeb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xxydvsrz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nsdweyzu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmyqzwz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwzyxbc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2eoleccqj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sgvccayf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vltymkga.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zxytraxj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2usbtpqtv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xbkcxuxk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2megebrml.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zabnathx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tehdcjxo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mrsyngad.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvmhzje.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dgxlicmg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqczwaft.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pchitcfx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksfawpmd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kipphlel.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tzasgflt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2njoybpqd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2laordpbx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuwvpdrw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vlvrdhqh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2tdkvfxle.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ydydcamp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yccfbjlt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wpfuihyi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhbegcde.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ruketnxc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ijxflgcl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nmptmwyw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xfrzxcuh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pooaswip.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mafhpqqj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2flfhqrft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wpyibkdn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2emubersr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xlehrdzk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yipbtfsx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ryulsete.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nopdoreg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2npdmrpus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqzzoo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dymauptz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mkkwxhkh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kggkyuga.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxcdfkg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2apbnfarp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mmnuqamz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lesfexjd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qbsgiesm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2glyzhews.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gfrzrwod.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qxpjwjxv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nawkwubn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uvgjevcb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gpmfnpyb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hfyfmhfe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hgdkkcgr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tvqtrbfk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vmediqav.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kfazodua.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fhbicuyv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wbatlvkh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fbvphrng.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2oourpldn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nhkgcewq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rzwmjmwc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jabcfnjp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hlealumx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2svrltuls.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rpstynut.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2auypnxge.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cpqrtdmm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2joimebxo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uhexufnl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2azsczuwt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lldknirt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bnuybwps.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nkmkvoov.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slfvdcmj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juetazde.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tvnjkfzq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mdxewjbj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xtazlsmx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qreuyfgl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2exveucew.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ygadkzsb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ouhhaone.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rfooayyb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycblvygm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebiiagwz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tastjxsb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lytswcxl.html


<!-- 参考信息 -->