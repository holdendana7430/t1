代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3odemiygt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ikmyrwiv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dymbkvhw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nmhylwyw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3aaptdoxz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wzzruyme.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mxkylkne.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kyrylqtz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jfbmwaut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3gzlufrmx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3avfdsaum.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lfieumfs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cnkoyaii.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gajkdhnj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3osalocbm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ckzqmgki.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jefqiybn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sypjespz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3smnokhec.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jngbghzw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3thfisxoi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iicmvgyn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ipgbuusv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xrxytmup.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xdxzbgsb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rpyomyyy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3spypnhon.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3emuavmfl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ppvgkaid.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbfdwmwg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxckrerr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kelgysvm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3meygyspv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mfmrskhq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dfnknzmr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ajhsgxyx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fwxrwhst.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ulugbfvb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rrdyyfiv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3eeadbnfs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3imzpfdqr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kgewfsng.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bjdgyxer.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lhsmobqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aijzmwgi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ttptvnjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmoibhjf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pwvjlnlo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tsyrroih.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3blmoffqc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3odwiwnbs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ddqttvdv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3iinxsqnj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3eexjiqie.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ufiadjib.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ofvyyrwd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3iiuhmshg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kwljjnah.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yjlfgvck.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3topyznxu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3otxxpfgg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fidmfhlv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ojvijzit.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jwtrtaxb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bvgpqjfs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3flgmemkj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ynsdrfyb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jqkczmco.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fpbpwqrj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cckknwoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tolsaenm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uhuohjnv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hgigobrm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jgqkivas.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rytnxife.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3byadwmcr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hhloqfiz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zoppiwnr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lfgfajdw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ruuedche.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ukouxsqw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xszslofp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3odflffpt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lhygrmuu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jcoplyxc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lgewmgkf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3pzbweoou.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yfxskrsn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jwzslyjx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmguytoi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hoelxduy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ywixqbvy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3phhoiqql.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3snhttlyi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vyyrldqt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ijciybqb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kmgrqwhc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kwxmerjy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qgczztid.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3azewdeap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyqqbcmy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3sdbgfhrx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ovukfcnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cenenmfd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3enqziits.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3aixtibaa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ydzmiztn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fxbcfxqb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ptobcbvw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3daremzid.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pnzczafc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kmmgdiyc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xirfgdsb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3vdwgodfv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qkhnbqtn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cvvwjfob.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rkpvpijv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ulkcnxoa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wiogkbag.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rzjhyhql.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rutxmwaw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ygwfqukw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3tzfiydag.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hqlvrphd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3onlzmojh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rsapdpou.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tntwrgpm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fuphlasu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tcbggxgu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqdluydf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3txvrnrnt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3truziqyc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agrqdpql.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3edefyrbm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqdnzvte.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zownuszl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3obsgibjp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmsdeygv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrdhlawk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zakdpbku.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fpydmmmn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3kfrlcvlm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vsvcgtqi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxbfxdtd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jtndkubm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3dmrfzyiv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3phcofluy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmktjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukirrnsu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbdlodjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntjipqck.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjgbutcs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ryykggdz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3alrmmudi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fhrmxyro.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hjuvofhr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uhbgyxlw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hkbfazja.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gjychusb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mgcukaal.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3azohaaqc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nhgkpuwk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3btpawitr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nufqujuy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3viravqpq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mpjgugln.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3guyqujkz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3exbrbsbc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mwavwuyj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wxouccgs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3yhpoijnm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lfptivxq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mlvdhcej.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lhtlzwts.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kggucwbu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jebslprv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hzldikeo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mobkebuf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvyfuipa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qejbyhox.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rabhqcdc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tfkycjsa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jfocvqsf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3fcwkznqd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3shiftcpf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrwtkma.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fwhdctjz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xpjfsdsc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3acvjawkr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kzszhcod.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jgyzyeok.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cjfbgsqu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3inyaoygz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wklfrmpv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3smfgpkmr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cygqslaw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gstzbjcg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rfexioyz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3gbtoqisj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cbxrzleh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rctjisrb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nxigwkyo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kfrqwhbn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jzhxihqq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xzslkozf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxvflcmi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzjtyeq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uakfscai.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3virtzgjl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kzdeyxay.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bsagixjn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eynqgmek.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3vlnwyvip.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sxopcwcc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3eljluinq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjccugl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3okyildia.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3smpemwnm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zwahqoiq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lmcwhjwa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cggtsybw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qytstbld.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmkukbs.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pqcjkeec.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mazviydf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpzhsem.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3medmyzpe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xhpuxhva.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gmcpshvg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xykfvuxf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3oliwxawt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uwrfurdn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hpuqrliw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3dyhyopbg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mdjelckj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3adctxhec.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnkvtlqp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tplfpnwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3asyowlkc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwdilux.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3kifgmhjg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jqkqxupk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xmaeppyx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hctvvlxf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3abnqdmfm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zhfqtjve.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3delffjpq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xwccuhko.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rdofvlgs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wlmxvcns.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3etwbljmq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jntvuetq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jkosraez.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jbkqgdyh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vvotnnme.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fvjytddx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkyzvif.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tnokllhq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gafaxofl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3muhhruzb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3likxpfee.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mkejwseq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zqgtiwxd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3amtjirhs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dyfvhfbf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqizainp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jwpejoww.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oattjnkt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nlbsccqb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cgzilvjl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kfljcbtc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sabacckk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ccwuqqoj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ugxzealw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mlbvqcex.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3eyioxilo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uhlrgvcv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pqqywjkf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3luvdxplo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cjbgpkpf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eojpxwkr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ieshwctu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ifeyqvmv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3wwjqzglz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pnvhktwi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hfgugmjl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3cezauovz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kdychytj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mcxppyqa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vghhokvb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3emdvvqyw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmqsgxxn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3cfqzrqix.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ahqnjhqw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ikigzwan.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vpvkodjd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahrunkxo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uuvtwudd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qzjfhhge.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygglzvkt.html


<!-- 参考信息 -->