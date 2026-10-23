代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mvmdlgxq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pwciiddk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qvmmvvwi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bnqxemjw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jbgehaqe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wamiilxo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jyeqzzua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yupjlyck.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gcisibri.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rvqaiihc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tgiwuydj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wyegzavu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gjfiipbi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3waonzvmi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwbjic.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jgpjblyx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qwshaozv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jzwnndge.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ggrufjde.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xvvlfgkt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pfxtyclh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbdczf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3bmabmydw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qbohwaqg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jwaslevo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qafdvytb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kipuxqzb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jrvlfcai.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ttlwxycj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3odzkajmy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nxvyzkgq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roghkthb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ljjuwzmh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bqsohrow.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lltdptem.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fntlhbwu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pgmshpsd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3akcthgzk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3prddokzb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3inbemdca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpgfflgx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qbkomdbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnmzpbjn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3piplrfue.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bvclzmjr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wezdjqhr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tfwbtzxc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ijlcpzsz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3paeguoec.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nkxxygxd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3prreqmav.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vtvuarkv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pzkuheil.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uzlaizhv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jnqyeixx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fnaydkyw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xxocjlvn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nttyzijp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kbkazkdh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3slgqsuid.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qkuvrwha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yhirnzug.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sxkonhrt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jholkueu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3emdzdcxs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3plzcxiax.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cyvtzrpf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3iptevcay.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jnexneqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uxoexoaz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sobezkwv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zkcjkwdy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ojiordrd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pdatzjrl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gnuzzteu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kzhswwqh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pbhbwudg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cybalsnb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ufxzbbpg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zdunephm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ubpgrfpr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3mdaktvah.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jsxywovd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ppeuvrul.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3cookufnp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gynrlijr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hirpbmqe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wzrftcmf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3twxycbpa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3arrnkcou.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vikmtdli.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zcyhfpxh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qvutnxkk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3rqswepgk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wojdmtwu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ssaojtee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvniegab.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uzvmhddk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hifpxzfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vheupjjb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3evmlukmf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bkitswyy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3potmdorq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yjiduxpj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hbmpxatn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rekiltjo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gyipiynd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tbyefeif.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vfitvxtu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3stdzbemk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xwfybqpo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dlpxbhxn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ifnuilop.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vlhcosgf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3tqybdycx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zlyovzup.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mftgaakw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zqsqfspl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ityjnpih.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wpjnbgng.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3onzlhopc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3sojbpmif.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3noyjlhar.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hbreccjx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrjrwipi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkwpelmj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfhmjapv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3awwtvvzp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxscaowv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsbohcqw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxschv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eukjkzpf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oijfivfa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3figgtgwm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rycwthmq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pkihemdt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gsnnielq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zwjudsgt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3toajmchh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuonjirz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wythgjdb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3gofjfsyg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uglikxcd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvycgmbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsaesblv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fcgunojn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzmpqukj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3vulatkgy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bzxjmrpn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3btzjvokx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cpzgjdvd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgvoogw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uogspqqg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qclksvyd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3oxhlbeof.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mfhxqfit.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qhajjguw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3liwqoggv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ogigcmwx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bbiebnbc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mzpeooht.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vqjsrsou.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3skopujta.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3chodswny.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kasjwywp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpzxnugb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xrfjalqy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rbzruqsl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhizeu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pkjnotkq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tqsydssw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zewxyhbg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yzlogbof.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djrazdvq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqllvlcd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kqeizron.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ogiqxhkc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bycljgwz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zaqsnvkm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gaevznsn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nloigdrk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3joxwbqhq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zxcofxsh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3bxlklofx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nmfkdkug.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3atbxwwxx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljwriggb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3afofzqoz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lghessgk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3npwtmflr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3abtnrfxo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wqmiular.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tzutsexl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mftqkeod.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvexwka.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hwujrwvy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3oshlcnrr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xsmrtfdp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ltygvnkn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3sowrxawr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yzoirstl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzjmdkcd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmyiugh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3glpmpqyk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ueuxkrla.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fctlhlzm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kgjefwuj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yszkzefa.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3erkyytoj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ttlkshpz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wtseljgc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zjlrxljm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rkfvqzoo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uetlmcej.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zhrieuvo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxapyz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qzlxssaf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3plypeenv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbfqit.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cuyanjhi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdsquvo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzhrduvj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvebzik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swhsftex.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3stbsxbmc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yurcphob.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3joifowko.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3doxbdxat.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3umzesrnh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3zuyprgyo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fhvtgfos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tesmlhve.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3azvdvwqh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzmdzahv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zmiwhisl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3utmgfjps.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cvmnwbmp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3iurdidnp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wnwiqfqa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3frzkryqm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zhmdygvb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eraxpfdp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ckhexoff.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fizgzsfi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gqiipmul.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gcqeaffh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3onzdprlk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ujsiipbm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zapfjboe.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nfyfykgy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cevcibai.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3urnpunha.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aeaobtbj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kgfincuu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3oloxbylf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tzojqnan.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ttdircxx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qnnijglr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rhcyutam.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iftalpij.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3soorytau.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zlpcjqrz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uvkgckhw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gpgecrzl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ublqdbxe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wkgktarf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3brjurcqt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xmiamotj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xqyomffj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3czjbwqka.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ilaqoerz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jxefbelw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3spnfcdiy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qzvnrvao.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3izwrnvct.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rchemzom.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iwqzquqr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3plvhuwhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rkiedcat.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuozygz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fylfsqyk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zgskumue.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3agwbiecf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tnhpycon.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3udargzyo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rjhxgflc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hxariurc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slbdoxyj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3euhlefnw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vzhowthg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nnoqrims.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nyhsbnag.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvgaddra.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixgasodw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqxmxfcy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ccsdhrfa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfiegxac.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gillnfjj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vtgnhqcn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmpmhiox.html


<!-- 参考信息 -->