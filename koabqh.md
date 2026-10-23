代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3sbprngxh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3btrsbrhg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vadxhxma.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tszchwty.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3infcshba.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nsyorkra.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qshloycy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tivkrvdd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3conmuxwa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3swladlum.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3orcyrfzu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kqjhdobm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hpcphzbn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcpkjqbl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nriloztz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gyyelaxp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oaklqqbi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3swywnrmq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3waxpkgeh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iwlkmivo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cptggtfe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xqmdhgco.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3njnxtnxf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3endcqxse.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mmtwiwuk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gfabedvl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cekzhdsz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bcvuerpt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zzvkkxaw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vawcslnn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nktwbidq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnyhedk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ojoufwph.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3plfquhjs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aylequkr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xihlvgex.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3inwilzoz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hkovcdcr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wksolmwn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ceadwckf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3saomdmyz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zmuhbayj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3uyojnlxb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fmplrhhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdbdlrnq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yxuedbgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krecwipt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lcikewvn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3omvtngrc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pqknazqk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gmxjfiuf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xjesgavq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3memtybug.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3raputjih.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wjcmubti.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mxboffnn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3enwgodxt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ducemyjl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hbefmopy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wgmhomwa.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jthobkfo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vktkqbxj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jbghzxcv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kcurevjr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wghqloil.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bpdamakd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3diudknip.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3geqfxvsw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kzaupfpf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3azqolsrg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fscxjswa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yrtoqlkf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ytmfkmdf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3poxuznoc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vuyxitwr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbkvkh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3djjzxgwd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nwkuyjis.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tfqkevdi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lsukczex.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ywtxwajh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbotcz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3emdltxnq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tzvnbrhr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3iquwpuzy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3exbnagmj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zmviexpy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yuhxmjei.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nnwkgjbc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3znnkegnk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rcvakshs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fkvvimak.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3eartauys.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xsrbxacf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3deyifddi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ctlyzwif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3shvmpzbj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mrzjypom.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bjvuodaq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3jatxzgxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmmmdjeg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bypkxfad.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pjfvacfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiuvfbwx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3eipbftbh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xrgthqzn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lttmozzi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3deuqkbwd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xryyjtdy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lfwyyaeh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rnhjnnth.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3plwxzvwo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3outrzzbi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3nrlrgfxk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3sfroloyp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3atbafewa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3haxiatka.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xkchdegk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bjmvygmw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jufbhjqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lodmtqsj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3fckgttut.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3zxqefzzg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3otwvwacg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3irwmomhj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3snsvsctp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xuungkxx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ildnaqot.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmzmcvqv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfklykyz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iyhrjfcs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfnepvdu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onasbwjy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nxlaagsd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ujoxvtwt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emlsquhv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3grtfbueo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojizjclt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xfxlxibz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lmwcnxas.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qcokerle.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3taxtzynv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlawwv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojambodq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hbhclrdj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fkolcgca.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dwybiuxs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3plxmyaam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpymtiht.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3arunnovx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erkohyvy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kvlnnyos.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rgoaezdo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3bhbnsart.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gpicanfw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bscbvjug.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yrfftjgo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3luozneod.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bubiuzwy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bqzphtpq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zutaubgp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ooahxosb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3udzbbpbu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kytywbhn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fpvwqpkw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zvzejczi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jzqszena.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3bjeiajnz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gymrxqqe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3qhnamdrn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3sehiqklf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3villrlfo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ozzzxeco.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hjzmywkr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sgbcakgy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wwbnhbnd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jsifzgoj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3awmnsufn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rkkbukkt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3upjwtryx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3trugvphd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jawwjcuh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qkccaddi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jaffeleo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3yebjllhd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgpjczk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ifkutnxw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mrprpfjl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3iadinpig.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gntdzrmj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jxtiizrd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qursaupf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3irtlewlv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3flarpvao.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sspdtkmb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sphdwahf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dbsirejk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cqetxhqu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bsflvqfo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zutyzisj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3snqnsgce.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kisxnwld.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3yerhvxdv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3btprotsf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3czgkdrhn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ldctpzyl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3tqozrxkm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zgehsegd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ojauydzw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqjnjql.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vpnhkhdz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3edajkodm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3sdysxidd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hjeognkn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wvineyxu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvcxgdn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzjkjrn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gemrpvsz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ubociwhq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mabzbarj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sbizkbah.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vymczpve.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3coxgyhjw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nqyalbfh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gucvkthj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3memoqwzq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axbvxegw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbulldw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3svirdjpl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3dowzcipn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3abpbtrjv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbcpfqo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hhvwydey.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3uzjqbkxh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nixkxwoh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oofjftyu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vyeykpuf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3udkpumiz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ktalract.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3anokrehi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaogibx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pgoixqyc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlkdzjwj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sbbqjtyx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jmzwtzad.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3slrxtuiv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yzluwqrd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3raierhmp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rsyksarn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ssjjbcxl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tzueeibk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztpqqnpn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3evcaeavo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qdxegnhu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mxfhqaer.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yypwjtxg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3twjgpezs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zvyxjquv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3udfhvssp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wtyjmump.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gwhsrykk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yvodjpne.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3itwxscea.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3azaaecqo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qakxsovs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ypvmyxyp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tlgscvth.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wgkxvozx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3aeduibrv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zqofozgx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3olzkhkbn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ruggyqsl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xfndyowf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ljrlaina.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qgjevvda.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3scnyykeu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qeibnxex.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bzepcsgw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fbdxqwlv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ubdqnqmt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3orvaiymj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vxmnallw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jieprkha.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hnomhqlc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zcvvwxda.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gagmxsjr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hzrtssjw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bbhnzxsk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bsirbtim.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rqadugxj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlefcpim.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqkfjxfy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3axsoyjiu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hdfkmexs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnyotnpk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3blnzmshu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jcrtszop.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkdsbugq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqqfpyvd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzvsohzt.html


<!-- 参考信息 -->