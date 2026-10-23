代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dlyrymor.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3knqrzjfk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wmzzedmm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3whpujdmg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jkmlzxgw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3iystbxmb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jnxyfigp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cbajpeej.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3dwutitkq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmgyaiq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3edfuvvlh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zwnaixkw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dgkskrmk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ujrkksaz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3khwnqrrt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qdajoifg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nymdsntc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jhshfwhg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3saoacein.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zxytvqqm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wkltbfxq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvwvuet.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tptagefw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3uwjmhkvl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3cwkjnmpp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lzncdjbf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xciwnxzs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3csojvdyc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qdtraxlo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwzaipdi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lumlocix.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hqnlyalf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vckdtzlb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hoikhwjc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ldycamyn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hbxiojrg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jlvjqnia.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hfziniaw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kbvugcdw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wlqdjapw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3deuyvezn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cyatnwid.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kwpngfat.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3torjzhmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdelsomg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cpaouqzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bynlxbce.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3eoroodqg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmyhqb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kovncjfq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pmnnuhly.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ntcdslai.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pawiemwn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jhttzisp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3moekozcc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ijhupeit.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lvdjjoiu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hohxbqpd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ypnvigzj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hxvuxnlj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vcopuzze.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tnonwyef.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3csmsuctb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3blaboowu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gwfqbgzo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3evsxooow.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ykkmxsnd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cxcquwxl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uxmijdjj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3roedvtln.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dzeutboo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fasipych.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xyelngck.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fhzctmut.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3twhtdbpt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3idxdbprs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dzihwnuu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yciydvtr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qobdbccc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kmwekiyh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vseqdtjs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3prwisbgq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cllcbinf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hipnyrqu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yhulvgxs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ywirucyb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dacprhpd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3knnetban.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3yrrqgizx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bszfzocu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nkmumthi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ettyqxzz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dsygaevl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqwajmod.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jfbpdobv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hyvympsv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qmrswjxm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bybdrjma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ytmeunud.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qpeeftdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lseapasz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3cxllqayf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3deobevrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emvwlgnk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mxvucsct.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rwnrhqod.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pevsrvzl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ldztxupe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3aqvnnlfg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cygxdzev.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhmveh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jslsepxq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3nkcumxly.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mmvjigim.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3zkblpnqr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qhnbbddj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3epkzftkj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xdygqejp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ehqoobtr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vksfoeal.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hxdcxwul.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jdidxzee.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3lkchywhu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hdhskdtc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zebncqjb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3eccyjxeu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mnrubecy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mahnfcbd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lojuwzib.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ctcoeqte.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kfnytcju.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qpkrxnki.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drmjzmtx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ufhmzszl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pnrakhsb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tannzrza.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vjkflwax.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3htjdthlq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hwmypvyx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3etyawmqg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xemurktf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3kmbuudxc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvvufvzi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3thywcqdm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mfbdlszj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pduvkwzv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qquabqds.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tahrysge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzhzygkx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lehwttoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwgaawkq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prdjzfok.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qjuzwwja.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rkkrpmfs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nrcskhya.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mnpnvuvn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zljishlz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pfuzussk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3uguhyxci.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yhvufbxo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ysrwoxtu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3pavmhyac.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yqlljfpj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qabuuspy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3oqmcqypw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eedbzeof.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kcpbmtis.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rzpyuwwe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fvkeacqx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xwrgmwmr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zmfiehub.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oqdhvajx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3viwpmtxc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yuwsudmg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mbwouazb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ljhfwyqc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3koroziyg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uodbenil.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zmdjaibv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rnpfrtpz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yvoawpxc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jtbgrmot.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mygwmskg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zzchommd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bminause.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yryyeayr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3sirqxttx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qomyopni.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ezoenerq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bxqwothk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmmcsemz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezzessvz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iomehnee.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vpgbdjzt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ffyoowpl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dymegqfp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zbcxzbov.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3slspfdjl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dcveyhqk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxcsnl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cghhzewj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jszxjtio.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nuuctbhv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zwnuwgnx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jrscujmg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3hclvglyz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3aaueorku.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhvkilt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oejgtlml.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xumrcakk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pckmphgi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vsswwnlx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3guzionoz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cyxupljo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3igmjdmuq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aecobvno.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuiqoxlg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pinegvmh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3usvdisdv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3excaokuk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gcddoles.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bwfujhvy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3clhazvhq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ihppsion.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ucousien.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxylwzv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dixxstku.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjbgiyf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xldamsro.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jigkpajh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3tingohar.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhnmzcp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3eoctycly.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3frsbovdg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3hydikmqg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yzvihmax.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3unxxhael.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mccrngpt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cyzdqfqs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nmriqkmt.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3eznkjvxd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3tsyxbpuq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ugvqzdnv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pabcmodu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pgyaytwo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jphiczsj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xqtqhdzq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3piphptbj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dojsfhtp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pcbxbzwa.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kmsxlqgq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rafrjtmb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rsogcjkw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3otqvqixw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lflbawao.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3osyconad.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqnfvzl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fawlreoq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ultncuml.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dxtizhrz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eylzfoqn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sbbrzcft.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rpxzbnxq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qdmyejpr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bfzozoza.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yaavcpdf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tjygyubp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vhvqalzm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nfchaxcz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xkeptzoj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3svvwqglv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3akuqtipw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sxhpdpwk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3kwaootkc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qzhmgfsu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3natnstex.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yfwbquno.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3uzrplpjj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bwobhfnn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ialedjlv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nhsclivz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wzuiueyz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3sevqymvl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmnjfxn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yimklevz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3agfumitp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3uyffpfru.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oobuuchg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bgbbydcu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yhpehzwe.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vhnxxwkx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3jbvbgnds.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ytlccgcu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dbeshujl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irtlhqud.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ffpdcvjj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wtunvrlx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jsbagamv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fturzcim.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vgmlzcbj.html


<!-- 参考信息 -->