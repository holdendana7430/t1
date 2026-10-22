代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2szoizwde.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lhvzmktk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2upgemjzv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dolabufr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xhnuakqh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxullp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jmjwlgfa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bygvqphs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jjkpqaib.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjopgkh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yrpusrqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uhwwinkq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fbhgdhpq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dirdhgmv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpxjxrlk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xtxzyupx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jlaotzqz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ubhxeizn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2satybwlb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zahgbuqz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfwpvtwu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ronbaqoc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2fspmrhvf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lopnduwx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2octsjvmw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qcbltnyu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rrlflnbt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gazyyhfo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xsrnijca.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxwgredz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dymeqyuu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qqurhtza.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xdweafqh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cdtgghxg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2egzdrybm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ltkdopyx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cunxddec.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2klcxwxfg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wfkrflgf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2icqdtcfu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pgsxjmel.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zwcmxbrt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rskecofy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lxfwsdzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bubdgmvo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mccfyldw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icxadmdq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gsdayfie.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ovymcgbf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2yuodhdyn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2djupgxeg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2krggqpeu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nwgdbqoj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2okqroxqj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mhdcubpc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qyswtfpb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2czkkbqgo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jssniqzu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ddbyvnde.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tyzuktyr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qzghtdun.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zqevmdhd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2lmxurhci.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2egmlbhrz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zqelthho.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2awfllwod.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qltpvbyw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xdlykrvc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ghkarnib.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qiyocxlo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mnsnzghm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nvjxablw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mxvhtfkg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2inorcnju.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bruflwau.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ibifwgxl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2knksirqy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mjtspprl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fejfsgqm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2urpinmks.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qgejudlf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ophliqdo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ukwhbzsp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ifrstxtq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zybtzstu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kkxlukdj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fbqavdaw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qcuyisqd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gdiomsnf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2drgydoiw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2enkvynmk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kzoffbqs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2uvhihclw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ciapphur.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2aguyudjm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yrdnpyld.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2brcxwvif.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2oetgegey.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2auwsewcg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bvzrowww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxsboawr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2sajpcqlp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rzktobwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpdprlco.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zftxgswt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jdhnzovc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nlnqetwx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2omiktwyh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gejqqbkh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bdmvwsfa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xmogxvgg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xerlsszt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2iutnzgjf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eouraqwq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2kdfcfigz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwdduo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2khdtpkma.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2gbxaujuy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bnqpbaqy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2atgakwao.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2owxrbrmv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2fykjaglq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2udwhdlpw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2njrflvqr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zhotdbxd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2qyimfjeg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bweeapyu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqbabkrj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aqrsgodn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lenyulow.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2topxargx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2lkkfszby.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2amrqslcz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mdbjdbcq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2slgzcjol.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdtuojrr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2deqwrhno.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dckzlkgn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpdfxfii.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aljwnqsn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxzzzfit.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2znoycuwo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gksuktov.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ucylkvgw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxqfmy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vvltuggd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rwmdxaku.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfqutful.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jchfyqag.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2dvvaadjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtnfajqx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2sahlocno.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2opgzxgmp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2nkyuwmfl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gvnqygfs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2umomymxs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ibcypwxp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2egfomeem.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bbcjmyie.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rwbwxuxs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2bghgekxt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mnumruuh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xquyhruo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ekhgscxm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jetzdvkq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jqqlvdso.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dyxvukir.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rouiphum.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2avkzzoao.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gtrixche.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tsrymyig.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ydhjchpn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dzcrncmo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkuvbzvy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pbxkpkqc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kzwdfiyj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2efqcwgjp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nqtxnxvx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vwfaahqg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2etubqjmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdefrca.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qcepwqeo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zkocagfy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mrkepkrc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hdmqfueo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jxvqowzm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lgvzhkcb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2kmiyexyc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvfxeard.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jfmtuels.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2asymfltn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ayfdefcu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2olflrrwe.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrzpqx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xrxhvfqx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqdietjp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ovqntoue.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjgexes.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ckcxnutp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zhhjsjjb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tjmesusm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bvjmtlqs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2blspuomr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ekjguxcl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gdccrqqx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fecigedh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jsguyjjt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2huwydbcc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2odgeqibg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvmlnfa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kkhyafjx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2apcwtkgn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2irgqfqes.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fzkdwsoj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vjgnnwlq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jziunlqu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ldphqavf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yxbcmxiw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqbpied.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmnmsoi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qeagloxq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yprpetsi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bfhdunhv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bvfuutej.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktkxiaav.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ramoopje.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zscwszzk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2twpeisad.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2baedpqws.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2skapyiqt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2pgntauyd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bogufbmi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uwzlrcqt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bhguhcvy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2quqmtwcw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftqrhfqr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2plvtsgym.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltirbgmc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2uidvsvyj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xuhpqdzi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qsuqhncu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ndrqjxux.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2zoqtayrl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tnnjjckk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ljqqmqmn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivujpzyi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hptpisvb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lvdbffap.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pieyyfsn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iwkvawyt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvcjus.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2plextlfj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gsfeyzoi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gelchpjd.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tfuudzol.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rdziicdd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdnkypp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2lggrntrw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2libejbmp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2mywzxdsx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgrfreqm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pdvetyhf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ludojvyv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2awphkbql.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vadrzkzz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohysvtpv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmwngckk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bzembryx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rwnsdfgy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qcqczuul.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zpwqppij.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qvedrclz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kgjpuymd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2yjjzjrtt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mjltipzl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gtqhwrzf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wrnjrzmp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2itjlluai.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2giysgese.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kgznnfic.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2czodgdof.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mirgysit.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fsovayol.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ubjivcmd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2imkzzogx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ihziafjq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rojyvzbj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2byvzgcji.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2szhwfbyr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mbomqexg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jfhdzuoq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mltcbdwg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lumomyew.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vshyohpt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ovdesvfp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2npxblnnf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2offysjeb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddqjultl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzsxdbkl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lvgaqoht.html


<!-- 参考信息 -->