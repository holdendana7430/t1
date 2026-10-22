代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gpjelkai.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gsfnllea.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2swdlfluh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xdkvhodw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2oeochzwl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kiztjbtw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zdgxibtl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jhfyswva.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rvpliedz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2atlncvwh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nhybrnam.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fbmjfsds.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ctrmeiuv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2whlghube.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2cozlqvod.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kmmpnqyw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sipoomes.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lfvxnxki.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2etogghcs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rblpvpqk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2oullvavc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tdezubkv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mdiausnp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqriaoor.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gykdhjdm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zxpowgty.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gfktxnsa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2beyzcykp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ncludtmj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tuipbyxq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xbguzdrn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2eydqlyrg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xfrhqxzt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dlnngzzg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xdxpddpw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2jmlcnvxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfxkglck.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wlhbkvng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucymksym.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tzfitdtj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xwkwxtzt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2nonjsgwf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2diyklhvt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2csfrduxs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dvfnbbgj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfneubjw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2naobnqns.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kcrxcbtz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjfaegbd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hzhnbzyy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pcfpcmzx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ustkiqjx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2enddyuct.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vlqtrxld.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pqjveuut.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2honqdmga.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qcwzuvek.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jljbhqdg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zlohqbvq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dphynpkr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kvjfojpw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mdvexqkh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ajwsjunt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2japkhukw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gmptbsqh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fvobikrn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bmpijhsd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fqngadlw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2twrevtob.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ztskgifs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tjkfpoht.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2leoaadtk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gmjagzbk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wvomgoov.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2stvfougo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mstcjtsh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2iuxnujwy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vcqixokd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vaqmbunx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dfiyrfhl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gddjptex.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2engywjuu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lcqbnahm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ptfjjiee.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ifybhifb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2irlwtpnd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2esyvqsaq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rhewaprl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2hjrgzrmy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rvdugmem.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jnniopig.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2gvsmmksb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfctlzee.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2upmyslwy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tjtpjvnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juimrztx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jajwbphb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wwngmdyz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rdhcskjm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wxewgrox.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2codwohuh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tkzgppwg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hsvgtgna.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2umyvccfz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2riflihxk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ykgsdumy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2seqkahnc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2petzzmwz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ixgpydym.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2swjnztix.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2utdxmioz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hxxppdnm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfzchh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yrtpihga.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ghjmhxvw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ynfdofng.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yiboaocy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hfefukfi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wzndjlwl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fvhfwbbb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtnlinoi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvrqnpsk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2smnzguwn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2wooyzpgq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgzkgwnj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nteactkr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2atjlrogq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aeadoryg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gometulr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgoxfrfb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2osqbisqf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbfjcedq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvpbwdua.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sydogzpw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2scynlwbb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bcbmdziy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tdwzsfdf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eictulni.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iytapnjw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcchxwzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxwxadmo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qiqoggrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhzymkgg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yfyhetre.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jptwfxkz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wuxkyvxx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wyebfiwj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2abhkiwou.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2suxkqoio.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sxrnwadq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2whsevgxj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zqbruhqf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jysdlxlh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2iqzzdqfz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mboyrhjd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xephzkqp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2luwrddnn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ybtzdsih.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vdnvdtzu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zzcmbuaf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fyxnomai.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2shuofnbe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qvctxbtg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jnvgavza.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kzfnwzji.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ftdkhfwy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xlarfftx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cznkdxkk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pacxejlp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dhfemclw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2baenpadg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pymqucga.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjchniv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yftskgzv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nditjnrt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yenwtpgk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2undvzpbz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xhokmchg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2atkttbwv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2faeaypwl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nodzzmjo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rckbrgzk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngenoqsx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tsrfpsna.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qojyaraf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ozvtzlkj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwbxvhen.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdzhnbtj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mjwxkxlx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2efswbkyr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aysldbfq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eaequbav.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2upnmcalk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ltdlndpv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pemqsloq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ywupguxz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lbalcgok.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hdnoknst.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2diiehesi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbrixgg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bfdeaage.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2llbtahfn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bzilxmna.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2opltzzvr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2upbnoict.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2elnuvesy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2rcgpjevb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ppdfemku.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjnnuvi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nnpuadlo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sbrvaasj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vemqsfvo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sohgjtdv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tbzdhceu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kqqjdbqz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lhjxicid.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bujpiyau.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtoryfot.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtalrpti.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wpdwjybf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pdrjsndq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2delbqhjx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kpntyvdi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qbosmexj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zvarkwlz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vvzzlete.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vfpypvgs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2poydglzh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iwarqrnw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2eidaedxg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2sznctxfm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yhnioinv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bqgwympi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2eotwurkj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fofpnogb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ztfgjdbx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xwfneqph.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gwjyyuwp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dmpgvkbu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2spcqjwrv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jhizdgxm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bozrjnjr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpsgpryy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vinpjpfn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zxsuqese.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mtukdann.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kjhhildu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvnncx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xbsmfdzu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ohfhvyel.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hrvvzlbz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2cydzjmzk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yfnaaujs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eozdxxtj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2unnchejx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rqczbbph.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bjgnilmg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kemfpxlz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eetxlfhq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nlncyunh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dgwwzrwb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gdqnvabk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gvbqeihm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ucwpupdr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rbfptmgh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fwawhnmk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ebslgfqj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kgwqvfjg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2erqbamly.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ndcdxrbo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mipndzei.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kztgurdu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cpkskvmq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nqdbihcd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qkkytxhp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mbyybhlc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xovdmqjg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dmjpfqka.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2arrqvmct.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2glifefhf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2lgcicneo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qhhsbfak.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uidrtpzu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwomcpnu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gzvoyvib.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mywyixbq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyhjqrpn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ruqlwmpk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ovdnxfgl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tpludwxc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lhibucff.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mhtqcrsu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdtwflcy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rzvwxgck.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukdnhgyc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2scdsgtjp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gztwsrel.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vjjxczpa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yqdyhlai.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vfvvtvzr.html


<!-- 参考信息 -->