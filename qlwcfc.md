代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zpleczjh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3takjouyk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3egeyhqje.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlllbgr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqkerf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qccnixat.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zzcstgex.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ooologfy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3grquggps.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lmljhrir.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ygzorzeu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvkispn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3azmbaxos.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pcqpnuyz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mowkdpvb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jaxbqjna.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3merremwu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pjbagfbv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zhcrhqve.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ikahrlal.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3orqmdnws.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3giedqmrm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oatnqiwh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eckpjlbb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oghuyddz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3neycbmaj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fpvhfgao.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3onichcun.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rlcxiqyk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uitcgrhg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tzugsrym.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pygzznfa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ltbxzwnt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fqaixokg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3noepsdej.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmnilepn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pdfsnpsg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfvxnso.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gydnelot.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3phrkqhck.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kygoaxvu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jcierrvv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ckbucher.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ifneeuzf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3iamzzeqk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3utrattbp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3asycotyf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sdpzjdvx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fjqjxofu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hcrfynfi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sfolgtnd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pszafkcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiibrhcm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ybaolpwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dblywphx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3eqvnoluk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3asjcrmei.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kakpmutk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qojtxcpy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ykkqipgn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmsrdnux.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gombydbx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxistxtt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bxduczlw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3eomaqwzq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hnusvmzr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nxzloylg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cooyhsns.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hdkkksic.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kuytgbzn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3teoeogoq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wutbypbf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3vygwudbi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3egclvung.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cpwuxlzc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vmjrbscz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkcfhe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cctwpggo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bgzrjrci.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vecptevm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3sabvfsgd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3adcmtpim.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vzaroqlo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ggcogpzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qlgpyxdt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3azrwpxhg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zsdmfqxs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zdkqdsxh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vaqooozs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tiyfdofe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zdfwlgsz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gypvjzlq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kuiyenai.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mllroxku.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3imhdvbtj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nstvhsod.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrurkt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ibipmtmx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3guivnllr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qfulssbm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3noospeek.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bzbiphyy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3iohiwixu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ijjmzrxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gphcjrip.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3sftjnijr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yjgmaitf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3vjheeikl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iobkmpxe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3eojypitp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3khgavnmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvtqturn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gcahktoe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vonxxili.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nsdcwnem.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ndctzjbu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bamfblil.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vrgzakdg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wlmqhxai.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ilnwfwdk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vjymldbj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3fvuyozsi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3yumyaamk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rehryfas.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hvxlrvjw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hesfxjud.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qbaqxlez.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dalgkmnv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lnmnmjik.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3eomxjpul.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qqxwnjti.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3jizizekt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aheirkat.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jmmlwghp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xbfrrmam.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lvjrysal.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jzesoziz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apfyulyr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bvldgkou.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tvkhcfjb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tjqbojqr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cznoocnz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qqvrcubz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dicsiryv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sjcbkpbj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cteqmsxr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3reektwxa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sjogemjs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3frbvjmfl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtyupvse.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ftafwsnz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lldzmoui.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmawlgpo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fbsiydts.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zvdnwhug.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dmkotvnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trcociaz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnotuzdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsogjgan.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pgqgyner.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwiqfrc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pryuzgtn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qsxjfics.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3smymvtga.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tznlyldc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3opejvqqb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3fjefishs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cspvwian.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3soofinly.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hogqdayi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ardchthe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pcprhhrl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cefimdni.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uhglimdg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wbzdyitd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bpqpsrjj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rwppxtcz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ijxtqscx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3spolabky.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eqlrefqs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3duosjeqk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3casmcwml.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hetiebwc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eqsdhbtu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fstbejcc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcpkkvv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pzdsvdtx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fgkanvlp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bipixanx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nitsejvb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hkwatepa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3aqcljfum.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxqkthy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcosean.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zsvmyuub.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jytjsxig.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3guzuclfa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdwvwaxv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dwwdsnuh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uozmdgfj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucyunxou.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lxkhvrli.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3msrdbxws.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrgxomtc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ufikobdi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3azegkfdc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zkonczzm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pcljxyik.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kdrepyqm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nkxrrmjh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ixrmkgle.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bqlbrijd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lxmmwfny.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfobacwp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgvwqmx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrppvb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sunurjza.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ehawvtbc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3tekycamw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nalfevuc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nzziexph.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dconodtb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rksawify.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mdwatsfr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3oswdmqwr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gkwnahgp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jaoycahb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuziil.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvwzpsi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xmzxzbvu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gadozvls.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mdywkdnc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrnwvro.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3puwdwubx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahhzwdtk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrxarul.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kfxurltr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gfpgaheq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lkveculj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hepggguo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qsykbvxo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3akqyoxwr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nzzbwwdj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tpvmmaci.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqzujfyh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zspeikdh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ahydhmxp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rkroxewm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3pjszoiza.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3mqroxevy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uchquxyh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fkzndrgk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tpzgrbzf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tikypqqe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kexmgorc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3yhdxbyop.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qmhxochn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ahydeimu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zvslersl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lyzdhwsb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdsbewhw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dqfrolvo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rwmcjpvo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gdxoxang.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3araxxtxl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3kxffkaar.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kwuvpgnb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qplkwfih.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vzggcxym.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wmhevtwr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ztmeegjf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nqejgceu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tojnsttv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qohtklhg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pycvvqlu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ouawpcrv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tvvummoy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rhznqmvz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ucncbkvb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ehqtyjyv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wiggsbtk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3oktzxxxr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iepqerkx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dkjjszho.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yffrbzic.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3srkplkrr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zqytkurf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zdfaktmv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ziikaaaf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gjsipstf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3grbtowta.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3skimvgtu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qavmbniz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rowigult.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3eudnkjvg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3twfsdkfk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nrveuvqk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3bbwdgqym.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpirybpg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tnvljpom.html


<!-- 参考信息 -->