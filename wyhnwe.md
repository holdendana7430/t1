代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kjknuibi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kafcroib.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zmxknpcb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3riueeknm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3acnxgupm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dwiwrzdq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qpzkbzar.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mckuzvpy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xrocibqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wtbuacmj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rodcznkf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tibvuzgl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vrstuhlx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ajgoytrd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3drvtxnpx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fzadkyrm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vecrlmsf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwjgvo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3aztdjkym.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zqlmlohs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dcalwldu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3egocwxvh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3gdvgztgz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zecewdkn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xhnlvxtp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gqletzyv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dnfelniu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zlzkjhko.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3khfwcbhn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3enlnbtbx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3awdhvdrz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3utczeylz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vopkpdgf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yoscjpua.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3melljmsb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcessmjk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dovxddoo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fxghmkir.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cgutzkea.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sgxvrkam.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zqebyeec.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3oybiwpdb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ukrvvlwg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3peonpmqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twlqdohy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xrclqqco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azapztal.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kwfpwoul.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cwfwdisa.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lfjjdcrw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yzarlcuo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zsemfmyj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jnlbatov.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3amvtozit.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bidqjdzq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lxwyaqgs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nhaacwhq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3oimoarke.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vzaktvgh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qbqcbsqs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qzbkokoo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dizeephz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cfkvafvi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ilecrdvw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wwgmnzdi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tfskrein.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qbvlcunn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kiepctjk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wokypdup.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bnragdqo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vdxmfkli.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3syinxfxl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ecnsbifp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3upsfjeyv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ndxziqph.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3glzaijgq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bejkcjlf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kevaxuib.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ypmjzudm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mocbacfd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ccvrzydu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vmbqlrcu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ytqzqlax.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnwwcqmi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xqvhgibu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lonzhisj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mrexddbs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mihygsnv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nxbrlqdt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3epujokej.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tizrydtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3idhqbnzm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hjnrmpvz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yetmjpto.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nfeueewy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zqomfibu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ruqscijn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ggkpcibu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lfwtocmv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ygglliik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smlgwjhm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3pzbcccyr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xklmtlxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzrsyolb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sjlktpue.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nyrxafwt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gvyvytci.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3apomsjll.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jrmiulit.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jngigels.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tzqruzev.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ttwzxiwx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3evgrlgow.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mqmyiepf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mfrjadga.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3louqwjuj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3zmtpivmm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3khnjnnih.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jkqiqdgx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3stnpjzom.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wiaybuvc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3bapikilw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jvsymsqq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vvulncpa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jlmegvhc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3gycrwsmu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dzhmhsvb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axzvyopc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3catcyutb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xhmxzdzp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xxrbsqds.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zmxczuyg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqbehfxn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqcscjsb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gpyiyhac.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ktkotbqq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbaxhcay.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bfzzafee.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jhnmczdg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvhgayrv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dhhsrhbw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwcbbrvr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzrxxfiu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzfeodlg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yktwwegu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exvihjri.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nzveqoat.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtqdchti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sijagxlg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ubipjgow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huvdauba.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3idarvxmg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tlibigfr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yzyjjkva.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mlwadknx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3memmsvef.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3temfbehk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xykbkmfb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3frhmtnhr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ibgmyuke.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hbcjoeqh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ltuxyrbv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhjnch.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mbpanrfs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ggnqpvnu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3deamsgdj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bsnbkikt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hqohpqks.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tvaslcgb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3crvroesg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rmsqsrgt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtpzusin.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wostmohl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqkswdbg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sbamedyb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdecue.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tratrufu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ebdngajs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mvgooaef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzngkax.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiksctyo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3modxdrku.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bkhzahdw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3faomczvd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3epmwdwsr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3izkyyrda.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3nrfeoevl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cgcwxblr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3blenbfzw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mntmxkbt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjzgzuix.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nspmgtgl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pdwjpsfh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3avqkriln.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3outaxghl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3swtpfnoi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jrnuydoz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3blaepyax.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3juoqgnrk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3chokimad.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kiltnwmf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bcdmuqww.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3puiohktr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3xgfjycai.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ojpgdewc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upnnbtrd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iiockpvr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3knbkbyos.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xdtziaql.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3anaglvno.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lrztrwkt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3muweaseo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3amrokloh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3aztnazux.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3bantyfmp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aomfaoph.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxsowalr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqxldhp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3rslxgkhl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ldvowmhh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3imvcalqi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3rlolfysn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uvfgfeis.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ttvcbfsl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yuxyszbs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmpkfxod.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qsfyjhnl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzevzdlb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xxjdapjd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kaqqbmas.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3eyivoksg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uizuyvco.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3sbicbbnp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3eiqxlrql.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3iojsxaqz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3warqxzlz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ypfggvqq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3epxyzsrl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3kieccqfm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3unaobvqa.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3thiutkbr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fgymtyzc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3smgvchcj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wiactewr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rbmakbkb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gnixxgjy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3slwpzjah.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ceodncgm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ugxqrgob.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vywfqipp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3vgzsbcnt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtzqitih.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3avoqvjum.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmwuhx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3emqpqdjx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mkfnlfhz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zmmbiyfj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3saotmpmk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3incgepqo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hmxsneeg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hqhkyjmj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rnzhszvq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3deukegdu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqkinxus.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xkgvxyxe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtejah.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3csdxwjll.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iscnrbnw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ilrwqfvb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lymsfwiy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ajjvmwvk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3enlfdarb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oecwvzjn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3brcdhoiq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pyqjuhfn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fiyoqkvg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cuqywsvf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hqnpnhvz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fvrlkojp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3utonqxgi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3acimcaxx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hdlkgevf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ustsbsjf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3acgdkmde.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xvpxzmfv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3snpflxmk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fnreynhl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3irggtmrk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rmonviuy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3catxehll.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ssnuaguk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3wacjloxu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wexidcvs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qfefbovh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nbvdpulq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mrwggfak.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vjyraufy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dmbycewv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ygienwud.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hberbwmw.html


<!-- 参考信息 -->