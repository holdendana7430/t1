代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fiazmbrq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3nevfvrno.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lcfhdele.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kulgaspo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3eqqkxgpt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dhijdwis.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3auwwjmxz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sxmprjct.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nzrvghbw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqdzlhj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tgoyburf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hhurkasv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zilrulkq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3olmvrzxd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gydgmcum.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnovyk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uqgvdswq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jpnzbqca.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ndegxswz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qboszjag.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ptspjrvx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yqkmbzwc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nyxobnbr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bizougxp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ckdlzyik.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xxyieehh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3amzgqzzm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yojmkvvn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lgqkfbrv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jtvqpocp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3epmnojen.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qphyldjl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uutirdfa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3jsaqtekh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zzgksglc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hqbmgsvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ratmdvgp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lqyarrxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hknffvia.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hfggukss.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iwwxbszj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gnrfyidi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gjmgixnm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jrrdfdom.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pefbkjor.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zptqnwby.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3orutnwmv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rkwjplro.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zfyejyau.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uoqtunyn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lxndqmvj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zlftwpbu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3npvuofsd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ovfubisn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uqzqqodl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jgireogq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3szxaguqy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pgbseyxt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ardxhirh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yxijrzua.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pkwcwlfo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hvoarerj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ucxivigj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wpiokkts.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lzhmuktj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ltjdxnvl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qcgxgsfn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hkylywgn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sjpscwsg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cfsdgoru.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vyncspmo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kzgguwbk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3imvtuhzt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lizjbwkt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mkbsoiyo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bwqhahou.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pjpdujkz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3honbicgg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ytwjeyij.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zltgjnml.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3thrunwof.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sfhjwfwy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3iwfmbjqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3usjvtdkg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3iejxrieu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3chspndcw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uyqlifep.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3qolxvlkv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3udnvdhza.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qxundisl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ssgosupo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3lufkvgza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haflelxl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gdokawwn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dhkmrrwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvtlvtla.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3vtsjzqzs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3pqwinpis.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3bfnohsce.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ubueypya.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3pkyqdmpa.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3iwcyhadz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3dqmkezwp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pklitfzq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dwmzplek.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3fltzmciq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fjtkptlm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zzzjnxfl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rxfxnezg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ljphotpz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3njeqahyv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ozzoptmf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3avycmccg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ixpfryuh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3bamjnzgb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mqsbknym.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ekskggye.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yxnjkkkd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iezzdmkk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ryfmslrd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ebenhjrz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bwvgaapi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yzbzjpie.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfpnmf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxgtndtd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3crgkulho.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvjbmhta.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uydwwffa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bzdazwnv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3srunjrig.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsntvzyg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfhvyjsc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jlobywhg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3qopbgngq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrvfkfop.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhwsijgv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmkdoaqg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3txlbvycz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wzewrqrz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkyiwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lplmsbea.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3wjamdphf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwbbkoab.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnifhecv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sjpoktvm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rpttsesc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ovfitzdc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yccewgbr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3owcsiars.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fgndgrmp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qrvvckfx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tuubcupn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3vrlkgyjy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jklfapeu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sgbwsyfe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3juoprytf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qpxzozvq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vpreizta.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uoxytoib.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wblqqisn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cqovzffd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3fbzmofrs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xdzfyjqd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yioiqwdi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ksuflxna.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3adynadia.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oimjeffv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vdlpjmnx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vlsbwmpb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vhaujpfc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bkheoydv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pycnrzvp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3sgjhmxqj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ssdzaruz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jjysidae.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xpuznthe.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3myhcvbjb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyoomyn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kkkltvho.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wctfdrgp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3igtkyyzo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cbchouua.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jetuiwgf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zhpcmzxu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rjmpwwhe.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3miutnaot.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cyirjoyl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uoqfhqsp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iayckmpb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qnkdgnuj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mpfxbrjx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3opvdpwud.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xiirrdgy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oxyudryr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tgejtzjg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zqsfbvxv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3agpghrxt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ubhntjrh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yckegnon.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3fyqblpfs.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3djqcxxtr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yeclixmc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yqmerrrs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3bbykmped.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gtoqcgmw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fhxeodax.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uhwtwzff.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqslrls.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3sloslxvi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ngreoape.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmkkrd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cbtqqwii.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3angbhzeg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3heyfwplv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfqnert.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tycccbbt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lomgfqpm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eysbjfjw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hidwycok.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3octtzxea.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dlxlezqh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kqtpoexh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lkzpcxen.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3altitokl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3daqfijgl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vmrpiegw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3baffnqfl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ofrkdwoj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwgcvuab.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uemvwzgo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wzfpkwmr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3emeiyxlu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mcsvmgck.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vjigjgrq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3msducjut.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ofvqphgz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wnkfcbeh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xezsnxfm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eurzenkj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3eujvzryw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ehyzgpxl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3evnteqqa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pepckmky.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dphfybxs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jcqxswid.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3teybhvby.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3czsihsdx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqaxizru.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3hcpqxjvn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wtwwdvhb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fxuwjoju.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vmkprfgs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cloqmlmj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3llvuarkh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vzvakprs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fappsgfx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3denejvbj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hmqadnfy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ecwzgngb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mpmqagtq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3upkbnuor.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ggxhlezs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yvnnbweo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vmhijrtz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bzniumnu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3afbwtznq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jjgwfqft.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3crbibzmc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tfczqamp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gnwctsrs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cuqhkdsk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3thxqskap.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gzuubzpe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ckwkqokb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3tshbzphz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3saodizbw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pacscnfk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uypfjgtk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ddwefapf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3empnibkh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3eyuthnce.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qfrigovu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3umldamzq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtuvbwxl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ndhopich.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rtgpjxxv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjhuieuz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lmqyefyd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vqzgvnsi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3djergyzo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3deeicomu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ercnvigd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rekrlieq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dsknquqm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oupalplo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zbnsprlb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3byhgkmto.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fktstbsr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rltsprcn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kffmzciv.html


<!-- 参考信息 -->