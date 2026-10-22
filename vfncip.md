代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcmgrqpl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2akzvfkcj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2unldsadu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qswbjytl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lqregase.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tpfenrgx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2gseohasx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2raiavblw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eqkefflp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qoifapuv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nzyxtlso.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jdjmvfoj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gzoozpri.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ixaiceyr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uyvrobrs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2lqudctjk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vbvjutuz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hxohnteo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2egpyfmtk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dakzqijs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xiwiccfn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qgmmtork.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qvrnivuh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2luyfcjym.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2atmasant.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ojvqidkf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2frgzqllc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2svfftfka.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2olzxdijp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kqkxyjou.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gldfrrkl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2iektgaba.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wmeyjmfs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuzcagk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uewqgwdh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pdnflemd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gfxzfrrl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2gubdloxn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2egoeruwo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nzfvjnba.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zfrlolvs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nmxinfhn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2mnludsrr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2htltsvzq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jzobfjjg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qkqmyoap.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hisnmcyd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2txcpysmr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sdfkvsrv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rscxriwi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2gxgkidzo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nljzjtfy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sjzwfuca.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yxksgdjd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oxlfajug.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hetjprtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qevhbnla.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ztvlqvnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyxtthpn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cdmyzacv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vhjksewx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ylkwdvxk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hwadeieo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gjgomzks.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hlcsjxuw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2obnjhoro.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ezdvfyba.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gcvsdkaw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2msnbpqkb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qfswkshl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rfyjcvtc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gatgnsev.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tesoexwa.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hefpegyu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kujslkol.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2qqhqduve.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jgoucdgu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qrsqkbxv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lwtfqvab.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dtytweay.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2utxntxih.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vmqbxffs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2spzqbarp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2olberfzu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fworibts.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dtohtoel.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fkbzhmfi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ssybjdyg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nyaigtfe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wopbjihh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lwwswclz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pjgpkazv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ocojynhw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2imcmkwnu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jjsqzolu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lnayfzjt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hoetggva.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sznobqxb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hierakjf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pqnibgsa.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jkzpksri.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ledkbjhb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2whhalgin.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qmzydjad.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lvmhttxg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vcdjroyw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ptzcotuf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2thkjhjvi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ejradsbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wanjpyov.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xqwjsuzd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xcxxoekl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuyfptrk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dfqensnk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2truhxeyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlktkjsk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eojkkhfy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2chdjngya.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nopyznvv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2msdussxs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vkohqouk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2tswrgooz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jjbouocx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lfgplluh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2bjnewnme.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gazugoew.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pwvkjwas.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2xakgtcny.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kfsgavpz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pchzwcom.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vyupsuzl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kcibspcg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2kdefqtkw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zwguhbrl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2haqdnrqt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2fbtdoaav.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iwlovbyq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xtvpsplu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uqgzkbkx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wbhsuqsq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onnwmiky.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hteliikl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjrxxtqm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjijbgcd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dyeguevj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkipliie.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2socfpsqz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdvtxzgj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccxeptkf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vjkkusjp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cilfbeyh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxeuvrrj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hpkmrprk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xozkzqqj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bpbuhblx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2npvpddri.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yoglslyr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wwxwqsur.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2etpftaie.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xjqnlkmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrugzwom.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2itrfysqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdrimqnz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2boalokwj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sniuetln.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yrhvzesm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jvyiolfk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ysugsjzx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xmeyddcq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zghdeybe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2gvnjyulk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dyaidrln.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nrjthoku.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pgdogutc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hpjtfwiw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fmskbxbu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2chukjveu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qtdbnpqr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ihegawgc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xgdnnzza.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ynnkplkw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ehoovxsf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jgflnxxt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxnliaph.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nrjspirt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xplgweff.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhxbup.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mbvawesm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mleopnll.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imbmmjje.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2nmflqecx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdrvxft.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2goffekxp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kqccanrr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xdjjfslz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2qwkjybom.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2awajjquo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2eopsgjgo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ggniwjna.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qyawbkhq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2heowvbsx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ktokbpuo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwfrbpmx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2symluhxq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2odzcithb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cdkvwegu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aetruiey.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nqaqkjsw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gmtqvdex.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tqnwfhfu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jtlxjxiy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ywtahedj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vtjohfjx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fzwsfecn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwmdyen.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vfkeovkv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ccqiggce.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ytheepse.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zdddxdcv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ujiuetqn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lnqijnvz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uhizxdmt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oefsuqyd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdzbryz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ixxkasdp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tqcehqqe.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nucgamqg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2frwkfvgt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2brpuzdaz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xegkkqms.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wuweaqbx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxcwwof.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aprokenx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2digauoka.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nnqdalpr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yldutluv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eeesfeuu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbaslibt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orgdkdte.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zygdfhoo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlhddfus.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2oopxheqp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2oifbvkmr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ahkszllh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zhiuqgll.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zfwpjsqh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2uswzrbvt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2macsbxuu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ofbctnly.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ymlpzeat.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2btdvtkmq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2iygvcqgh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2tewnugab.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hvhzebwh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kxgfthqz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bhwexias.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cqusukqr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2msjrkrom.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2agejnlwo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2inyomgct.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jwsdkhfr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yzpuahre.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kskbiwlj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwuulpjm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpoecj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2guwpchai.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ijakarof.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rllwnrcq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hjilzrbs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qobwggjs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2djhagkqo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rzkfotse.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uqwlpxuz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zhjehlmz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ewqyvxbu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hkqvuwgk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vuepcotv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ultpxtbm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uqwlvgeh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ncyjvndb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fkselxmh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2iqmmffpi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rzwabokz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sachvqdh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vbepzfxb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jnjbevrf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2npzaxtqx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2moadmaov.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2brwyiabs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fjwxsxid.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mnvziccm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2agthvzsq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjzgfe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vesmxfhw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2nhflhdxg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gbajbwhl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vtbcotzt.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wdnbwjzc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2eysvbkfs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uiynthpn.html


<!-- 参考信息 -->