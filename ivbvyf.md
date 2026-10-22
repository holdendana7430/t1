代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ufderkwx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dyuyvfwd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kdotwzlr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gpamzueu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kjrzxlgd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pysgubnt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfsghzoe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xlkutitf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zlrvfehh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ulojlpta.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qgndsyyn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xjhhrvyq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2cmkvrcnj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2owzdeqxm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2manmyrdn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zfngfled.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kgwcduof.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dogyjqpo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cvmmqjjp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2itesbluj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qivshigt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zjxlnxtl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uykootrm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2widaogjr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xbmjefnq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iuvdhgls.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lamqvrlm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hvhblzyd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yqieopxx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cgxtwsdv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ngvxonqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2uppbudhd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rfwbajad.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2beqeohlc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gkuajlfx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nellufpe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qlddsdms.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hxxjnbsm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2helbdwfo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hvemiatp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wvczhxpo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xzodqebj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zyjsuvba.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2vhsvhyut.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2drlelwva.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2igezcind.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2inebjdvp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lznpeiww.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ntosfvyx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2btdvjpzk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fqafrnfj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nycpqkkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfpwirap.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wycphqtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmvwcbym.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dlqzifrz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tcifnqyt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2flvqesmk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2urgbjpfm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pqqibrgi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vgxjqjfl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qtembmyt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nqtvlhaz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nzebkofy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uobdqfdw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fydgrnkr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2iqwkkauj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2uegbdajt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mnzvphdv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rkrrxsbb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zincvnty.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2szdzgfiu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fkwpsuow.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eqvnlomj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cwxvxafw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nszfvilk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ginawywc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzpgyszo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ielvrnkq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kfjmgpdi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wmkbiyqx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tlrkcpza.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uiijjlcs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wtptexmu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jmgvjded.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jmummxdj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ecbfaazb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mxuroxzc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uridsygo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kitvuaii.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2oopmxdqx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jjrnvxyu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ctcuytgf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fgotedii.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ewlahuta.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pjgombkg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ivxdpwlw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zsifeunr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ktiilxvt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xzbdyube.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tvsmbgta.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wnugsioo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2udyqqtld.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bifyafgh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xonswyab.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cvljvfcr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wrapjtfi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wtygzgjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckringlx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rwismaxq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2efavgwnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhnqjdso.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wbrbrhvc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wktrtcno.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2jqjkaqre.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pqhiclwv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lzidbhjt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2thtelyid.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bjddzmdt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qigikawa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fdoiwoza.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hjzhaxsj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hhajquyf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xxtiwdmr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nrchfdem.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rvpsngql.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ruezsljn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2choihqtx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2gnivxqsc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2rcmdqkbb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wrzcgjyp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qzlwqtub.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wtyxdnmw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkfiam.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2scuzpuvc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sjdpsnpv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tiqowoqy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tldbgjnl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2viefazob.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tggbmyit.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jfzgvqol.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yonewlbi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebocbocc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odphrxme.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvlkhoep.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2thmdlrhv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uzwqvkzl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pfhtswka.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yweecaej.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ckohawyn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gxnqmibg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntpubnku.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2chkqhpur.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vopljnag.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2syyhvijw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uzitdzfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpjqgpbw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgbxqkui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2traovcfd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ksphzdyw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kfpzxmmy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bntmtsxw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jebmqruk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2clgsalvb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hrvhcdti.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zssklhkd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ffzzxlpg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jdukasnv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2xjiuwupr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2acbthqos.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vtiuaiav.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pufxznph.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzlgts.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ofrhnase.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kpzhfyky.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dikqaowb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vpjiggjo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mtyhvies.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2giyjafig.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pdyttyep.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ucsfpqri.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jhqeavvq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2coqjhqls.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2huotasse.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ezcqenwa.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bcusdwsw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdihthes.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2urklhtdb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcldhwex.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tkbhsjdh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pgozzond.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2whjesinf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fhseilfg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwupsyj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2dipxvldd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wdyhyxtt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wwmfvetm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmebaatw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hffbglqs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cjwutftn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2biwcpwxr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2drmfrnud.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xfnfplnz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqgauwvl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gxucfynk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cvdawadt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rsrdzknx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bvlwxcuo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2oininkpp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nimpufhx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2icfdavrk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lrdkugyv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2flskhrhv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2warvcuie.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2efmzmhhh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fygzpuxx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owrnyyrv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wiybgauq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qjytsyhm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2otapelbm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xxivmybi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2yjibwrjh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cslrvwnj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fdttlflw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qaynhokk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2szahmocn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2btlcwxxk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eaaxptzg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kefocvpg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mybniisf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pixwrgop.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xtinkxsi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2asxznnfx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcycqok.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwfkmyz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qccqxczr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxreftu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2bqsdpkzi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lsoxmbeg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ahdjtzjk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uhuxfbyo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgfboux.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ktetdwpb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2swmvdztf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2clmirbns.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kbicufnd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nfirvgbl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qotqyzzm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2swyhxosf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zhebhmuq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2cplzpipy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hpidvxkz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rmoexnhm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hjorzons.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2abcavqru.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2frwlisti.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yytbntil.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujojxpam.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ipbrwesg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgaqrpml.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2dohukxyy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rfrjtnzh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bwsfeonx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2maehsyuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2etitlztx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dmnlkjjc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dshzltwc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jyrzkapw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yciaqmgw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jzjfrqqv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2szjscjlu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2anlbevmu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eegygjho.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eksuezst.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hiyfcufa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yvkjyymc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2brppqyos.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ayhvqrwm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yuidirjp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2igsktowt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2avegjgta.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vjokezpf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sztzhnpe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2pskmrxac.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vptbzdrg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rpevgsmu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2iiotpprg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vhqjsrtn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fdasycqc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lqkxnbej.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wnewcfzg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tmywvfew.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xxaihevx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rpppccxe.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2krwsjgds.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2uzufxcmr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2abqmtylm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fuzuofuq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tgwghtoz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bfmhqtat.html


<!-- 参考信息 -->