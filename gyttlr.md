代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uximjlmy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qndpcdor.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3onqrkpcj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ddmvgziq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ddluwhdg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yhmyixjm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hzuvdbib.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wxwrrtdm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nccaobhr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nikzkzrw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bxbjlxqu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vznutlef.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gxwvpduh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zdrnwbcf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pyvetift.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3oshjpwbs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zgfadjxr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nisairtg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qcmuaqzp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3maeuemja.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3azrucsfg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3behuceai.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3psubdzft.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ppoolnkl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uhiybcyi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yoqmovfd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hvgyckoe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcgymtxb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gumbpqar.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgvkvzwc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3utvtvpyn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hcgkushq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3civpaeoc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wkotjwgo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uyqavzxq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stggyxmt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cadtpoxr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aymugder.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3glzpgemp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mckolxsx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qdajvege.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ishbiwtd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gwnrqjop.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xiprowxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eckzouog.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cksjiuiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izuaqfoo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ayhyfebi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yuruetuf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qeefphzz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gbxkutmi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lyhboxsl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tdoiwgqs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3somkleuw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nuuckjpy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gpouqwee.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fjvxtgkd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yohbzavo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3orxhogwu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3zwqslxeo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xygscqjt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iwnkdeoy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pfmzcceo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ujgkhwlf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3burqivzw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bjkiiufb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tcmgdgxe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jrystpli.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hmwgovjo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hphvnzon.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3styazjms.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xvtbzwhp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pvnuqurd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xusbqnfe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ebxkmtlu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3swzewmer.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jgernfps.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gxeytxux.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wjtykljg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dnfhyfge.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vozldheh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dnsjhuyf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3klwdizns.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jwiglaiu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vswzxsjx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3rqagmqst.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3oaibyber.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3juynaarg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kwadwfqh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3awrjurjd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tmwmbqwa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xbruhpjr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wcylittg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dofewgxd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zmvzqhtk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3imxmqpfs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3sudaapnl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qxnggeha.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3pjbzawen.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3shdkaxqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmcdjlad.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mlaymrxw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vqmwoeam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaxhqrce.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zojbxrva.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3maxpsvqi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rxbktrtg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qkqaqnor.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xgpgwavd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lfjdoodo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ubmhlldz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3unfupoin.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gnxsovtw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3irpjjxgo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tnloisly.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ykuwxqrt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ziyluldy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3uehezjxd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xnrcgysz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3paavcvzq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lxyqrfke.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3bcwhvwvp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xjokuzhi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ntnuxlew.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hpqalfmj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ybmiimoy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ackabcpt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dvjijkct.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fofqoquw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yqqvjndp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wqelyjrc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ythcuhgg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fgrmocnc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ufixegge.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3riuatvoh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scqphdpj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ynhxjrzn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vpgsghdr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wyabzetv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryykibza.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ltjylxxy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mlnvcftt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qqzxnghb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3buiwampb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3manixpbw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krhcbbjs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kosgrney.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mviavblx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxndubxz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3dlimpwyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qirvetqs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mabkegrw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rcwvffki.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ywqfyfwf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bxtriuth.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lystktlh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aesiofcw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rmmecrne.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3phmeqafp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iczgqdiu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3abqeanme.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xtlaxsem.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hwqekrlk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rxzgvzoa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mnvnwfcn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ynhvtndz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3adnoozrt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3bptpvfsf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3foacpmjp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3sbfzipol.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bxmycweh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vdlbzszn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmximosu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nxmimzia.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bnzokjym.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ykimhskn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lgettcii.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbiaeorx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvgudwgz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3wgmwkvai.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mrimlnav.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3swoozgbx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yjpxkmdk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hespipyx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fwknbkwp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ireiosua.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3otxctznk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uqivvvga.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vjddxgfe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sbimvyyy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lgmucdfv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mxdzuguv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hfjfwbwc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aetsujpa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3klzgvtsj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jiyqglun.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vbsaypwj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ydemriuu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cgvmravm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xqidonfp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3afzpneja.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zsfuhjdw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmwwmtm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3oysdosxt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3onubxohr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qohgjprm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qlwunbgu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3egojckvp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xfshnakd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdltizx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ecakbtzl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rycpuzys.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jptgnnlw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wguryhvm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ooajmrwi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cspuzzpv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkrfcpaf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3euokngtp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xbszietg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3redohdtv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lqdyxwqg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vcogqllf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iylxymli.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dhxycryn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3viwrgtnr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3grjqopou.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxuzceq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktkykspn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rsyfugqs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3buuexzzf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ridcdvxc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3afzjdjiy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yebymeas.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3orshcljs.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ixlheewl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3izndrbue.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ompzmdmf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3loqqlecb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3caeftxng.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wxivuetp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fpyhport.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3trpewcnj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3yknufmny.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3godswmrt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qkxgmasf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xopgcjmb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ssibfakt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3znywxnih.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gqejuipx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsrbdi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zzotidbw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3wavsbgzq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3enkvuulg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qxhyualz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wqinnqod.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nykaijfg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3itytbohl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fhbqxyav.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fphynxjd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3esnlyuwy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ldwotryu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tpmxzdpc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3olhbzonn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kyodoena.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lrovvdov.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dlytgnym.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hpjohkrt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dlrgfzbi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3okvsgalm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xjelbmdx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zexopjlm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fxhyfein.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eoeslzhz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3supgtzxz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yuigonfc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3esqowhuh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pqwqewft.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jqpwgtyg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vwmajtgw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dcllkrfr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qxkrvein.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ffqrwwcw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fiduqovu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kehsyysu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xzexdemi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dpecwbwm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bnxnjkwq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xtkzhnph.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hdvbmdxg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fnhrsckz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qhjxgkuy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hrqnquoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3utgziuou.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xzoglxbu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vyzthzjo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnwqjm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trsatvcq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dzqbwxmt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vyoerqza.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pguriyhf.html


<!-- 参考信息 -->