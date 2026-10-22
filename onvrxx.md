代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cptglulp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rtwvzgvb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jzqngvcl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zagwtzee.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehimuwsc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fksmufkw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2howiyhqk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rihzujrd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xulotvrw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fgayfwyc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtqipdge.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2siemiwnh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zkosgtkh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dvrgnmbt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2knsfgoto.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mvlnkjae.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qqtcldox.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ficipigz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2noinrlwn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2imvdabak.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2miitnufp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vsrdivem.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rmutfjus.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2tiwkliin.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2suelyttn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jvpbfonf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2sioxzgfv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xpmdvqxf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kluolddk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yrxnxqds.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qizeyire.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2uzytvptp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hvbcobec.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ktehhezk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fboqnbjh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nnbpgtrl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lwlxixfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qfeojdra.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bmwukazk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rxooicrv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hlelhkty.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2acopdywj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dyemtiqd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcayskf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jhznxtru.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcqsdmra.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2frhwwqdp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2grlvkxpi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cgtpnozc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hrvlpwnn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhbjzx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cuaqkmtq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yjdzkass.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wretmfsp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2omjzoyyd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jcicuskz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2adupbfoy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mhujyapm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2danfoopk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rkcoshje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvhfjkcm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xuukilvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mderugjl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2yddekodu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aotuybul.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ldbpdgvb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hpkyydan.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dcctfplj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pbmphlxb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2weyvfnhf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gpulmfuk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2phgqbdru.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dtbbyuka.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2szegmbmo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ysdsmbos.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2snptpkpz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2omomzblc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qhonmoba.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cbdarayv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ygymqxvq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kcaurnkt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fdzrhxjx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vsmfbpcc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cdrqiuij.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ozjqluiu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ueulugmo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eohbpytc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wejfztmj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2iaorpqpv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rfipyokp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rtojwouz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2apinhxym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wputbeer.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2snjncvtc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jflrqwvc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gyyetbsl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tsmuwgcr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rswliadu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qciynfkp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hwihnzxe.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dvkjgnxp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2winnyofs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qvlanpfu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2epfzdsal.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2xglmmdmb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2escpenhg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lftifjhm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mqlmksnw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tnzapifa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zzvjpfrg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qmfwymfv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zqhnippc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sfsbgfcw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2lpuzynww.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pxhmxqoc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ypqyazde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apatnvkn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kxpmvaky.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qdedadqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zloqnlff.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2hsiqsclj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gjohtjgz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zbyffmfc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xhefptqu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lcklychw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dvcpntlc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xpltkemu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fvygsbzh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2albjgsht.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2szcqcmex.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rquwpepo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2luogefzn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2abxrisdp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2nppsplsl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2clgxmvey.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fjyuhqte.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nfariwdn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cvglntyf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wpjnkxxk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qgryhcmf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ivsfpeqq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2sjidkjxt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qacboxzx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bjuizeir.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kclfzicx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vuwxvfbs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrgiyjat.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2jsfsbqml.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qizlvlkz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2onhtrqxu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2otkhzvzk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcrhjbpm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nigmlhgp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ieibseyf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gcazsanu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gihfqekb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhwpohqp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lahfbxhb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebaeifqp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2gwohhhgv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhvxsmis.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vurivcxv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2syussrfr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iokmbwtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbzinrxz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2aziepgav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfejcpjn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2beyeydpl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lmwzahop.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tlibawys.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wkctemmw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mjilfgep.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cobmmaua.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2httrosko.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2omufdzie.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hawxyxlj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vkfczjjs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ttncvadt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jkqmsgzo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2okovudjw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kmoltfzb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yddgvfcq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xcapnyth.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xhpxrqac.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ekqvogxm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2brdcnbju.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pxkbqbpv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kpracgmf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2plnzkian.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bddnzrju.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xfcqrkil.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gkyvdxbu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vmijhgwu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vivzltgm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gmqnaord.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2smblaqak.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jmtpgnkg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tymmdbyi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bohzhqwq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2pcqkqeyx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fjpdgpzt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpcsbpc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vkjecszc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tgxlhcbx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2oqetvvmf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ugrgsxhv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmjwupfu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pglnzptg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rlobgudf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gipchasv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gdqqzlld.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jnyjkdyc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2knzsengq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hvdadkqz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kywqzwsm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ckmfejts.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ctdayive.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uxpxaxtw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dplpjtvc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2nmsfztdi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjyejtz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ridekdyh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwelyud.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lgxfcqnn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ipakruod.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjtnbfq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lnyjhuuq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rxcduytl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2halpqhay.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2rrgdevcs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2baquvaai.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2viwyvnbd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuaplkic.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lvajhwqv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2brzclpnt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2luybvjhv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xaoerzoa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uznyqxow.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2reybmkje.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wmmeyjzw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hotjrwkv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2argoympo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfgnhqnv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfvjrtog.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wjhhunxe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2qbbcgcrw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2toqfbjhq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfinssz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ccudrzjd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2mhesxvdj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2iixzvqwh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fnmvdpwq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aahyvtow.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwuwycnu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2oaorxbmt.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2cakjfztd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wsrhdqct.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2vjzmurxh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fohwqjlq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nzzzwdmq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2edkcntxt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rltuwphv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fircwgyl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tqmclqoo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivttpiun.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bhovbiea.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2usoevuvy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2slqrzaxx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2qlqnvjzy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xvmqehdy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2frjntjis.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vsatbdsl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gnazqhdf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ugivckgs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fpoyyagz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2cnchtddb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mixlujgg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kxujdzew.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2huufprwa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cvtetvnq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohkokgrx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rvlrqjab.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ezwtgmpa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hvfretmy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zvrylzth.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqmglr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eomhvshl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zttbdqbm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cqyekzwy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lenbdpbj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ghwhskgo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2weiowbsl.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sljcdpfi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2apejiitw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2enxyukpf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bgwkxaqy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mpxfwdvd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fskpljxr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2anopqqpr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wrsrwhwq.html


<!-- 参考信息 -->