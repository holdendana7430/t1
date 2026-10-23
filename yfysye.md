代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sdebencx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xofmmvyw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dcanmkyl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwndiaxr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lhsfvvls.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ghfwccds.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gqnnosvi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kurxeadu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yctmxjco.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qqpgzibn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3oyrxeonl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tzvbeevb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jggvisln.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ezhcxijy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jtoptlyv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3sxxxqmjv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnxtri.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dxltsnmb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dcxduuzv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wexmmjoc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cvqdklcu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ovsucfjk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wdrxvecc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sxvwtacq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wdcnchos.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3glbfzjyu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3muqwcpht.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3emlgkmql.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xtudjlpo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kexmsjvo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hxrdxasn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hgznptsk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ensofbsq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3eiykqvdd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yjzppjyn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ycxyoeaf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqctdz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3raovxmww.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xuvtohqm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wmhzwymk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gsmitlgh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wrcjwvnz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mrxsclbc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zguhsmoy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sliprpmn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3arnsrqme.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3whijplav.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wmlkergm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pzorcznb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ndlgyvqt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kgfaodmd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3burmaywm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skytytmw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3eiqmzioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohsuxcgg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3febdfubq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3kenbubqz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jthyokzk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yqmjvvac.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3augapbbk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3raxnzymk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3acakyefs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3krghdscc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hjeacpmn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3poezozsv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hxhummgg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3avriyqqk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ssbkqqkl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3oefhxrki.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xcxrfidc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vfiylosn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tpausyha.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jsqjilfx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3otephdfg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3mlnwxomv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3sevsfqrx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bfkmptsm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gczraiox.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3avjvzkyg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3feoknucv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nfyejhyw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zfrrxpvl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3arkbtwct.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dgevruuf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3loiraqbx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nxaxnqjk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sxbksblv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pgoqrzts.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yjysceoj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3owpqqxbh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3foornqnp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uqchtwpw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3svmrdaop.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3uwtoxlzc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jwvmegpr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dvhsqwhy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kcqcrkka.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrqptj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vvtjcbzy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eaxmeypb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xnmypcee.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hmtqhszw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cgxtsope.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mtnwakqy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fnsbkygt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zvztbiad.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ymzwvqbz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mndfthso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnibrffe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3upvronjw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3yxdnobju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsxxecqw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ruzifwfd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wrisvkqd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dphxgisk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xxcldbfo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vnikkegb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dcbbhvdh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dbrnilrq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pegrrmpc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ezvfxfxb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bhhaojfb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3oxdovnxb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xxrkmnpf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3uxcqdcab.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3sziagpir.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ztiqayxw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3emonqddx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xejfsbke.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3tszydwco.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ywrawpli.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vqekcwxf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ouywwlxg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3gcjbaawn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vorvcdui.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tbkjaveg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vzkpwhqj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqegfzwb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lqmbwgik.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ihadkqhu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmcyqumw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ngkuzbfl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jozqegwf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uzbfhoqm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sslocmzm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srhrmicb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3grchowjt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cdxnoafc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tvmklvki.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3oirucyxx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utxcfctu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3tzyajvhb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzhjdqni.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwmfygwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qmxkpmlv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ipbjqach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahmeuwuj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3euinnxth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsfcroaq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ppvctluu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ibcagtel.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qojbfgud.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nahtfqkb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bhkhmhpx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3geqghpxo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qxynyuzh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tarrwxqf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iwhsqmnr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jqxbgjtf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cowtwhrp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3odzqsgfe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jwlniakr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dbolwkll.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3csteggcx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3iicbhcgo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3afhzvntj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uhqptktk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pjohagsy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tmeiwxcn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ljyuhcqn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jgsexfnl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3engasblo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wyirbelc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zxiqgboy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ewwlkoll.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dttsgvfw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3iskldpoz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wkyonrnn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3abwwhkqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mznykdkp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3twtqjrbx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nrfqcmul.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zpdcrygl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fksxrhhj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xvdwaxjt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zhjoimmg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3qzveimwh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tndaemtk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uuzcqtfr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xluhusac.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kdwvjhww.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qlfrldwu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eybknctx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ksihxyai.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qdlvbokp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ihzqfyid.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ezquqroj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qvgvhpxn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kvqstunz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lrjweguv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3cwzdruzr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3rozrxdkw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3iofuezsb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqonizjo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dztluwcu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rtyqesvs.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3tlojulah.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwzrixc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ubtqhlas.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3drdzqvni.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oresunrm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3raruamvy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lkiwtmwt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxksxqj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvlzmkm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hjidoyxi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wbatbkiq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eemgbupd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fuosfhcw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ynfswlyh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3luraftwe.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ohotpiqd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rsbdkuqg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mcppmjto.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3apdkdwaj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgnzffg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3donddfgp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3zapdwsku.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ylxskxmk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvpzfem.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xdiilqaa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3guajfcxe.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xvcticso.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gygllcbg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ueimnaem.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3twhoacni.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3haseobbp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fbkfogak.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkdviol.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fonhqcom.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3qbkxlhdv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3npqicojj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tnuvcxti.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qcjoskrk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uhrxlcrp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3btpunofb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bbznyijc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3beuppslt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vhhdmgel.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zbkmhonx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3teeqlsfm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lnzogsjp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rlwcfjji.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3panampaf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3yhdrttmc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3obcbgpaq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxmoaf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jvrpvxew.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cwlzkhml.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uauaznrp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nnxryzor.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3khfmqnsv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dwqaejrc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elfoneqd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qcmfqsec.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uglljvfg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yrlczqxh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3dlgpioci.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hldeujad.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nredndpe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yzwvsdjd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qzapjkxf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3njanefot.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3sdqssnza.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pdnyzjvp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hxdvgwcw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3skbnawem.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wphrjsub.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3legsgeph.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3drsjxdom.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xordpdxa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yswaiebs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ltbpzbxe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fffvymhr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hjitxzam.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fwukzyoc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xfmsktkp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3aeethrvb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymzuerhs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kxchywip.html


<!-- 参考信息 -->