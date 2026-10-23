代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jqkxvujm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nspgavxb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zhpktuud.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jtcesmzn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pmjwefbi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wsvgiebt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zgopsxww.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cyhttnpo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3sqgzyvik.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uqhmvgpz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pyvmlily.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lwvtvokj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hnalknrt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcunytj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3neapzicv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dtkrujyg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vtpywryr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pideijzv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qieplsru.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ismkmjqp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3evnydqnw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3idpatynn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ciwvwbtz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jmveroxu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lxsyzwuz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nuozcbuf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lbautqwu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cdvmbaoa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vrtzzhho.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oppbqvyd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3asqjschi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3eotbptlt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ccheayer.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3owithiut.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wxndczcg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3phxhbppr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yqlidfbs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lafhccan.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbjogi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3morjagmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmsgexyd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3itrarxvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcuvexik.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jfoeetpn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wflkscbu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kfhtndyx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mnqgsnqs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jkbkaieb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3asiwwgfv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lfgrrcsu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3prqfexea.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3byhgdkin.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ecxisfub.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3utgmmjpf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wyrbyczc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3swweyghm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ubvuiftp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mfmpklea.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3laymmefy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fqwabagm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kowckryt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ouiegqql.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zhsptkzh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qfyzvazt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gesvcexo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3atvpmsbs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ysmpxrgn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3oxrwjujd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3lllguuiw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qhxhcomk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3odqlsedx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xwezmvhl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3btahcnso.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oyutiegr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ypmooduy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vwnmzklj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3snwpfxzo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zlysmfpj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cykgpmqe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3thqcitla.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vqqmdynq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cvqvmjle.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3lizzcnhy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dxnnsgie.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ysvdzwul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oebqnfjb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jeestlyf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xxqnlfps.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ijvxpuzr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mcqwzsjv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vbxlnrhd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hczebubp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zqhekdjs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tkeafcdj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rwpuxeki.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qjytslft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anyuzeyl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nhzbfkbg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dpgbkjee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlnirhkp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3iyqlbmxs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjtryi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tjtxabve.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3pbpyozfz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rxlvtxlj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3uqzwkhxm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3lfgjpwjh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3zignvtov.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nzrmkkzd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wewzbkkn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hdowabnk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pyexntva.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3drnudqkj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ylzixfoe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3anepvyct.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fgovjqqq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hsucflkm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3htgyovpu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vcqmosvx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rsecxuof.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rghrixvg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3biuyknmd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xipqbguo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fvlrupqi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vmhkmzbp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfvmvdsk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ktvdbzgb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tgbtnkla.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3codfshnl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azufizsa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3swpcwjca.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bmcynbbv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdojuvjr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgultzwt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xhkbedvr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drgusfss.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3macqzbib.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3abiuexos.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ollpduto.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzcaalab.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vdeicrcs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhpdrsvz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3erxoelhw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ybgludpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwagwgbt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sndxijan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3felybqdp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tubwlcun.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ujzkbcoa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3mvctqnzw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3svurgjqr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hxdawgqn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zukxowoj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pigaogsb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tkxljetc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wruzevgo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3otrmhbvc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jzzxyatu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mdybvpja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ovzoracf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xgksswyl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ejqceyds.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fmbivsoe.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3sqdmhbkx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jnerqvcm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3qqukfpig.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3uwwlfvgi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsvphuwl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gaxkewic.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ayzclwva.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bermxdyz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bemxthup.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wczaqjzi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aezdrgwm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjekkouw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pclvrzsl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wohivsxe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pzbhwkrs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jfpsvqty.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qufeqfeh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3oasphpcu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wwhhbgjo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3staemmqn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ledjjnmw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3czsobgij.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tmarhdtt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3irlogqup.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hxpqrkdj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxyozhhk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3feyiwmdy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wqiiwpdb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmbtlpxk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kcyfzwsh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kglkzntt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ezevhkoz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3aposqjnb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wtehttvh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pxojzyau.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ywnarjgo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ppwdgiby.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fjdfbcqo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wkeikrdu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ktstgldo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jetumvcx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ghlxulld.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3incjdvfx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jbsidvfa.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vunmuvqp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xpncbssb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wdxqtama.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3idawchof.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mrgzlqpt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqyrzrk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3obxuirhx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrxsfax.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwqyvty.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zplatdsg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tdyzhsaa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3codcqqyw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3afqmmgfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nuliplkx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xkblrmlh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ylgfrbmy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nezmazes.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gkkbdrur.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wdzkoqvt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lbudvbne.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iskszimn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rikprgbn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mvzidghm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3aqapkoae.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3njuicvvc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hwpebjhj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tqalgnrz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qzjjuufi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xionrjrt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3azlnhmjk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3joiidlbq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lczkooqu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bzodxuhz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oimtuwbv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mmmceskq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pkwjdnht.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tcxkxjol.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ftnvrmup.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kdwzlhos.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ftitsjhm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3njpehzxs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tnskwibk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qkoaxuqy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hnkycbad.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lgvijpnt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3rpqigmen.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lsbyhryw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ekocxmpd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jmxzjgpm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ashvzuwv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxulrnfm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3stkrhhhk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vbuoqflf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qzastszk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zjeydhei.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dezvuhch.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eyzgjaty.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nmimuqob.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3utledrvt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nhyrnidb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3inwrkxbn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zatleywy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qozdhtpr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wulwebwy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3fgmimqzi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3otjdlyas.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gznmipww.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rhtpupbd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gttjqoio.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ypheybui.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dprmnykq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zmqsldss.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hvtzymlo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eovwrynu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3btxotebr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ymfkkmor.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3eiyqndce.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bchrssri.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3shvkawmq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mievnthz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zrjqkdwz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vajsxodj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3yvzthpay.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrlkrx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3oqfngalr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ogempbrv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3parsvivy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jjytthki.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cqjkhnzy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vbwhvcbg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbczxxei.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gljnvsnv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3guosvbfp.html


<!-- 参考信息 -->