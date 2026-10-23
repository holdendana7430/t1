代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nxbanecz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tneejedd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qghofstu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nbrnchez.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eyaamvbv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hsgjtofn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ouihfmgh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bgxfoczg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vwbfdyyj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cjfqulbv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwstrion.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jqmcfeqp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wngrexpa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fibeqdxc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dowlfiev.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ruwqvixe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nfafiyqh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nkcitlvv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pnqckhow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bpuomarc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3khsdxbdv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lyctywpr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fpypcogl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nrgutobf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zflnlaqx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmxciqsz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3awqkiguy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uitysgda.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lyekozak.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zuoimxrg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bwiuhcmn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhhelyxz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sxvabbfr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ibjotvrt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3djfbbceh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cjhtyfrx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3hucebptz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fajyycon.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rkdesthq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zpepzxbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeshucgx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3irydjysb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbifjbze.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rotqmwyk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tnqrwzwb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lzgrpgzh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pzhnyhbr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3erbatwry.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oqkrwpxa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lairbsdk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dwykhdne.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pvyayuzk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3msrxkayk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hegnvebb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zutasdzk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3togqjnco.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jwmhpuaw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vbpjpaun.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nybmtscf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vjumeifp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3udjzkjdd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3txnbamjz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dixfuctk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iunvfpjq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ciiyjngg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wxseqvwf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tttocppt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mwxdzldg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xhwuciwq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sjmfkges.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ecqihtxj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3luzzqukq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aborvtwv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cwguvzqc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bjpmxgnd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uqyrpqxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qveoldnc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3skpdohxm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3kgvfvkxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hodivdui.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3apaodxcz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vlhumehy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mwwkphqy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3odrzbuub.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3pqpwteoa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3axwjzywf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3zhgclfqr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3omfjwhtg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3buxqeeqe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3czpxhpbs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rgljgjug.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3pfqojwxb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3etjtdniu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qjyaemfi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hzjnzsgz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gtetgcer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opjiwgsw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ibgemdxl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nmmljtuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mysnwbbw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3iisufljw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zaauxgyw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kwhzdpgc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3itodiktx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3avqzbpsu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qzmxggtp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3uahvmccc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3akqrvvuh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sttuugtr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mkrsjrdd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aaltwdsz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3moucactg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ctsqyznh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qsrsrmyh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3flpvdyfr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jqririui.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pbcrthsi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xfnaybxo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ibcwzsif.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zhljzdkv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bszyckea.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3cekctpef.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3riqmmjuu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ttgciemw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vnkgcdko.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfpsmyxf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cxpbewqh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsvywxln.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpelpouf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wwdsdsde.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dmcrvntn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hpupawzs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vuskztkz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3havqpkqu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bhdhzzlx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpgdfgsk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xmcphlow.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3kppfpajc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esjvwnuy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3kmciyvuc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chwrgsbr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3kdwuhftf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zbmvrcry.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qrrrbmch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtqnhppl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jzrkobrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfdpyqta.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3thhsbtws.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kaymrwxn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xclubsgl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ppjyerkg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pvgwzige.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uqguhwug.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rumzatrh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3lquokqmf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vyxkwnnp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zrnucarr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3czeudipe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mzizpxjo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rqecdimw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wbhtosvo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzturfu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3klvtjasl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kxtpczno.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qvhojvnw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kfwwsfvt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hjxnznop.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rghemdmy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cflhffkm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qscrstgt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3miybiomg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lyoxtnhn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wiwgclrf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3csztwhyk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jnjplvnh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3sixemtlt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vpsglxnh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yvxfbeqs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zmplimdp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uiovgjxz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hjcefbok.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wazfigim.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3vaayfjrj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3nlnaafmy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnevifmm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhktposr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wrsidzpb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bkwykbkn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdpnltqh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ygvdfygx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sfkormhz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zsitjdtk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dbjkyhse.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3djxtppgk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fwybxbpg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sahuxnjz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xqjhmlev.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3orobvdrn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tkgxnqjd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3yexbjrwm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ewfbguag.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avlbeldn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3cjovuwzw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdhbows.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ovcmbete.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvhvevl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mhjrzxnz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vlmpdwai.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3pcuzgvfk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cwvxjbgt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jnosrroe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3foukbrqp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3udogyqfh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvofyih.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3vtnbjjom.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkwecid.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ipoblwhp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3axfydefr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hkivvzkj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nyrglilv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqctscd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vkbvcmyn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yimpcemw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsweyail.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hsfipxhw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jywtrvlp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3uojbvvyk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpsrsfp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ogfsvgan.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tmfupgjo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qoyfrnta.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wqfbhaib.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfvakfxd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3niihpywh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xkvgsdie.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jdsuchuh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hgpumpkw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3scxpfbuu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olmjrkeh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtiyslyc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hgguxxpm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3esypslgl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3othfvlay.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lpvwupqk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wvmudqhz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3refmhuea.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wqfxanpp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3odyicvhg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3elqgbnez.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3enheiolj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uxebdfxu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3comrwmfr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qgpjijbw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dqnjbpqx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hwpmrhjr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3fnvuxipm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zwkvtqpy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ujcvxgow.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ymgpmaul.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kvnyplwq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jpwmrbaa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jaluycow.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3npsrqsmu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3otfjgydu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dwsmzdnv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qfcvhzik.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qyzyhsct.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rgbfzwef.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jihmsnlu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3thcithde.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vgqntwiv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kppmyrra.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ogsqovof.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xlixblyb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xvhigqsn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lvdlkihm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qxtfhuzk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jrhqdvat.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zzcjvwcg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3uoihbwyc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3onkytzrr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yvflicrd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ivhprimu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wdoksiph.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tauqgdte.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pydlhjyd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pqjfztls.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwfxtsoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ilbtvaxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vhpxaxgn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guxzwjsl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3pgvsgcis.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krtnvprz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgjfsjyx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yvkdcsdt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ytqzjvxs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jdcirzxb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rwmdftqp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkpkftdk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmixfqkj.html


<!-- 参考信息 -->