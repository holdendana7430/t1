代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ycadlpuh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lxdymlvi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ktcofhkl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wxgbgnby.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ujswleio.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oqkptsya.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2srljngtw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bpnrbxug.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kcjxljnk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jcgsdygz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zxsfuigc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qvloyyay.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2acmttkzc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2okwdtnyl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jayfgpgv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2okabwpir.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvccvlxj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiyfjck.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pqqatbfr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2duayxlft.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hgedkkbp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2onfxiska.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2avstwhqu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jgmbmapd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kwsaculk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dsakkueh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vriuazhf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2atgfnxjn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iifvjker.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uiiuqsph.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lirjivzz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2vvafxkbt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wwfduzrv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mhybjkbq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xgnsvpjs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vaiqtlmh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gjezzvqn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mlvolgsz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hjubfvxw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vhwpulgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcbpnioy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2isdioyhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uumylkiu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tqywsnkm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oupterjz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ppsznrhi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2omyagtex.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lcdhrrnu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jzwlkxbq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zlxqxtix.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yvcxmemk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mfivfitf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ndxdsulm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2nlhblyqv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rdkehbod.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ofkhapqs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2shehgivr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2royqncmz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2taydrbkx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vzuljdof.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iivipajo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ficbiylk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dbacsiqn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tnwutxdy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uffvhmtx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zqvocyux.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fildwczq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bnpunwzl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lhdlwxzl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pehdvuyy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dvqipnwv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tdlgkuvr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qmztpidk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2enakbbam.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yzvhvqrp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdqgmboa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zwrgxtqw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jaiahyun.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qqdsjjiz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2psryehpx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wmbdqgev.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bxmoghok.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fwigromm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wnzozrug.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2apjgrtpt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lddsrenb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ywelfvua.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cjvgvoib.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qmvdbvnx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2antqggki.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2odaeegnv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qinpdjlm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ueorxxtf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lhwstcwi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2usjsnilc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hljnjnru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmcdryed.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jnghjwvi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wqkdxhso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzfpxlvb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ighlndno.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nygnzfes.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2vsstuvou.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2vohvfcvg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2klejqgnj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xhocjruj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xehoeemu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nwtjoaur.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hhapwzjp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dcuwcuuo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bmrisfqv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tkaxitse.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxkebt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wlaakwst.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tsewfoqc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2rrxkelvq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2fcztltat.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2funozmex.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mkwncjzo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nlqxccgw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2foulzzkm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2nunfypsn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qrirfzzy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yvrouich.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gevskbsk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yknalkns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wtorapqz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iefkktgk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbdqjxtj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfrarreg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2alacgqog.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2plwdzhet.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whwzelpl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gjoqwhlr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pzgnchko.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gdjfuwpq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdukjqij.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqlhefiz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2anmdcaie.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpkaxtez.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2djsasqth.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wqqrrcze.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ajjrwqce.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulzdlusz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhljiyma.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ghiyjzuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znlivuru.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qjimibla.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hrbuywrh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qknisjhe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hnybnnnd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qthfslqh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ghnxthmi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zzgbauoa.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ekzpuzri.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mbqtdwiw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pjrnnnto.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jevopjfm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ougrylor.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rhhvkrda.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sacgeaud.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uegmggtd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xtbxbsnu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2sfauhkjf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cmkoiahf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ssfouzcj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2srxrvdvw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2keldojct.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aghomyxe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xhuiydib.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpetcitm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pjashlut.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mtonogjm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xntiuocc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bubwteiq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2aemxnzli.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hwcrjnah.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yemnycll.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uqazpsno.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tvxoxdik.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hnipnmyx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrgpzey.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ekwvkewp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2zvrzgeba.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2uiolwioa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwqkmwgh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ueznqrch.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2stdtacnu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hcienock.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gkaqowbb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qavjytuc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hpreakfj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2amlxorpo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gsegwdhs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2unllbnmd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fdbmaykh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2axngzrdt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2efqahymh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sifeqhhj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wthtrwcc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nnvowbgx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rewoqzxw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2opqyfbgn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lhonogxu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jnmckyzv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2npvzngco.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nnjgnhzb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lycmvtvf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xgztovmu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2eovfbbjo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2voxnftwt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tdotvexq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qoxysytk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxjikjr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2cojixzfx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hmykaltk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2juzekkxh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2byhcbgvr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hhecqexa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2scydwdca.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hoahtbsw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhtvzqwm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efngbsdj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiampod.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwobpeah.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2twyebxxi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wwfezcdu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjfjbrl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2eeioftgv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ahudydcn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2rkcbnzuj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2boeiyugs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnomtvil.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2srjuvbpt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rwmfsldi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mptmsune.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xmynecte.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jmouqrmm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2icqpfdct.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcnuaj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jakpesjf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eshruqjr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yeopfqtt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2unmkzdcw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dwzkxcyz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bieudsxy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2qtoapygj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xuibknjb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgddpmu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mizbzcrp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xwbfcujs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zcdyjsjt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnpvayi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2icluxuvz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2puvbkiao.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ahcrnnad.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2whhencjj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rchhzlhb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vcelipts.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vljunjxn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iutsgriw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2swfsasho.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uermyljf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cvlvjgtk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2cpivodac.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qnkwzpbn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zfxczvlf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2osdrghqd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ofazlsup.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2styuzvbm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hrccbvtq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2traapusg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sklilcct.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lbavgrur.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2iomtatza.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2irelquik.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2osrbavyg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uqryqxeh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2besfftjq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gqqfxklo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lvfedzck.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eivktewo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2icbnhlry.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lttdqisk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bifsnzuu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jtcrkfpz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stgyaxeb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2hqzixlwm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fpuncuhm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ituxvaio.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kzmkesed.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bttinoym.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sokekcfq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xgyhhfav.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfkkdiql.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rtgxdwxd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvshgelb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ameohzkr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bciuyqid.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywkmaxms.html


<!-- 参考信息 -->