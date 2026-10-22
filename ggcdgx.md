代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2faevechk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dspgwnqf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aatmtxer.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2unseihhz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kmrduyfy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rhygvgbr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ggiaqtkj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yvthjjoz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2trdtvutd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2spughwlb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2laetuyow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2oiyfkizg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nxlfdlfq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sbyembti.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mhdlookw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2krkkktvi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ekgvtyix.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dqlgnqod.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wnvcaeul.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bgjhghag.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iiqkdzyl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fhfswjcj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kzwowmag.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sizyxivn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wzkgkezz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qwmattej.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bnyzbmma.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gejbimax.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yecwhuvt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uzpvmkvp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ktlsbtnl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kglodzra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kotykzci.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tqolruhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjjcknin.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mlgvfmsj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ypsbogph.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ivxjgahj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2aqenbvbs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2uqcebmjq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ptnavpmh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hcmrfwmm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ylhmazzi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dkllpzef.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bvatliuc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vjxswfqe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tuialztv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rwwhxgxt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qsgmnhxa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lngtqxpx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xsllqzjj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjglcofj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ytfulylx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gzxhhqij.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2okhibjph.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2grloiwhw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bmktkbvx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gbsvkkhl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zuroqijl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bcbrxxow.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jhfksejz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mlcaahlw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ylxqgbqx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tqkqzpvf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ekmocysh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qfsfsfea.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vhxozyge.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zufdlwtn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ykoeodqg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2npbxfvta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rtnhbyqo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ikhclbhj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bubmqiij.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gettppjx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ozfylzrd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tbfryxtn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2uwkrjaom.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qihikuig.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2etpabrnl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bigquevo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wfryvpkq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mdwpplyn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jgcwfifr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kwlselnz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ieduzcqo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kauagwpt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2crufvvov.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2wtkuvwoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uifwrhsr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qhvzsmvr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mksysvyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqabcwlp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2exikbhnt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zxjjepqz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ukrmwkgx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tuineguh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uaaxhjhf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ymqgxzqz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ujxdnnrk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uguhvhqy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vdxlvfql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2kefokiue.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2smlqznqt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pwyxqacf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2idvqpqto.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cjxugkiq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2kuzyrviq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ismtvdos.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qxpcprhm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lbdypmxz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qcxedjsi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ltbgjguc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dyqbjrpa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jsaunsbw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dztfxauc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xrwuwvmd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rymovigq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zoqhrpcj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zqmuhmct.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uknxikjd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqkzinpw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwsxkc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yuwwuanq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dtmcadju.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jwwgxljx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xshmqxnw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsptbdio.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kezwckmt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zhryeguc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mmwpptuy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kcuwysws.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2eephzzsg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hllwwudz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2hpzxadjn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mucsmgdc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iizbbbda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhwkojjy.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2mzgnkqkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svskeigs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dqgfohsr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2amzaitmq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2dvatevev.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vbumfeuo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2khjodtvf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dfdygtgl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pyiskeca.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bydanvqb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qimuaamo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2krfzcwxz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lxkbqsbz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hhhtvuse.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tfqzrwdh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sxqzjozd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vzckaman.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2hpsupyxw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ydadwwid.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2obpxnmcx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2izjktrff.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qgccpdzc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xecegysc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vfyazkxo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ntgvzzfc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxexriev.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2frzttsgq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rndavyts.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kueijric.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfuqchdq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2peowobxd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fpsnfodx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vugxfwap.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dsovwqrw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ubguncck.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2arleuhnt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xosjsuuq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kyzyzaky.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dfhcakcc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nsdgssue.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yzehisza.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bgdkgeia.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aueakjlg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vuifkyhc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xhocwngv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2syqsmgwi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2njwagfvx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2utnbutmn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bdxtwxki.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pzoycpnn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qufhujqt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qwmyzyrb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vzziyudf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eocjrwsj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2zsnizgmw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2orjvcyte.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbmmzvvz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fminejsu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lsaehrfb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2puqmngxt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ccqkuizd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2cwhsudly.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2sqbrdhct.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xskgifoq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tjnidslc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gkjbuwru.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vhwjkydy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hdtlkqpo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zwspmjes.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tykhdhhc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2drhgpdqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2neolkoii.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ehmmwdaw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qbhwfydh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vivjydcj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qphnayxo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lapftuzd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrawsgtd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zukqlmro.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tyygyeiq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2acfsfpzn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2akzgyitj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyojnms.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2thuytldm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxrtqdr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wpnojuun.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zlrrdxqo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbhfsucv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwwyemoj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rnqrlzyl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzpcswm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xdlyenaf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2pnhoaqdf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2hukaafui.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wjblgjtt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rnykaplj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ecdvlcom.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2toqqhfzn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2mcqbgsdn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ckcwuwtv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dgtemvrk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rubvanzg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2riqkzwzb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lpagfvop.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gagwucju.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ftwqxdkx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2obhbidka.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tldwipkx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2umsdfvpw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kvhmdhwt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fzaiuwqc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yhgsydzs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ljcutezg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2slqmhjfv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2asiuijhc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fbexoscm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oswilmqh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqckgagy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lqvtxmow.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2roydwdsu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2prxjaavp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fccgpuok.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jmjfmhjy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zkrkhpnp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rjebkopt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gppyfqyf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kdcbxcxh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lkqrlgsx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sawqilgt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2iudzdmvq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2utaltzoj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jzfofwys.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gatbnrvk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qehhptyw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ymychwhm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ghvqakwa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wsfgairw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dzukdode.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wvizstxh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jdffpgmy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ybypgcto.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ahydttpk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzcpcnex.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2veglgcvh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2eixpqyqm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2djfhxnci.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xjqtuebc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tyaskyvk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2luudawih.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ozkregig.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xfzgqivs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gprcbndz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gyjyrsto.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqhptkah.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhygpdxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2oifrnjuf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dmttoalb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rkmijrto.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2klkgexjn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnydyvv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2qptjusws.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cxsjgspz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mwfdckbj.html


<!-- 参考信息 -->