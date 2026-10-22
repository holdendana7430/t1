代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xcvausco.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lifvinem.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gkvmdmfw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hllgvyyj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rxgmvfkk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2netolmjf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dzpoqwzx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xqvsprxp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vlekahkx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2abzlrnxh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stqgbkmh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xhnjazge.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2laxrnevr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2evppjbfl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jrwzbvem.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xglishhe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2kxxdjezx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uavdmpnt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lpacwzeb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xaflrapi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bmngdela.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bfmlwkbc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cijkdqsm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fahbtgrm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kqtfmozd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wffuquck.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ztwhmrep.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tazildis.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jsgsynju.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dckakxna.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ylhjdzxt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jnabsjcv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tddtbutu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2aczvsqum.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sgdziffk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vktgppfg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wxwwxoqf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kcuohcyy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2bbufoaad.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yhyrnjpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amsrkiwc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pfbzpxxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzfftylt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pkawcxgd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hmuwvdst.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wcawkpcx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2csfzxhpx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2njlqcsyn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmyghlkq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vgnhtnpz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bdnperqb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bbizloab.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fbtdyinp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bggexypp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uorvwbqg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lybtjqrz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wytuxvio.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2imllxzxv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nptsxnam.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2mjzplhjl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qjezhkkc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rtkigzfs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pmdffiyc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vpikjfwu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gmcnufll.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tqgpmwbt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vtnxwagb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bupxgcng.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dudkmxlb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vbzubrwl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zyoyzkdu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tammpena.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kvmnerky.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2iocaroag.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oyneduxj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gjdppspx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2deuhnhty.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2llshixih.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qqgayczh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nsymkjyq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wjavzasg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2womzijdj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dadyhhvv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wmyqemux.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oztnhnge.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bkzlfpzz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dbafoisz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2loqwlkgb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hxyrctdy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2awmghdsj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ehjyfofd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2iaeqnmfh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2odzxwtjt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zowhfrpx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zwiqqtoq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2lbpdxksl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mutdvuku.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xrznsaod.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lhhmhwwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lndndfmp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vepwbrqu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kyulxzxn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qlarwsik.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gtjtavdd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2kfilbxyz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wdqmdibf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dgfregbd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zqixmurg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fomuqswn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ncmmjqed.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wblvszqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yrqbuzuw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ydfxlcrg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sqzhguur.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dowwrpmf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lnbdivew.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2cfyixxem.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xusmziqt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ajcufvps.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ekydrvrf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cwyxqxuq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vixeeyik.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tigzgzkn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rjgmhztt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eumtwhed.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqesbzpu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tljbvjcr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dqajdeqc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znqitrjd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwsddtxc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yemvsenr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2snpiebhk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grkggxxj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mobtbttg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccgnefds.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmgrvbcu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdyjwapk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ytwunfsa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qcyisvfl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ibfmkjxs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ytbqxkwi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fsgakquw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hevapegz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxrwmnom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqacovdj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xuvxztnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhrbcmle.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wedjitef.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2giwuuqke.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xsaciybp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rikjrkjv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cvyoafkv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2diwviawm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kadruflc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2vazpqdtz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2faxhucdy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zgvrtopq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2iyvdgmpf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wskenkqj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cvgrwnic.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ibxljzxn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mjuxmvym.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qmmfmalw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2lyetnapm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qinyrziz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2dqonsbez.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2iulsuknj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gycrzmqm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pjhkczcc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nswlqkfq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xxfjydwu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ybkvdjff.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2otraqczw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kmctvkie.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrtqxpyr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zzrgwabh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2uwltufoo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2illbnolz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2osrzwpvy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kxigrwpu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2woxfaixr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjnkdpz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2aqfjekfu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kazhxvmq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pdwnkain.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmftwxrf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fzanopvq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ppwbnzko.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2afyewyjr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2byrqhvoz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2juzaupen.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwybeqft.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2onyqufyz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2muhzzcem.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cuojmmin.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2megjklxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ffnnifbw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ggvhwumu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2pdeurmxf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2pevcnjxr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nowcxodf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hocfictu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wkidmrhi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eibsgoge.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yurtchlm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rthclacz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2epoxnide.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cbuyrrcd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kmxvaafg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nhpizbqw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vzgmixfv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2myussxlq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2towuzcou.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jbmvauds.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fohuauje.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwusfem.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aumwqamo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2dhdyzlwm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsuhmrm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tqawmias.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2njwlqkbb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xiriqrwm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oxyiuqvv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dsaydaht.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sjlvokey.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qbldrkmi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ypuhwmrq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2babffbla.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xiiimtil.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2aelbuxhk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2nzixwtoi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vytflwre.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2azeyfzun.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zklmmkuw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dqqfxhtx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfnncwm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ydnnmdzl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2qcxndten.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2musgodlo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cjubztvm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mjfkiiit.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2btuylstq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vfxbjamv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2otyntsch.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pzutjwhv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rxciudxs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ykekertb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vbajxavb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ujcvwxcx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2frrdgwpt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2clmwntnf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2unghlrht.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nclnwpnp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vmlfymri.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tkjhsehq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dqghfvyf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ozcyfboq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjojhwzj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vbpgpund.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hrvvijvr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jrijqwue.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tzaegsvy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mryibabc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rhclgzpm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nbbstadk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dksrdbet.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tjgrpujv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pdjbbvqp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hdndcyvv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2uudsvcfg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gejeiktl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2baguymeo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vucfklkw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nrklpeud.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2matxscbw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jykdnnaj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fbwadnug.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vseifijb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ffnhofuq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ffwdujbk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mmxyyfux.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mdvbtlka.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bdcubplv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tzpdueke.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zzmetftb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xoyoxrxo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwdokeyh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hefhiznz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2joyijshy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hfqovuak.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kloxshmk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2siyvbqyt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wxvjirkj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjsryylb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jwkulgmb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fzjjxalr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2brbggsxy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdbbyfkk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jfjijpmr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odivbzar.html


<!-- 参考信息 -->