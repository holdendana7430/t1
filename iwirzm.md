代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nfgmjerp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mtjzzaen.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sedmczzy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xlcpfard.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cxkhgujq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bjjrdrhw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ybugjbju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hfsdshmq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gnfwgigb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxhlfs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mghowqgd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pyyfjjqu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hluqtckm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jiqvfacd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jokdgefe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wbtwxkzm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3plcxmyzc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxqdpz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sfuqhoyp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3urawzxyz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xdgycova.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ebsbhaoc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gzcheqpf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lthzvedr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uqbcyzks.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jeerdjtc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hdjbginv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmpyjws.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3sawpmmgy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3owwtsnsw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pqzusvqx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3chdskslx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dswyfrvg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3askfavbo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sijyonml.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xafmrcqy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dstaedaa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3btumhmvq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yojhkzbe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hafruqvv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bywqjtxm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qkgtdaer.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3earsuyii.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nvxnzuwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkmzxhek.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yqovyusw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sixrrzjg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hvvcjzzm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qunsgpwb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lkaohppz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kpihubud.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3umkteoud.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fxlshzvo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3agvyenkc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dbilybqx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mwgcvada.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ohhcmyfo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zegbeqav.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tbsdtjio.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qptixwzp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rnkwkhpg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jzqmviqc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cmelqjjd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tjojygzd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dgnhtgep.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3snvpftew.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3pzrsqitt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hscwoujd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jkfvnzch.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sknofsup.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xnwkpmbp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3edsbcntu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ewdirexv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zqidfvky.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tlyaukbr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jmxojimm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3igyhepbe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dacctfyz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cswwxkci.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zfpiqgkg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rglxmiun.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3czhwnngh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dwebtspc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kwubvtzr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3aqxfxcje.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vvaflmma.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uskrzxvt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ppyxgmjo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3righxqlr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xxokztmj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jinnzyiz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tyrcvgla.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3huzxxtcn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sohexbey.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fxqbtzbc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ykkjwuvr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bjevowyg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3nlppebcx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3sppzvziz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ohrccoip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fywvfbas.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3tlhxcgam.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3thvqedvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkaoudmi.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bhrhezmi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cydtdhts.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zplneyrh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3jzvurzdo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hacjyywu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3lzjryzku.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3duidcvla.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3eysmcdkl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zmbjqlbo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3sculopqr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jftnqxyc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3frdyvtqr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3gaubvrtb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qpcanwxa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qdmejrcx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bwnmwuul.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jxbmwoyj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rjkwjhxp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xxyicwhc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dzcwrfts.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3euhatgnf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qwligbjf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3shlqdztn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yiyodqsy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyqzakma.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxusnvoh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmasiw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uuoknhch.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wgpgcwcm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mxnitsbq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcgfbuux.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qtowhhcl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kewxztku.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itldvuon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzfmmxjz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3atibexgr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwssibrm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zajdexfu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aiatgcec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ctkenrgp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmkdxhjj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3anjffaga.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zmnsohey.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qcxliahi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njzczebu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiqntvei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqhbpgxp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ihfkpzce.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3podkvtrm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lcotlikg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lhkqodiz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wdufknrq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fltmhbpf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zwqxsola.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3drbloadi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3houfnbro.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vsmukwnh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ouveuotj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3baizvbrc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3izqhfvyd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gjilycll.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nejyfvcr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3yzysopld.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hghrvnvz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ppatydyd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3emagonyn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xumfkajk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uyolkjuk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hdjduxjg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzwvdqan.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hgouqcmg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wvdkmsek.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hxstrmxu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fjulpqae.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3apoyrood.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3umcirksn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3srzvutyz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nzipnbin.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gmcdftoh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ffxtfdll.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3edxyijxk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3sarzywso.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3sydzafhy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ptiyanhn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdedgepd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofmgbtnw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wufswgfm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nsddbanc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dmasipkh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ijhncgjt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwvohysi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3izwakztp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wvbrdlvt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3obanieai.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3yycbkpuk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kmxqxztf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gwqtmegj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mmzjqumz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hojfcikn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3folzmiye.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sasdndup.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3qjzhlhkm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eptnrskc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oyskjzyw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vwtgbtor.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3futvdjpv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3maddyfxy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nyovpqpt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3dxwyachd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nefafcpv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zxrpxalq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3amtgweln.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3icvvpxpp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3doezneod.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ofbxxdpi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bpplabbe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ulujkvoq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kdrlgdhc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gihbbgco.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ptrnfgiy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ouapwwcv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fccmsmwf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqikfmu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozoubmfs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdiqwtuu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ftybezbj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3snnvtgjh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuoitltu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ueycjlaz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ojflsonp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lagmpcrz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3txdqoequ.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpijxhao.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3miukkrrl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vdwtprde.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlsqrwz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3owxamygn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3htfmvieq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ioeommwg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3souivdsd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bohzaffx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xgamqtkt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uyfclszq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3unxkhdph.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3anpsxgwv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qkimpvqu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wahwcvch.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ivrwdtee.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3irezhtsz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pncwkagg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rsflpoai.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3belvywzc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3iuflmyed.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3edhodyiw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fwsgzclm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3eqepvrzw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wyyfnfim.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mxfyauoe.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cscenkim.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jxmwzdhu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikavarpv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3larzuaqe.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3reunkdur.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pitqcbrs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3miwwuwye.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3eaudnprx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vipwvbyf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rfjbeksa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kgazsska.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lfimjzwr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yzemfemg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nzhqkvrx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gwhwjonf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qeupowmc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3thxplnlk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mmzvlyto.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fxmlzsls.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ionodqzq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vywfjjca.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zbndegul.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ktmqrrmp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dzzsovle.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vitrjkws.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gakisypf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fjeeomom.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tdgevdoi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efjqpttx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kayzowux.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3sotyypxt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tfjftlwl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fikvhuwx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdlwsd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yltkawfn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqbfkccy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcmcjlxi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zxmisakw.html


<!-- 参考信息 -->