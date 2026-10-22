代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ncelfqtw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ynvskawr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2swubitci.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxweowne.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bmdilpxl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ipgojqrs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mqekarsq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2owmcsnau.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hlkapepi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ptgjybfq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbumptmo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cqerikjc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tnimlouu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ppvupyjq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kkfsjaaw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wbvkfigh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pufvteht.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fpcesdbv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hazyejdl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gkwtkkya.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2esizxklr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kmqutojn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ezstfaho.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bikyfacv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pjhgxktj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kbsofqep.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2tnihyyft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ajqfcqaq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vxewecqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zhxcftgp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2yjcsrlas.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbbnki.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kbhlxjao.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2roqmgkzc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gsevcjcf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ifelrfed.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ywanrqec.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rtngnwtw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2imugxclm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zltgbxeu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lyzyvsxd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxgtawr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qrggremi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dlydsmei.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lqmreurn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nywklijw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sttvbedu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dggwiuob.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mncyxbei.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hdkjwlnd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2stoqrqmi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxprdhi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2syzchdzd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jlecxudh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2apwdfvcy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xjzyzsvi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zgttopsl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2drbidbju.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qunngotp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2sdfwnkxf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2htqnqkld.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2loutzbjl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ghhxaydp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dehfvtzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwnugchi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hfurejpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzyebryu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gprrlrao.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dwwxrlqa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cwtpwfdt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2srqktjhx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gjkrjrtp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qqxbcmxc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bktbkkip.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vwhehkba.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pvlzybxd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2juwgrduc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vhysqmic.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zirxmymj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lbffyave.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2obgyrlbi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2empkhomm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2znquqjiy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cfzkpsmm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2evisylwo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cyzrxotw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2aymrvqik.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nizvyvgc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2onwmassl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2opqzgvra.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hygewawh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ecqiftui.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lmtkrbwm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lqvtbpdr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sqjnkkkk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yexccffk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bgirxyjz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2knbgvlnm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ouszjptd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vqdwfxzg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ywraprrg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bknohnix.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2sayigdet.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yqfvlakv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2uyrkftbj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2obqlbnas.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xzrmftqq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ygivrwnc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2oddmutpt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qadseeky.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bcjkoitr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sostqdxy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kctmvzmr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qucyaqzh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2djndseuo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lgvzoyds.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ogaxglpt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jiojtora.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vkjofdfq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bahqpudz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdolbhut.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nqdatlyx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gmjqemnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znpqrcse.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ecyhkyds.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2idlkcbul.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2abcaofln.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vwdvgqrt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rtyzwnya.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ipboodcs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vovqkpwh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tgvqietx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hyaudenw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rtgelcpa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hsowxmek.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ilaypsra.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jqkusgto.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gabgpqtz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wjablwdu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2snnmbqgp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qzazysnt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2jbjaektk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lxptisvl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2yqszwebk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iyvcvemf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jrsgdmol.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ojmgxnao.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2crzdzxzv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dtkssdua.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsnkcemg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2unqygdok.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsurqmew.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elwabngq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hesmdova.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2symnrbgn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hdjeixsb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oyxycyeb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xndoqmpc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eewezljo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uykmmpmx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqrrsibl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qshfhyka.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kreiuxry.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfjpwnbt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qicviger.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2orfrbpjj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fyvranri.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsqwahji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqyvyucp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ovmhqhyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhmmwtow.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xywytaie.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vsdabylo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2cseedtgo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2figzuvpq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2whmabunx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kuytpgft.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hjlwsppi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2evfqidza.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2unztfons.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pgbwtipb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2nwgaiowe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bpcyjhlo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zvwmrhfx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bbrftafy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uugvghzs.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2duripzhi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wqihtseu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cnansyhq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2moujphij.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mzdtsdmm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hqvqrecr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nhovvutw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rwpfdzpe.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nqrckswl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fzhwtqpc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gxmfrubp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kilhobot.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kdfdxgll.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2yzswaefs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtozdozn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xdutgzrr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ztcdlpiv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rewbhffw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2nadxiejy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjctbyq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2yopsufxi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bzqxephc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2sfrdixyy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2skevdkma.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gpmdogvs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trkhkmug.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hbgsnsqp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dlsxvhcm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2agdedzpb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gazpnffr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lstkumrq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jeuqtlez.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2haruqpsl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrfymtt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2aiowgnhl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2udplxhjq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2dbrdigil.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ijroturw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwbqgue.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozkqsnmb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sczikoyb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbwdatl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kjgxzccx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ttaspdvn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lfkerosg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ifeoaiwl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2adikybsv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rlauvvog.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nbttricj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nexmtszb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hsddvxch.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xiiyrfam.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqnljy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hszypldp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gnfbkcyy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mmwutcbw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jxxothey.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fmnwbxrf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzgjkdd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtksek.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjtaugq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxrrnomu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rvrcztyl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gmdmybrq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2uutpicbu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvtvhjhg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dcyrfrbi.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqxhyoa.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2swxsyvyk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wygbpkim.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmjgkwsu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2elqwrrmk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2iejzqxrb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2djpvdnxs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrdmgtu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fjyqgkar.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fvmzicor.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xbjuoakb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bqsmywyk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2socixorj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gckxvjjo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2amqkanrq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gqvdzguk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tuocieha.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2whsexluz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zjcvahcw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zmrnhszi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zwruxxxr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ajglxmoc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dubvrmgq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdauyreu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wvyxdtqk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dkuzyhek.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2udrngjxf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cfueygap.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bhurobdv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bphxuogj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2boigcajz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lzmguruv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tpodrwmm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fknjkgxa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wjwalrff.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2afcphpkj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pezyvfny.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tzleguwa.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vygcgnnb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jlhtfhwr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vysywhks.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2myhzfdxl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mrltmmkc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2atonrtkp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fdyvfjaf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pbvmrpgq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2elizyxab.html


<!-- 参考信息 -->