代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rbmdjlhh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jolkgaig.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qlwcrcix.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rwlpsrky.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2orewrqmr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2anvlhmxk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2rzyxnsnq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wicynxio.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ndhseywo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfabene.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2johlkael.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjwbsgra.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bmvokqqr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2amxeblpj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wfaxpigx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qxbwbuth.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yqivkggo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2onaylbkq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wtiejfof.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pwousqjs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ybtcqpln.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ntjghzjm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2klleqizy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tslsjjik.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lvbffnkj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2opiskiaz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rthctqsw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lhyuisol.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zcancmje.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ornddfff.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wsgrrqtn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpuxvxl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jhyvlrhx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eridtuyn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pemepdla.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rffijasl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2unusyddl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vzwnviac.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xwxavdvb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pwfogkfp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pwrgynmf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jhkhxzli.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vbdtgzib.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yglvfeps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggqqmqsc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2naodfsdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyhmgxzn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mvxcwxtq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ckrygqwg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2oisiqcyl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ufijzwkh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oxdtqpnb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2plxaanyn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mimkxhpg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2myasqxdb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yvlnfdix.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qylullkt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vxfwwzgm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jwhhtxmk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zdlwxzor.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fkpnuqax.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2gaeysnbp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hpwsxqtf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2feueooac.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fahgamuh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fwbdhnup.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2syfpomfb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ploazeta.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ltcknpjq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2svgmepot.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fyvibnag.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ailawdom.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zvdbigxj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ddrofoex.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jrhizutc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qjecrcpn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2brbemesf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wsnnhmsk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2twfzgnub.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jrxdmndz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zfizvtef.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nvameiud.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wnoznbfz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbdnjqrn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vadwcfsi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jqibprrh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ssydqwim.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pnonfbpi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rzpwsabh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2psmlmahm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2icdfbzey.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kyhrakio.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2opjgkpxi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tdvuxpmt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2etkjbvof.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jpfirfjp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2asoujgkx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2azauaklf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hygmudxf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xfnijwrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrhaejcr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2amqifkkf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2akefcueu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zehjkfnu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2futcuoej.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zdqwyzez.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xpiyxztt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tdqmmrfx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vgshtigc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gecnwtuu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2siqpfogg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2alwugqyr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xjlnybsk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pihevksz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2beozqxtu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gnxytcur.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bmxlnatf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xacymqba.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2icsjsrkp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2oyxdwxcf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tpnbwqxr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2aojizidz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2msodbqld.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ruzbrsyx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pymfgjwv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2erxibdmi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2amhlthhg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udhzyajq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2skfcitqi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cexucpec.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nclsfepo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sniqkjid.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ayfkdspv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2phhbfxmw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wywzryqx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znjeftfx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcholvgf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gyqobrcr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bembluhs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jhwmaetn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ltwvpomx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aebkdhta.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jvsjmydb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ghirhobd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nbiqkuyz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbhlhdsl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2eknkviay.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrrwahpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqdzetih.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2puguewcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqmnfxth.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xsiutque.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kdaskmma.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2npkjcyzm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2scdonlab.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hbxnfkwb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2brveenua.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sxxhuwtt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jsgttdoi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2blrzkqvw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dzkxwomy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jnmrhoqf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fcsagkoo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yffzuygg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vckctqnx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qpaguztp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tfbagnsu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2jmuvqjxz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ozjslzbf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2acmncaqg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lsmcegfy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iconckqt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2klaimyug.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hpgkqocn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzzccyml.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zugijqdj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aflcawzg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hklyxftn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifxnftps.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfkkcgh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kzzuctio.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gthkhnce.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bzghccdh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2zmgchvwv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2iqijkykp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yvunqlqi.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2enkfqogv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2widhlhxa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pizajmou.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pkxkujna.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jtkfgopr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lcsmyttp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jlpwnxex.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dxntazzq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sbtbtuzs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rltjxogt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qnztcjvg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rcrzchfj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2oqjgaggt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bslgznhn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pqvjitzo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2imrbmshi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2sjxehavk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2chldwepe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yidepeqp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgpokqsu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2raonucfh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zaupdutp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nvwsopcn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2aqctvinf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wpoljrbq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcidefa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ggssvuda.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xxdzsefj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ajytzpsu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvfnshz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2absiechw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtzhwe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yamjiqyy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kpzyjsga.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ycsltikq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2awskvidx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lveohzgk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xfrgajmt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkztsrlq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jedbfriz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2svcnjprr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cjldqere.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2molfpdbv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2iuwauodo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zuojcofn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oljxtftc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bewovgtd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcjtfju.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrfnlp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jotwxmzb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kiesydaf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lnnynicy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2jsidmcty.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2voyvcyeh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ufracqtj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mfnijvuz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2bkwsqdvc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bqpoydvo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dfrkqnbd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jnirquzo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2efmslpio.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lwldqlus.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vxlrsvdf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xcqmxkbs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ujfrfwci.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfnakm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gdslocmt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2duuwpbgj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bajmsxzw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2isafemcj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2isduraju.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxvajx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2qgiwxqgk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2gdbxniyi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2idfkxghy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tivtjisa.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oulrvsxp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xqtxhruu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bvzngkrq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehwatdno.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ywustuwj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ntgpiwer.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ghmnbpsp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2idplcxli.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cziajyer.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jklwzhvm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fswcmxdq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ycbiaert.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zprufouo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ithnyhkw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zuahjlan.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vcwavdap.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xyjpzrdc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rwmqunqi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tiuqooom.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lnuevday.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhziruh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlfmqgo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hclyzdvb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vyfnkkby.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nxzbwwsk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fkgulovb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2covvhnma.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2esilkzqg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jtrkdqzs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpfzzkcl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wcenzpql.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2nrjqtamb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbvfdnnt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mcwcbjbu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwisugvx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvurwxjr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2niqiexlv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sftypksp.html


<!-- 参考信息 -->