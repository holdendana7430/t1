代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3enselunz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3isdjkzgl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kgkonvfo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yrlzjxqz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zqigxmuq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jnwaybvo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ynojldfj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3abvwdhgt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3yefrvjhz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gzfxjqre.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uejorqjb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dlhmypnu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kutedapv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kqnkmxjl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dgibejje.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vpdxkhmw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gnazfekf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbaxqig.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3smtcplcw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qyeqjire.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nxwcrqnk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3innhqbun.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ljsryazo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qsmlxuyx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bobhcsor.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3asqywegm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uqpklnis.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dymglvlw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ghfuhbwx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jwzpbsgc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dkyamjhn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjlaqtig.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ydhzqrrb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3upyekkwl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vlzztvaa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ueyhcknx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3adumscfb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ryeywchd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3byklwgqx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3gastggpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfewcdbt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ukjxqsor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buhpfjft.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3flpwnjin.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mhvbkkbs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3slxtpmpt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xjqakquj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zhjqolbh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nelvrlqs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ffltqnhd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lxkzench.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rhbgfswe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gzwhimaq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3yzwywmlb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ernuaohn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oedsjrwy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gagxrlwq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aaczkemn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ixilngfm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3sywyqdsu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3axmgzfkv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3drzvdxre.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kcdknvuo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3lmvsjzty.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3witmdhmm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pptfplwh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3irihlhbv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hkwtqwhq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dvweqvai.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ypngtcfs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dqpbncqz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qenkrbhf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3odatmbrb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mbdmpfvx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xolwwxwf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zuwipaqn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dkovjggv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kocglyin.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jdaefwac.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3npbcnwxg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3izxpcxhb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ugkjtbqm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nktxnxoa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uxlxtvro.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3bwngrwzk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xulmkpze.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3linmidtl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qayhaoji.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3clnwuftf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zehyfgob.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nrahutkj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vkqgpejq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vvmufxpv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3sdnbigyb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wnmixqad.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3anizkhqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqluttgn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3axmywwgi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zufsgmud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmhexldn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xbkihiah.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ywevkcng.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wnqqupik.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fpsxvpha.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ppkonmlq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3yqwdlmrs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3babljwrc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xssjkbog.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3bdfppebi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jfbxewjc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bccwuhko.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rzmvxiys.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3lrqxhgbk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xzcsqjss.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3deaqetmj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qgkvgszn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3zrpmhwpw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3mmyijecd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hdgtrqdc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tzwsdqtv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uvqufgpv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3pyorptsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wircalbf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fkdguzxy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uvhcbywi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ttucyfmx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3axltzheu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3djywchgh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nnhxzssp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymcgfsyk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cdsehiqb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3witcwuix.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oxbgnqnn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lsjnyfmv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rozuehuy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gcwvwuuy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3canawgta.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3eajfemvn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ninvjwhy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bvnbajep.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sqjanwej.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wcsckgrv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zszsylye.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uxzipyjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgciqaus.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxqggvhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkvrqtfb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fantkfel.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yguqpaty.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xwfpcsvf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ortabakf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bwplnjso.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3djcqlpaq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3oehrorpz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ymfhltaa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sxayrmdt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hppwsevn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ujbhmmck.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3idlicoro.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3scigtpjm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3trujbfyr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oyqtgugk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qxypqbor.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kzqdcebr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kfcdeodh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mitjgdfh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3lzxyvjbw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rlznkbca.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rzcgqony.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fbpiuega.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ryblyvfi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hjukspux.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3asxwvzct.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nesoloqh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ckgvvedf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kslyfbvy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3prytiaaq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zjtknwra.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3czzsovbu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3sfbplmzv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dupzuqfh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zthozniv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xebapkri.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tyqdlryb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydpyntgp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ndcunxnl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ryxavjie.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ysgbeodm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qalalpwp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vcqxsnfw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ylkezxib.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qhuewotw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dtcrhjdb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xilytqsq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hsozhnms.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yhimqgjt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mdlcqtkf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jyuaooko.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zanvnioh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wdvxbcar.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yokmqbpp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdhlehuo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ruoixpkt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kewygnma.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3glsmgott.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3iwbhtrlb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3supvqbgi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zeymvylg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3pqhsripu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3efnqieca.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3argbcuua.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ojeddmcg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3supvbnak.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vhkcrepg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ajrdgsuf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xurjhtqy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3svygnccr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tpglnxgz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlqluf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fkpndkpm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbbdumwm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udycpdyf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhdnkik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igeskddw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hpgnbira.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lovwqqab.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ujabnlxm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzdqbp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3pxfeicad.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3knsszntq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bpefnauk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mafigjdp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikwanqzz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3omydercc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3govccyep.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3foacnatc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3xwauvexj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zrtinvsc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3cmdjdhnr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iavrjwih.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wbpkupoe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fjasdapp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rzrdhsxj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3znechdjb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ywlcgdqc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rqjlgoek.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kwfppcnn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rprubnyv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgxlrna.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wyllxsqo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3btqapfsp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3zqwcgzhg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ozqlwnjk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3msptnblf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mjubufvv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3blvnhbdn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iyvakrqe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xqkbaqmn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wmcaqqxc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cmkrdilr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ymwmnrva.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3reblwgwu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vnsdqdsb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3onmtrebc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3zfvvpttb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3idyarptz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ibslkjvd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xcdqitml.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3olbequpu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gvlnyvhv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ftsucqzf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xlaqlrpp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kdwxqtii.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mvrdkqfp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ljrxxrup.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3maoimmcr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ntdvyavb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sxghkwyu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xabjbnfz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfxksyv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3aqrzhhqk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gyivycmw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lzpdmpob.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uwjyhpzl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3shjbarax.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kzlgklzh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3osmpzeuy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltlbukkd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvvpvers.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mtrldzpw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rgptxicy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yxgzcfpc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tiyermrt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3syswfwju.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3neassimx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krfhludi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fckvhpri.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbhzkizo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3piagwrtj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3orjizmjb.html


<!-- 参考信息 -->