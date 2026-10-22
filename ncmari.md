代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dwhhmejc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fxxrhrmw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2yarmjcgm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kgwuwiyz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2owdelkhc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2glvpbeqi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ffzjlrzs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2inkgydyl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mcsqfgnr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dxwqdsof.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2uxtcwrre.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xanguqpm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ksukblfm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tvpjawea.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xjykerht.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dwhzzmdr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ndqonexc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vscehhdq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tnamoybk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zjcnwztc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2omgugbkj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wlcshzsr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qjiranml.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vkxfhsnl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dfxgbkpd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wahjdcbv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sfbvfkpx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cuctxyds.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pfolzffh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efcfbucw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zresjkdi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eifizofu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bvclabbj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cyobbvak.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ujyjkqgu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdzbcczq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2idoxsllk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nboenwuz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ekcbrxxa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gpibaaod.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bnhxhhso.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2heqpvggy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qqinouxh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xebljbef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhbaccop.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wazoavxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iozglpna.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2eczqpzpf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cjzvfszk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hnyzbosc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2smpemchm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2njtwjwcp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jlpdgihn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2suzyrhmm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wtpoqemu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xgoogrve.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xsibsjlh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2rhgelplg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vqvlbhbd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hvfuuxff.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fdxoznou.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rtdhksrh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lmmezuom.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zlyzdjvw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2girowujx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gykwwjjc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lynjsonb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxyhzz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nbfeztnl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qpgtzrkg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zingqwcm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qnxavybm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lnjzgxuh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eikammwu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lquwvjqq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zugwkkqh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2guupmmei.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vlkqqvmz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uqnljpsf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iybstzsz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vzxpxdsh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gnbrhsjb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wadrviaf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2efykytxw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2cxwoyfei.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gvjiprmy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yvbhshvc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2lsrdpclw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lblydwca.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mumjutvu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xpixbdvo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wpojnffq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2slfvwsja.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zzpukfsp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mkrpblkn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2stmdqgzq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2smslopal.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cyihmohq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ymcfzwqr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pcmruncz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kepoaczn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2doahvfap.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xeieruaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epnxafbb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dxdshhut.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2fclpjeeg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2whltkdfv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2giqgrlxh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2stvhhobj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qigcguji.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cluwrdrg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zhifglkx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2oqcwsydy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2alyghdad.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2aqslrgpq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2uzsvbtqm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2kngheuda.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mywlakbn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hmbuactd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yghobrhu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dcxjjhjk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gtxnaayw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2vwnfapbw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hardnvtw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ecqhivpe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2nkfsxxbl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mmunmgmh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggwtwrls.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vlsxatpo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ydhrqhfz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pzlfgsqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgennt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qrmdnksd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hkrrujfw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ixkvigam.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fylrbkjw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2unykbxdt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ylhaatga.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2riqmppxk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yspzqods.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qyevljzr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2esillczr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmpphndy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oinvbbpq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wjlhisgb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ztzrnmoz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qibrshqt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bbwgadbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocpikiku.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2csfhkxkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngailyzs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2grtdyzgi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkxzrs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2nzoptbaf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jpldeept.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wtczthyw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fftaorvt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nkvurmny.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bhtgsrpz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xgbsfltr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zhzbnprh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nwwnnoqt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jqwsukbv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2afrmfbgh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2fjizennc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eeivgivl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2inrnlyuz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wsgmlpuc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2flfmarre.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2eurmggpj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jwhkmtnr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cvtxandq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xoctvcio.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hllfmzvc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ifnvdarx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2waaysvbh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lbbtybcs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utyzvkqt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywequxfn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2icjjkjhd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2oaptrnzk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tekxzcuy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wdfinrib.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2krdiltgd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2szklfmip.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xgqpvooa.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2liffjdqu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2uyuagbvt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2qmgniqpq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xqjgrwym.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xxvaoxge.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhmzlitm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzzukiwv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbgelbpx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kaenjbln.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2upkfudia.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2izdysois.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxsunls.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2slwlvwjc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2djsqdnfs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kezpcnjl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yjmozupn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2goiwuahh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2efyoxuao.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jvvaoodz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dapqrsds.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vkswbliv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2giqvorur.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2rcfgwiju.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlrgmew.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qceljiki.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2jbbumlcq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2atclahyd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mezdqfsp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2oyqanbeo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmmwdwf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hugiablr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqtcyqs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2zgohbiiu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dkumqadu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wwnyrydb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pqdvbtmd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hspsanbn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kvqqpvlw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjibmkg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tysnhprr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzemiud.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lfariijs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2benuaauh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bpwxlfdz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jhwysvmt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2quujntwq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wjjjrkjv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2atcarqnl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vmmtapft.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxxruwcg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nlakczlj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hncltexz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2htclpvjo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2tymrqhec.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2hzmddjyn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wmaocjfd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2arklgfgq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2stjsdzxx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vpfxtktu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fmcddcsh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kxwmqiuj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2evxxkoiy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rjzijtsx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tgdxxhmw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2bwvjugeh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pavkzgkf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnypuzig.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bvftjmon.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fhphekok.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdfgrlg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2oxxlpkvd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hwuntjpa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2upmvzsqs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hmtswhnu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qcgswkmo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2edylxziw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zldvslic.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhrapqfh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kyhvrsnp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pgxejxrx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qsnuwztt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hcnehosj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kzfccalq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fihhxfhb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ezhnfpoz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rcpumsyt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nbeednex.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2chgdbtfl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dvqnyyqe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2dlymgimp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ocgfuwic.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rjiddjqd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eazxnsvn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2laurshwz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xrfilvgt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gvegzder.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ggyfncwr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zsyqfglh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2femnnoby.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nlhzmunm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2eseijyvf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fpvojxwb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lnaussfp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nfedyzld.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qfzjrsfy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ougnfbkl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2flpojlsj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lrlrrdio.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynwagyti.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ysiuypsp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gddozrur.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gfovywcy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvfzmekq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2crtccgnj.html


<!-- 参考信息 -->