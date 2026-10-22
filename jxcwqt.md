代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2yamrgmta.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jqffyixz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wyjmkkfr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2btnuurcj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bzwqupmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2defosztb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lrstklyn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gsnhwmdm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kjotfbhk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gajrchjx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mkyiepkr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2absumvvq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2coxnnyrf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jxpbrfnz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2iyguoymk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xuoyjkem.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ueagoahq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vbzolnxk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kerbgeyi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcmewzb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2lopnppgy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zdljeril.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lgmwehug.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jrnjnwcy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oyjfpzzm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xwfvgcbm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2niffibvz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqeguxom.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ovggilgb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2obmrvkza.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2izjdcznq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rhdqrhzb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2raqylbiw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vrqwafwy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ozsqmnbm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2seazdlpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbqhdird.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nxkglqyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knnnfrim.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2upnagpvb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yhepchry.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2eaofjbkc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mfxvlulc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ryorhxsi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tpsgswsv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kdxumufa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qkcacqco.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bprmvcno.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xytssyin.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yxqbxxxv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2smbaxkcp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tvilknyr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fdrfnluv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jhfqibpo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mpjpfszy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfasex.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2nnekfmdi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gsckngpr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xsumjfpw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rsslgpzm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qlnsdyua.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2okiaymeh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2femofhvx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vqjuesqz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ptlltdfd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tclxwxgd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wowczlrw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rohhfqvt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jnbfvovs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vtwthqkh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kctuicyf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fbyeqtku.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qnltestr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fnganzar.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vabntfvx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afvcaofy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dbjyctku.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2cbhysmop.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ytqtzjky.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jznczdiy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mouktmia.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2efzfosog.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dsdaetqn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ewiblbfk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tuhjwqnv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ykizhzxx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2oigghfpw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mgzvwqjx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yxojyxej.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qxdpulpo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wlaltwwo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ntpbntju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlleowpu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2odczhbzn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qxlvsnfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wutymnhd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kymwexkq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wnrldpnu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rvthywao.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2pzyqwues.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qspglzou.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xcbkswfb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rxnzxzxw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lzzunkzd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2swxigetz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cjjympmq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jyvtozqw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vgqphoaw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2umbsbrjr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tmpuefzh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ywhljhmu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqdnez.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dslpnptx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ryzfaqok.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rnnknxji.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rhbtjwiz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2umigoyrc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2bfhqdhed.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ajtmlzfm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxftstpn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnejcngs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lkzwxink.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wfcdobuj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcpgoxtj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dxzwjvjp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqvnulyo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xuvabznt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwcowfro.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqmpdopy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdvwnqmx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvsnsrwx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlefnicz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2krbarntx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2tgbbcmgt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zviknnfo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2deprbzpm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mzbcbdob.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfvjpgma.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2urstikhw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxzltlwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hexqeajq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wcrwfdwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoexsspm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdoavfdt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fchonsev.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2megdgwii.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gymhvhml.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pxiqhddu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eapaafmc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uqgrjazy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xyjonotm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zbsuxmbw.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hmcjxkmh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fkptbufe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uofyfxqt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hubplubf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ffjjkunm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vfzmplkq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yczzsgyq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fixblwuv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uqplfdee.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hymrlmtk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ooypnnzg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nmrjdmof.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2krnvilog.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mhytuinf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hfhojxdh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2atmdnvtb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fxcobndn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nhcjkzad.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2irhcbexg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbkfjbd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2twgssaqf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uuewsymd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nfxwlhqm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cjmikruw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2woifazbp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xcbdlrto.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hulokxig.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kdywwsws.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2additeyf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rwthxinn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikfkhdtv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnfikuxw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kiqfpxar.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ltgrfxyl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oxeapcxr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2arwsqxop.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xhbkevot.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iiduioft.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dnsshofy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hxauuvua.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ppsaldlp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2imnweldv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxdehjc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2mixzgowj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2axjjdjjo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rtyuioxg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vyljrxxg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2uyeutkjk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2isxxwdyx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tgzbiiic.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzxqydr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xzgbepln.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2olohlpjr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kvdjqajp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iujzrtli.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skrzogta.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2eaimboxk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tetorgbx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bdraqibr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2emaltqkc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ntamkzib.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2bjmylqmr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dvmzgepk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2epmmqhdl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pamlvrvh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lwoooona.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxzpttq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fgarvpky.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2drjgauqd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vpbncghh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gjmyxhln.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xgkdhoas.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ocndahjk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2drsaaqdf.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zvpgalxt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2chdjuwap.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vjpwkljz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrbsowfi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kmyjuohy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xiqekjqq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2pxdndcfw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2uopeqzti.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2uqefusqj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pvlmrsia.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cdelngnc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mcmleokc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2elrmyghp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2lrswfguh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cmenflhd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2payqjvuk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2oqdzyvbt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rluxmzzi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rtamepyq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jfrxzjjt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rstqcrry.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2fhxnsdfd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tcjsncqi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xyxehppo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwwnyfej.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2idbtrknk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tfnavdwl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fyzwjmor.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fihkbqtr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzotjqkb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jopprunv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwhcwchh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oxvcujrk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjxrxdiq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xmoykxef.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ammazbst.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dhgfjdti.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2obrzdcev.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ropolswe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2pdztmtmf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vgfwnlvc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wruvmfxc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ibbfycbd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nomhkgje.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qangmrsu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2chmyrygs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kksixzrh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uaexvaij.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkxanw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jonksvuu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2alkmaqwr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fpuptjjk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kemgscrr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jjqqhrgk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2brvikzuo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qeatvtgm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ekwuqreb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggpcksdj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wfnyamis.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2tjfluegp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdoyjabu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xmwbnset.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ibvooimd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ckikjkwc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2egsotpjp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tzlhyqpw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hayqklkh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2scnjegsd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2snjezvay.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2keeudnkd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2aragltut.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eumteade.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2atlephqc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dbfvnrcx.html


<!-- 参考信息 -->