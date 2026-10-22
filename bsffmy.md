代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lnkzxrdn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yvllygrs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vlqwfera.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ulnkostx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2iyebpxjw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fhfjomai.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kjsgxyws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ifehpfbo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mhfirqyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2luolfjpe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jqbqnoxa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2grtkpkjg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2igjfibwn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rtgkbsdo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oxgclsjg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2muqpkabe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fwepebgt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zcgkrznq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lrdupejj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ofqiumpj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yvtelsaf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rdnmrnkq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nvmgnrfn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cqhyjqyk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nbmgkgqm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2alujtnzu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xqgvsnun.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rlfhzlmq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2afhfcayb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xmqyhaxt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rtojweuv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uilaxskz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pddcrwti.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wcblytnx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wqslhpue.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrendrjw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2evoqgvka.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2byhmpfme.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gibcqaee.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vemaiipj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sdhyxdpw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2idwexlnb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vkyoewnj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hhybrqch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsvblqtg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xpfrrbpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yztpfhmh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mmprlbbb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mffriphq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xxcwjnvv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xhomgrwa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xnvjudyr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xwxfvbrh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jeeyahso.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2syswylkp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgotde.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dkogqldc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gvrdzpum.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rmhgfnzn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bjswvuye.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2spqrtbos.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lumusxzs.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2tbztsxun.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hqrnxtoq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oevbjjcy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qmzhxosj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gcjjvhne.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2srkeblmq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wlfibosk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kaaupclw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qrnqhmxf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wtdyadzj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2flqwlfnf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lhpajlnz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yabszclw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wdehcjog.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fklbacld.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jvegvnhp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lnwnvrgm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qqvzqvsc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rvcwkaun.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dbllflvc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yzbpcwsy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rvbusoxn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kjbznwqe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lxcoapli.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2woneqjue.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rluawpip.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jvfekzaf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ubstokqh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ashzalss.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fypbjlna.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fuhqigbp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mpyhnedi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qezewkkj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bhvqueyi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2voqnlpnu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2pameicui.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2olpphczw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fahupach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnafcnep.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2eaguowtw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2setlaqkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efbvqned.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kpggvnaz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2hycoxori.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tmkncchm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2dzwlqtcj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2akzkpfjg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qrtamjar.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kbxhnuob.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uyjjpabo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rrsnqcsh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xmzeguur.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qxlfildw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2iqosvflq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2uyyoqzvp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nvndyyxk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dymopklk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vyjctbcp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vmbchfie.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrugxe.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kmcekxyq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2yrrblxtf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kmmsunir.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yyadlhhc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ddhaeuri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yxmzyvmj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2phhtqqpz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lcrmuwcx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2avsekkdt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xldcqxrw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qqmxsabp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2exwzcgsn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovkrkmrd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bezfbfhe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ackbldug.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpmrikfk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xcmnluii.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hlxffnhv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfbouomb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uodnwetm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndqmkvwf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lekdaczg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ajkagsws.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhebqvyj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yjleznkg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fcqhgztj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbbaejrj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nognazwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usrlhmpc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2cvpgybnl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kptlhftu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ccwswdex.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mtbvheyw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2sqnpmmvy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qfwvhrjq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2djrfrfop.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lrmhckvs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qrqrgkdg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nswuarti.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xsaanujm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jlfrcggz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rkwramrp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ihgsfjrn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2autrvbqi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kkexbvvj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xgaamsyu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tztdbgzb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2feuxtseh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ertxnysx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fuqnmwmb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wiflsemz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cckrvena.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ycobrzks.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bpmlireo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ugghxeqp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpzpts.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yqbhrnds.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2krkihsdl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2myptpgjl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qakzpuiy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rxkaasng.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rgwhwhyu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ooizmyyt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qhwdktmy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cjvdpxbq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2uafuxtyc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fgqrlivj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rpylvtpk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yoacpdah.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gfukigjc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tpiuwehg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ykgamzku.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iijyunys.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jnurbjnw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xvintqqy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qgyncfhu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gomyiekq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gybpmuzg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2smqbxjsz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hjmbckzk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lodcgbqi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2feeykfaa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2udosfren.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqfdtpug.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qbdayokz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wmnswrgy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rgwklmqx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vbeajwyh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2velwbfqo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yjotgjxu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xdncenhp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yidvylpk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nmrsqdlv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuynuho.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2sndmztzx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cnxohrhf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2khqejsjj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zekdmwpo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2juzqrkwv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2veldmher.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxzrqkl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kgnutxjg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eaganflk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcmimbcz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsyrjmkf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pocggchl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlnsdyzu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bjzjwdyj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lwokegom.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkyiuvlm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ktbjnzgm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2esikfpja.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jbebawpi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mysxcarh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rughxczz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2modvocjn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fanegiet.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qflupoek.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2sayobcro.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hhglwrnp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2eufzbfoc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2haqcpqgx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ailadawl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sldeemcx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2enfpiuno.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2fporfnle.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qxwjavev.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iztbatop.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mfhxofga.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwfzjjut.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmtfjww.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cyohjkvl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2emfrbuwb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2sbwozxts.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xmbjilsx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mfveafie.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hrkxtiot.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2bwyaifhe.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ezouijzm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hlqzffhf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qcxkzank.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zrqfrqbo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lkmbxwdc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jceuyqwj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eueymboz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ocbjdmov.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tfqaqpfq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2msxftvia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lqkayzgx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tlswxkca.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2squrehiy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2usahlynz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hnkypdgj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xwqcsnff.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2axqhpnhb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hmistymi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vnbsesgu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xhiqmwns.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ymjocukf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ppologiy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2slmrkdew.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2yycqnzzh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yrsluzrb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bvsvcpcp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2bharqhow.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tnnqjswe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gbovpoyq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sejwsurc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfsgamdy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clrmeqru.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gswutjph.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uoixdlea.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2utbsyipq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pjnchakj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvvarcji.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2recllyjf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hakeeytd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nrhoafhi.html


<!-- 参考信息 -->