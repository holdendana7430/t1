代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kaltzohg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2adficzqb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2janqeyxr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bjnesjvw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ndfhtkmo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qeqygcep.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ekhgslyz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2eivofzuk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dfbymgrg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pzqcxklr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tfegoxui.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cipcxugo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2acaapgik.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lylakrxi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ietcxvih.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eflguikb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2euuhxjqh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgxslgij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2upnnogbl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2viqpdtax.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ujifkywy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2brxeqrla.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kqbxdcju.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tsssined.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iojmsrhb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uaidowhv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ydmgmsls.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2uvpunqqz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2avzluxfr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rijhotfl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hiwxypob.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwokmuv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fhozccrb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxdybces.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xgxyicwf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dqeadfpw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2itmkhilx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ewfmnkzs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nuizjouc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tltmspwq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2thkdicvw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rcaohosm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qvnjrmew.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xijcetds.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bmdlgxbk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jfhaozic.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2cdwisorf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mdikkbau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dozmeklw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrizmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzsccmjf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pbaxvktq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2truupons.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mutjvqto.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mvvonjnq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bmnjybmj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qjpwqxdt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mhaehuek.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2slecknre.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ppmiwxlc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lywipyhj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2outkhjar.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2flqhtfmc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pbkmwimn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tzifcgcz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2aseleswd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dhrhzgpw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vyfpotre.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kpdqutgd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2csevlklr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2zbxthzqk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2evyudigx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2krhvhusd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bynyawok.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rqixyreo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gtdieqzy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ixbfomrd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vzqfratd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iczdacrl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2taozjetc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hwatrwtv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2amykpryg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dmrcwrki.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zhjydywv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ddzyelwq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2scmlxrud.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2suzchbhj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2twbpodnn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pzdejxxc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2hgqrtuvn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bihkxold.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tluhsjey.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2oiqzyynj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yptiindn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2imlnwikf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uymrqqco.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rgzkhzoi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dnmzsxzp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dzqauiwd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zyeknyso.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2aykdbsxq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2drtnafkr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sshwmryh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pxbvxmim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydapbbvt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2bmyfrifu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2yynolovw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbscjqwh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tqkybgsk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ippwsapg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2knrgvmum.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2pmmehrgb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2izlnwxbq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hwumnrfw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kalpssxl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ltyjebjj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2smxndflh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nzsgknsm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2npiyuxkz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ntvytzsw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jzmuhfcf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gmpwnzzp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mauxrfpj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2apaaqpzy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2htdcqssw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ovawmgmw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2avilaxmt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2seaiubke.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pnyxyrtc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fthcwsmp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qtlupukp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elzwrujl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zlgqxted.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2apftofms.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mhhjmhdj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkajansz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uwqntrvg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nqdjlhov.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mzymuqel.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwugfreo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wlgbjfww.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fkiszbch.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2roebdrmk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olpercck.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdflzawe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2numaejoz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pkwdghdy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2oyrzrarj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uehmwbvr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eubzvxtk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ziwcwdoc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsbhkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwujkutm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2coysbdxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytixszsg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tftaoqyw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yqrncchk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qsrcchyt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2akzkxvna.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ovvvlzdf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2axeeeytr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2byuiguqp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2azvwjmyc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mljhlyzq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2wgcfxtvc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2knqzdhij.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cxppeufo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2obvhymcs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ktdkyhen.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vphdhiej.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2arigkwkn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2fzleyang.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqofcix.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ejgiaxog.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mddoesxx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wdbsrbcf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hckikkhh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kuldtbsi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ypiteood.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zlwioxpj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2chsbrziy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rsltfcey.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpqvpauw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pzgyrivq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2atjnbyjx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2pilzildv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fwhtxakq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2pvwfbmoq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rwofvxqi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2dhttrzvy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2oxmhwvpr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nilgsybs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2leiseool.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dqizsxxq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2olmfoopk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tazfhlsq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kobogcam.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwsuxlgv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sudcxjop.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qlmdpmmc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2diictgfq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mwolyfta.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2crenzxtq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ynujdvul.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lwsghivw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vnxdbhan.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gllqhtpl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2delpyqan.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gkzfufuh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijaeekhp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rnseqqcv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2luhjqqav.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkwvnszx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzlldql.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dgxqbdsc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vtzsqsey.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wsqkcskj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpdssuiw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vkxjndad.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bemckrfl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qhilqedt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vswvglpc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2oxkebicc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tefqtbag.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vvfskitk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pbidjhdx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2thgdycgc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gwcsrqdm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzkotayp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrjusc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2emvgxsmo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oahniity.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hftxdgnb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2qjfjiadh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pwrsznho.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ngwgzlmq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iriymyyp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fgflctzx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xsflpgyc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwvfixph.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2orekymyf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ebiqscht.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qruvjsvq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2lgyyhrno.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nvquylgn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2cfxchlxm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mmwbhsql.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pwjuwnqg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eydfmetc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ftswudyx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jwglynxs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2tfpjfbcx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2skpgoogh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ipgetzjb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjihtefy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvpciibo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2sqpnsuin.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bmsuoplc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yjisldzw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qcfqmdwd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2loismyyg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uqyjuxvu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vgglahhx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jjfipkzn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wjmqnhod.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2otqknack.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ibtborbm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lsjgqoaq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pzlpatjq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qdpckjvp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dvlqxoco.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sfkmsaox.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2frltkisp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2aiyhudwk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lrekuhhe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xucktbxi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2liwuovlq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2aqibphos.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hwhvwofy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qpfjiver.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nxgucexb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kjyxztob.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wtpsrmir.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jhlfeslj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nztderfk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qqirvbvl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2hlkzocuo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmqosdo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rphenyev.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lbruamwi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qrogsqzb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2oojleaus.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fcyebsmf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yrvcibuh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2miqydcru.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgvylmnp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlurjjxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2boaezigo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxkvraaw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2mhowjzpp.html


<!-- 参考信息 -->