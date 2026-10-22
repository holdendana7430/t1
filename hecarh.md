代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yupyfsrk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cckglbmx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fjrgeeck.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2iwsysaeq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vpmjygbg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nygkzmqw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qglgyzsj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wcihftph.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2igswtyqe.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dblmekwj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ynsblwaf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2voaxuxvs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tnahhwgr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2dowcjlst.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2szocahut.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2abxbpexp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ynjgzjyg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2seanillq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dxkscxed.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sshfxyvj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oiszpwkc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2krmijyqf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tspmndsa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qykhosbb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lvztmnml.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aacjumoo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vionstmz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2utskanok.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dcaltvcs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vvkanfdh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2psfbcnis.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2spmqcuyk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ubunavth.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rpwusubg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmgjhive.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2verwsxaw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wnxsisst.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yqijypdp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wivbhqcg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mfelddia.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kezgzvfw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qwbljskc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bjsovaoy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vnepkbzn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2lxjpharw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2njzbsxhe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mlkyxjyr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qypondds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqsgks.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zwfoejwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncnxrhuj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jdltlvls.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pxqefobg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uwowaaqs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qgszlndr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mnvgkhlm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2frapcvkp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jxbuahyd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ujklkhvv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bobxzymp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ocjlagiz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ijabzipd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2oecydqow.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zcdoxamm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rrhjtsrv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2scyquopu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2iqirjlri.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xphbwyqz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bxjcfaca.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yetrkfjf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kibbhfbs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ksrzaxch.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mbuzqwud.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rdxxgdgi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkdsjx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ahfupeio.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rgyppnqr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kfcydqxa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2weljayij.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hggalria.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2joaqjgsc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xbmcivhk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jtwdbevb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2htnqdhbd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ilefzeay.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zoykudnj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bwykptud.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2plfikaig.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hstxjwvo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lbowckms.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xrvwgtnt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uynmdcgs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qoxludsg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2damafpxi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iysboykd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vujnbyvp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bujgilwr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bkscazfp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bkyjxzti.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pjtouuyj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cfocpdfj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rxzvwali.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2cnhynamc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sgbdqpzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgzcsnyk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2juktpiua.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hrfupwhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqiymrfw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2uuavifnd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dwipqkdd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cmavqpfx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2trtradij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2uxpetkaj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2prmscbap.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kejxbpfx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qbcwnkdw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nipjsspl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jhdgrihh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2cfhvdaln.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2sekzlwuh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2fqnzqrbg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2diteyufz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yuriezca.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qpmhyiii.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bwphvdhu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bfaljhow.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ukowagsn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qnuqazaj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mofsabbv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uqpexdlx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fatqeokh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgvlptxl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jezmvfep.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ycbttkir.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yoikbbnb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fboomjib.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dutpouqw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hjumgiuq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngukigok.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2brwjjajp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olnlreke.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pkkuwyon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmhtivuq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ytembfxa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trtcwvyn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2eeidhrgs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mlqnfoyw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sljuisup.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lqpyzmyf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jghiaxkg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ypxokkja.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bpizmzcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdpbqnji.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qtluusww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zebfqjzk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lzcwlvqk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zxpqeqjg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2lsgxtahz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pungrqdk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpqbscc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2veoaqvwd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2czmxnbov.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2okzautjo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dpqitpip.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zbnrtqmz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vmmpdrii.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jnbadbxc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aikrcamx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2eejlirbe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nmkqlpmn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2wifdclxw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zgmtjeat.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qkekgohs.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ygktpazv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pplxrjya.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qndasjaq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tdgavtgy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2phkhqbbk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hjvlinkm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2plejjrex.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ycvgoxye.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dtbafuvy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgcctemd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zgmzymsg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2utbqyzmg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ssusqwyi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ummhqnth.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2obftpxkr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sczxbmnj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yigjxgtf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ymnevtvv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ngwcmzdm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pijhhjwz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sacxyrbu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dagwfldu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvmdgcyp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfvnhszf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cymphoud.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2deqptsvb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2esdjoolk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nialrpfj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ilzynyrn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ggjmervy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2toqhynfw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xpbsfidc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2geecrwqs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jzrxqwsk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gjyxkmhw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vsyzqxbg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wimuvsxh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jixvasic.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nuutfmjm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmrhlmyj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfbxbx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xndmzvdm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lagmdced.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ngyendme.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xxlgmsge.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2omrblvwp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvyitrom.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zjoivden.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qdeihqwi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2aijwvypk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhncdvw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbshdkw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hzubrqwo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lleizpog.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2esdjqwau.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xxxizsfb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtnugasg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vgtcytyh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rcaphwqj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stskomag.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fucgppqt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pzujrvah.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ziqswazi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jqwnbzbe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vsukgmmu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mbilbmne.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aanchgbg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bsrtniir.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ounrwevv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dhedlebs.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrywvpk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tsliqzlu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ymoxctpz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ggxrwini.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bmimmyxq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vrlrqijz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nmdsvsdh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lclcnwpt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lxbkgomd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fnritmte.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zgvunebi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2snvtuxzn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fydtraoe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ohejnihu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bvzhmnph.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2aostdhrj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ktzrkjrz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnglmegb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qujdccic.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2opvijnpa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jlwnzuwv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nrnrgaho.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdzntoxi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2erdwwugu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bkdhaeaj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2odciepny.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zencwpov.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhakbkit.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xtzndhqt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2nhbemewn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ymskfgqq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bcucmint.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hfyyhmhi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dlrsfvzq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vpoyuegr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2igmiaods.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rkdnzgqw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2acowrubb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vgeuhfkp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oteipbgu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vaixvwof.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2elygraqu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2utmmpbtn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qrldslsp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydzuebcv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2weshgrnb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bluhslji.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gediywaf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2woaqpxfc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vqvzvwgw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2duatxssf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeaeiljk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2flsgvvkh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mgwyumpw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kdbtlmaw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zsitfsod.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ttjpcaak.html


<!-- 参考信息 -->