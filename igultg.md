代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2usiymwjp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nocxxbdx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vywkfjum.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fjdshgpt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rdlzccqq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xmuonenk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hgkuyriz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sqckasjx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fwhedytb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xotdygtf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rtogufyn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rqhobizs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uydvnimf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rxujpfzd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tvmbmrkp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ybdwlcea.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ppeeppgm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vbhkiekw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dvikqgns.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2acwxhdbj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nviinfvs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iesyvbkb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hlgltlof.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2susgjlmb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bofgrvms.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lcnhozpd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xedfcvkq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oyklaasu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2auposmtc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gtyjyjga.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xcnskqve.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edxgiunp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fkihfdmb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2iemsbvso.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sciautjr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2schafubu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pcqavtxu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ocdtvnsg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fjfevqhu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mwfarljw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvmzfcnd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rvthbpmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wysyybcd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xpyhsfmn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jmmiwfho.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2anskbhah.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ywkkfwck.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hrvmcbxc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jqxvcxzv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cffntuda.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uoigsfrc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zcznhznn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2zycxcgqv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mxvlxzat.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tokisnwa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qxpisbrr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxmvis.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rjauvnob.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zowcbjrq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cpwsqlgp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kiztsslm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pkjvcbhl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rmmumrws.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sxkkzjbn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2coutzktv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mccdnibi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ciorctgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dttxwkdr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lnapoftf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bhnrugjg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vfflmpzp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ybcewdca.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vdicokiq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nqlqaeck.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rvbmbuzq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2blbavzry.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rnofzzkg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uhyvoakp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fzcneqha.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uffmucvc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vzshbwbh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vtcokcqv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2edziblwv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vxigzfki.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gavxerxs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vpyqgjqj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mjlujifl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vqxeezah.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2mqhotxxg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2agbnaqdb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uklcrwed.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mmfppgjh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ttdrlffe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2pbfcyekf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yjpdsset.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xrpxkhuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgmrhpok.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zmyhvovu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2veuwqguv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwnzkhtq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ooshyhhi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bhrpqyhr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fkcfzkqb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xszcunlm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ehabgbjc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tgikbbgg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jvvkgpkl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zhxqhqje.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xyrjxoxb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2drhyahlv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qgdswjgp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2veywzxnb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qthwypet.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pgltsbbu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2anphkhlj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zajkdmef.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pfcyvfrl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hbipjheh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2blvudpod.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2fexylqkt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axcdvlmp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kuydlmmn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ufohygts.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qtwkjbhc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpkipfci.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2makvggpf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qwwbyxkx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bjumydwd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mfhaxssz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2diunccqe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2izpiaafs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mlqlayri.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fyzujsry.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cqxklexu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hqpebrpu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jxfvhkru.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsvifyma.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sjcotouw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkgvff.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2oavdzshw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khvpjmuf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2twixxtbu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2palpixhf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xhxyoope.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naiwsnuo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2aozaohtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvlrekxb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mfdxqnsw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2betfhghu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jomikmfe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rodncgxn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mthmkoig.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kqgbndoe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lttytbrh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xvotpdlz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cduoybig.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kmajcgki.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2inokzrjh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zetpbjel.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vlyqinwp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kpmvxebv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gimjzipb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2kgsqhmko.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jqcuotkm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nijmaqal.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjfzcxxl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xqkngjfz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nxsevibh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rotkltid.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gvbgieck.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzgkrwvt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cbnpvceh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2arbqosrq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itkziaxa.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dvzjcxxo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjznysg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkotykvy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2axfpqsvo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wdabtzwg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2birisgde.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2srrzdbtp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jhirmvfx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hyavdluv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cfqjzhle.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2jscxtlyx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mllhnnlt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2obntdsed.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rrgfamhs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftcuxwdh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2talabnfp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwzmscvd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2byvnzqne.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rsvvzaie.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rxhgkvao.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2jfytyixc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hkcugudy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tezjiwlx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pcztomde.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eicxukkk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2sfjlczuv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbzlneu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2lmeszofc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qrttkvex.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2knyujdkh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hngbuxag.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ircynogc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ktlfgmco.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ofnqnxbu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2urlhlwld.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qcnrcygj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vngzyifw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wfanadwj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2elllcpqg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2okdynzpr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2coipwxcd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcgdtzw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyeenam.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2uokbczln.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2quivwhhr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jqhjiwuv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bethksbs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eyoaraeo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsugfwnd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nohgzrgj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sctlxmxs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhbyan.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2eidtswqc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skgiiyfp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xmlwjamh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wepcvnim.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jsbhwtti.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cjkfvxhu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nrggfyem.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qrmvozkj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fxgtbyhk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yalwndbm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bglciqtk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wposzqki.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gsolnxst.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2knrhqpii.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2usjhepjk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nowvmdmm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdmfhyze.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zplzukcm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ddcakcgt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ltoqkzrr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ztkqkhnc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mipeyslk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkyloh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qmfmczlw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2celymtyb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtpueqx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2adwsfgaf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2yjadgzdk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uxkvorhh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ytjzdjfg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rszxlkgd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uetxyjnn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ivxknnlv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dnilmwrg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fdpfvxlr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dxxqhfnf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2becgztyz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lxobwqbj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2swgiczvw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2hlmcctam.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ghrymofu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dmeeuthf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ehaxtiwi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rycozwhj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xndlvpca.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fnirhcgw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rodhntvp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nmqltput.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xcbpinhe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vgnjnzzz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ntiaahan.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mlzkouje.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hhhwkssv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mxyiyoay.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ehcutiir.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2alkngyzd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nhvrygnp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sebffxek.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vubufmqr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mneoniqs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgixhq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cytmscgo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fizflxre.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2garcncts.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2aenilfuz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2phkfuaja.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2melwnwag.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dyyynrjv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dugbcjob.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2epjqaniq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2esilyngh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfywzjyn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jtxcehze.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvekaspo.html


<!-- 参考信息 -->