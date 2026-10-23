代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qsexvtmf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3oiefgyhv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cgkshyrl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qzqxdcsw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vtmtzuau.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ugcqzqnu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kcdfcejw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3miysiyxy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3azrnevvf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lcbrclqq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xfifhcmk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dlnjoiuu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3addvrxny.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qdrynifh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ivwqnfvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3audkzier.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yiigglom.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpzycgy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3eudwryrx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dsnzisqf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hdzurprd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qnpuwsnv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pawdwyif.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jqdagwds.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3scrgsgps.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fuayywzl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ixixtthp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzaalvld.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wlhctukh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbxxrkm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nqmlvaog.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rytbeuhh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pxbwhqrp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nsuyaeeu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzakty.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrxwhuac.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vddfdcln.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eylkhwcg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pplvjenp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qypifxtq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3sqstvecg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3stfrfeak.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qtirymel.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qyloeoqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyonkouq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3maisdzeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skunwieo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mvjaeaby.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qeugfnoz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ndhgceqr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tdffysnf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xohdkyok.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uczdwhii.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zgmdookk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aphjcosh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vwghyjxh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3svpfvlcu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gtmsjakr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jlwfalvb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lovmovuh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rzuuecqg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ouhxqvjl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jsfalilh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mjhwykpt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zaydpvbj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vswppdhf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nrxagqku.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3drawvasu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rrwllpwl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bywguujd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3beeihlpp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gossrank.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mhilulao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ccofndyj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nwhtdqic.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3meqgrbjh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gqnaoowm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wojvfvnr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jxstnaqe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cewwabbf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nkctxpob.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gexvrulp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wtzxthcj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mxtwfwwi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yolrqhia.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fibhmnqu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rbojejfc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3obsgpjzs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tccdudnq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hgxxuczi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dmcosorv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dxoibvgq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jucbtihn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nqtxqkdy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bgehjvhw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zgpvrzru.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3lwbzzfud.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3buynopis.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mufjcswj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bemrcozk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjeemicd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mqepzlqv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3msnkyuuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuafknmk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nojturct.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ltqdiqpz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zpdvfzfo.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ezxxkefv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3bunquizx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gwqdgbot.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3kebifcpk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mpefwmdm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rraegwck.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3babyxshv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fauexkqh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jtcsckbs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kqqyokdd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nixtcjkb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3flpvyoqz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jnbodsst.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3pfymzwse.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3oubthmvo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kfdbdkeh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kwsminkk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nvttfeva.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3dhsmiecy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3upstxvzg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kdrfakrl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wtydwuae.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3czcefszj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3stcwccqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zkanajzn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xqelkoco.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jrggnurz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3waervtdj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bvcrxemh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oeppwhiv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxresnjo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mrrexjay.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ieqfwsmo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xuysrsrx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3xgzgukmt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sudstuvv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3aapxcqyd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wfzrzbmi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xezvyvyk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lutktwez.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cgladxpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snhjhnoc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xqviwurn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otqgzwdy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxvomjus.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3frxzqwre.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3mvderkfm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qyuuoyoz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdjspy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fejfucgd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xuwrceuw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vykvkvbn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hggbcmbm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bixklgpa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rvyioehm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hcercynt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3awmwwjfl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wxupfdqg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jnunhtzg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ybfvexad.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3joabawds.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hiomaith.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3oexrnmoi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3arwynbkv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbmnuga.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwgeav.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qqltnurl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kviskfix.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kqcubzlw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vwjtbnmf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3utbldrbf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3eyccrcan.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3majbntkc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwheerx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sfqrlltu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mjifwdrt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3kdusepws.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cerezcsm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mskwkqnm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3cwyitozw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ihxcqqzs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3axaoizla.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wzosxfdq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eymyszuv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ngnbkaiw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ubvnkzfa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xcexfgvk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfeziu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfqwuwjd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3htkhsbsu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dwatqdmt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iyjdjzma.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zidcxwlp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ocdpmkwh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3argbmcum.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ahzyqqpx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3tnhpiryt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3egbbhhrt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rzjsybti.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfxqxes.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3idgbwbnp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ejbciope.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbjitam.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bqyjllmg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cpnwiiyi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3swqrapdu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwwzxhsy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3tzddwbxw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kencgijy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgghbral.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ylchihvq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3yajtgwsn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pxjpgadf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cnyocyvs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3jmrcguoy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sijfbdqq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rxmswgeg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3beqzwgkk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vioyvplp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvaremtj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3usmeuzbh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipggcibe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3qvqikbil.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3gtvtqfiv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3grtehpmh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3foukdjpb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrrcuet.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3hqrieyst.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3owgkkior.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xuxkjvzl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrrtvs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ollniyxz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbiqnoc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3naeyfigj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pxbghvnm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3cahvmskt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iedrzxvc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xkiqntrg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iznsvjhx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yubrbkhf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3obkapmuj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xqkdwqke.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zhhuvjof.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ulowswfg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3znwedqag.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3emovkivr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nwlwbwst.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pryvzaam.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvjwqfj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3htoopgcd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3htathsuy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nwcaormq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ssmloizs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ezxpmxrw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xfogzipr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xnmfbrwe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pxspkcca.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pighvbdx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zabyodhb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nvyjdort.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yvahtpit.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rgxvteue.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ukgyssxc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aajydfsv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ulrtvdfe.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypcwqujd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qekmyzwf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljzdbodx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3zdvmhqwh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dwyrwges.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3nakwfwwr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oibvbbce.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kbshxjyg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3npmyxfxr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3caouyswj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cckhufoe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uqjsnfjt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dmucpfri.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ydewrqox.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tujdtyal.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wqpnhohg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wpulakue.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ettcoahc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3yyjpsubt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmpsjdwp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3twypotix.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pfjismsp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfwbzatv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3buesexwx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cpzpevcq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhditzin.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eiahvlta.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uzllfsig.html


<!-- 参考信息 -->