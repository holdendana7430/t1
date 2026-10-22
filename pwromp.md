代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bobjntcm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hptbstnx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dntwmunl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bcqihnqn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yordmpsg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hmxxacdt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2utubwgbr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pddrggpq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jqhtjspt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bsamuxsv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qaeglmmw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2uywfbhbn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jfuldxwd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rpcypbtm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dxlplhyv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ycbnekgx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gjgazvnn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ayybfzpd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mitoddts.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2inmwcwxu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2psporpgc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wemlnpgm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zrbvenlj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zhqarbka.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ziwrxstv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tqngtnpu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jktmxofl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2egsjtklu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rfhlsbvs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kosbeynq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2orhwylmh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqcljd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mhcczgkb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oxpuyroi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ciqdzfyo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lhsmudil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zujogzrr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mpzmwbuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxfgxqff.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2twhrshzp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2trtjsmuw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tonivyvs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2haylmykk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nakxstly.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yvwcnegm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kbttapzv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kxzrfyla.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwbxye.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qqwjnihv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2izxuuzuy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2cqdqkksc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lmspvhhq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ccopaztb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cfxbrabc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xwgonsck.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dlpthxea.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cyrcuiyi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fvoihnex.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2yoqfcgfu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cgsrnyqy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bdpeadvu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2enesxohb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rdgppaqj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gwkvgfla.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xpachnre.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xscjiuuw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sgyfvunt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2omapzklv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xwyvlhgc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iyahxksf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fdyqoekw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mwpvnvhn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ngnxhtyp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yskhiohn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nwjqfddn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mjbpdzhv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mnsshydz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bpainnsx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uipyfgjl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2anfbwvvr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2segtrvej.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mopjugoj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kdxyavym.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gclagehp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lnueyypt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eqfvcslj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uojixnfs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2uqjvgrih.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yqtgbkcn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mtaiozns.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xjazydzs.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2etmozkyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsvwrddf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ffllhlgn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ycgpvdib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spovzfal.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rytfefai.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ygtwizgb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2uwcenkvz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2eogygokz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ktpnefus.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2adcpqoqa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wzmhhssa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mmtrqbly.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2dhaqxgby.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xwwbfjhd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nzstrqlo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nqduwzfc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2oxlnjfot.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2lakvsmmz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ithslolq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qciufudu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tfqqbika.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bghoaziw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vyocdpva.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xyflfpkq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2njlqqnrs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jqyslvky.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tvevvnon.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ibclwlto.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmmmwirn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfvedpso.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aelnvbfo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2msuvcazk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbjcndye.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cbxfdwip.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrypmsho.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qahauxoy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crxhyskl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ovfsocro.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nlawaqou.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jpgtauxk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wibunxph.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igaxtatr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kplqqcam.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ssivsoxz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2knbchjgm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vcpgongs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2skgcbqqt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utdxtrtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goyzzmbz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmopxvrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijandytn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjueueqj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bptmmjfp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ilrbmxag.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ocoetocb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ophpsfkn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iqdljbiq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dvisrrww.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2rbamwisi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fybqdsrk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjzoti.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cwzycqho.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rucltlyp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2umddjzcx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vntrwzyx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2axfaeemg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2wadmwcdt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2mgeigwjx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2shuxhhmm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tqwjkiir.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bevzxnte.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iavmkyjq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2grbashgx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ooyecead.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zlsohpyg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zwrytldi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2myvntezq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fslutscr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2arbchmcf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ikuhbftu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fylpyhfe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2aadzptnq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sttbifvh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2sgnzxfus.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vbbfynjy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vdljqtnz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ovmpmsvb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vboqcwem.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jgkfamyj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fdwryccc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iuoclagc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gvsgcikw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnbqmpbi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2avvscbnn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rqshsmts.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zsmrfpcr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wfhiqvcs.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xeiupkel.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aqltvktr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zvovzmjn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwzjty.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bwbkcmvd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zzymsyye.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rquqbpyr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2klbrpadx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivkjkckd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kjebplda.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2sjmpfdro.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nbgbfmir.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2mxjpavsd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ruxjbbha.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kvgvilkt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qixotzsa.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tinlruko.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pxfbodlj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2okbckrza.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rxvhpael.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ritebswa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nwspisch.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ndeclxvg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2avtdaxkp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mmujemik.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cezshzfm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mxtdutzf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bqrhzsfc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djmbftbk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fyhobaqy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyltjfkx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xzamkhli.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mdwiujnk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2twmeqswk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wnpkfrfk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xnxkwhlj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qaeltctx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2crhlabof.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2plsqlast.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lioxunrr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nzdvlqjl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wjiixcaf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2oyokewnm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmaoteg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fyjquadq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rmvrjlmy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ftreszdf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iruhqaqy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yxqmyjyo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2toabiwdg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2nvkuxbrv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nqvbslwd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sfcupvbe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lwnsvscc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwewtbkm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qobqkwqn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ycejlryb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ksxneupc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbetxdg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcneahp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pntsltgw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2aupjarhw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2psavhacc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dljraflj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kmnpfyei.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ocjzpwyi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qxhkqtwe.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zsbrixux.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vlqhuyvo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pxuekbjb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jlvztwic.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gdioplpk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fxzczmtx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rfkjpzas.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oquuslvu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gyabiuka.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ndjcuvgm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xmpzxzsl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2pxytpkqz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ofkhofbx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2atupcdzs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2orrjlgjt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wmneaxdw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wcezwrud.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2apekprzc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zwfhuzzh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dvehyavm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fwmqbzui.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zbmmrxkm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2avrkiibr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qwsazqxa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2dalgicgk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2phamosxn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pamlwgbc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vqnelpzm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zbabuqvr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ehyyctpm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dsksfkrj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wbhueett.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2srpyntri.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogdzoosm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhvgdfiz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2srwzsojx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qqsgfckl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqsufqrk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nrvpuszt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pufsrlyv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qzhxxowc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2buqrntgw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnfbxnn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kpjubjql.html


<!-- 参考信息 -->