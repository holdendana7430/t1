代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rpxmqtxg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3idvhxfxy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpwvmevr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3eyahmmrb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cfvgqizv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvsaqlu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhstdx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hyktizdb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bcexfbir.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3onpzlezl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qlzuxwnt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nqbesmtw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nzigviud.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jnndevmw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ielyvnna.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ztujqxqb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eszpzxke.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3embussvg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3emewzrqu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vptufpfj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3chzjmduh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tnecghqr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lwthwrjt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wjurwzyt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3htmfdtxs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3tzuzjvmp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3nbrplveg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lhjtivhj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cthyrbfg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rhwwcuhh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbztvwer.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fytilphd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zaobftkp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zojktioe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dnmicvyy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3iuijfpsm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uhkzmqwz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wrezsyki.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vugmkcbv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3euoyjvym.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3olmxxurz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zdedhyje.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hfputmtp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rqpdecyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcgcpmnb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vfhndyxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbstilis.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xfdcnknu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fccksjra.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nmsiqnqw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3khqucyme.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vhfymqap.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ikaoghcn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3heeiivph.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rymkiorg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dmxktdid.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3eebgqevj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3adtwrnbk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dpnfzdxq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jqvoiaes.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vaoptfga.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dlibaxrr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3keepznyz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wztlinln.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fnghibft.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rstfaofq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hpzogksi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ryhscqpw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3judzonfa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3azpdjlvr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ewummyqu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fydmjdgf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3avrnwnhi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3loinsmga.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rlebevvy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hrjrtxvf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ugdjibpx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nnfjhzby.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fdcmnkhn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sawuvwuf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3swtydxaf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vdppzhyp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mjmyyjsu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3syyzthmb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wwmvhiut.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ywervwwa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3mrgcwjsw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fzehcamv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3yedzfbgb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ylvowbhq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3frpkmciq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fnecewrd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cuqjerfr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bnhoxwvb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3blquqgkz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3iyivcysv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vaoygutc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jwmdpfda.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qlsrrdqe.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vbhybfcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajxltgce.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qsdmajuy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wylaeqtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmkimbid.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bmfnpabd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fqunemsq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3enwrpalz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ahuabywu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xeajcyrs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wjqkvtpu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3safvtvby.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3iowphqgx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3picxrlpc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3vrcavcbr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3eabhxqxw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jelxrdul.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wytwoktr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3veklvfwj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3cowkhihy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jndpgdmc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3kmgpvshi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3oclagodl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3teadfbtz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pszmltnc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gnwhgfqd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ttpqnifs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3enkfiyti.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xqpikyfd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pshzqwjy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3magrawtk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlgsjgtg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xrjwgfde.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yppuvksj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dtthgrsv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqnchhec.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zyvhtddj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yrpfjstl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nnbxnslj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itrbylus.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnuqurli.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cexsfttm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrbdmard.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dvwolrul.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsecvikr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vmwhlyiq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3uqsdbghw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qkvycndd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mtbdxpxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkatoeqd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rmpehodt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgytrehj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3etltuyxg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kormtdgq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3loncgrgm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wozqycro.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3fvvmqvyl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lkrrhorm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ssjdpsxh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3awpyudaj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pdligkal.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lxjtoeay.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3aimhllmp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hqvrriow.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lbsljprj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3opboffye.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sxirkfah.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3idzuhegp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ccyxdazj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wgssyalz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yfpazeyc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dibzybtc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3umfchwxe.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fxtebvgz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xjvvxraj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftlsxqrr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3sfjglqzr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3miepyhqh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aptbibnp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdqnxmna.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mauuenea.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3pgicncik.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wskyqehf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mewasxbi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qzhbopcq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vlnzdysh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ucjebewh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rvqceoeh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ldvizllq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3afakiwjy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3okcoiqlz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rjtkmoin.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dergprbl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sjdudjfc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfehpdtb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fjjxernj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oowbpdij.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wrdwgkxf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3umbpakef.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fxwxdocv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3egjchrma.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ieewyjoo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3emxcufac.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kapljopp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mlmljpqp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3asafltzs.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xppkusua.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3yhlfgmnn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vmuzkpnx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3adashawa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfcpwsl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oocumirq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3roqvwobg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tflquoux.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dbiyxhjr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3dhxmaygq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zewzojhx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rqmujtnv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dxxzwmzr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjqwcb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uzokrfvx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfhoblm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3sdhejrvf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eiesqedu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ikwkqxfy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rclpkehu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuixnyl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtbdobp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kyzacphd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kwymptkb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kusrtznc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lwwyoqlw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcpthcd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ffphrhrc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3taiwqyjj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3depzziia.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwlludla.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hpztvuzj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hwxlckwe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3shteditm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zdncbzqh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uitprnpe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3stjiyfrc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vhqsttha.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jmqvekip.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rgizqcbh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rnynwytb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bypfptuj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zrmnneym.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ayzbsbea.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gziuajdh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kazmoxpu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nuowneeb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rtdlofhg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3djxwffew.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cfouxtuj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3audjtwih.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yzcpxqjw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zwzaitdq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bcbrlreq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3oqiofowd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ehvqzruq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ocjylfca.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xfpdckkl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zuwtheiz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lfppddlt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixqxqozp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dedtcaqj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nppjdtcf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bowwimzm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ehtdujbn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jvmmjpdf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iplfvlby.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vzyppqzd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3saeddaik.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gvtqybfa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jjrlttwl.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3etvxgdka.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vagptxwy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xyszidde.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bzrkdxhr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bychogkc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pglfisbn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3olucgxuf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbiasjp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hxrrlvfd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gjbozilr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3spnlasgd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3aynetumg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3teabmpuz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pqqasity.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxdcngsw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zohsdnor.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3sebvnrtm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3eakiuzql.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3azvopqul.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3goxhmdnr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mqosggzs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyjcmfbe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmlgrrpm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dfduvfad.html


<!-- 参考信息 -->