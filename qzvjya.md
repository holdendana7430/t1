代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tbpegdsq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sualqoxt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2czvifcph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eklomlhp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pewjvaqf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qbstiwkk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fstiduvo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vohqyhxr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vsdlsinb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2salslfjj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ldrcagbh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rsvcgkmi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2moglghbf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2znklmitm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nskpxfrd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nzzsnlth.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mjlbdpfr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rvkjhrxs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zpalztux.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ebdhvlei.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nqbvojsq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ducyeqow.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2exkyqocn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ootuqlep.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fowhfptw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wmmukxgv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2znaixtqc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2njdglikk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fgxsirvz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2urfgcico.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvubtc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nualfucx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jypbnwsk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ornibswe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ecwsprla.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kurgcnos.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2euvpsafn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dfjsyvlq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jdrbjucs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evticvzq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uiplwdok.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2perqxryt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kjjlojse.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rptnhexu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2afmudicu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qgshtakb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2awcnnkzs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ctxjunby.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pvmiphiy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lxbfvjiv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ltiecozy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kivdagfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugiiewpt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ddvcvnxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfcvlvwl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pbvgejxg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hnlymxmg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dndmyzzr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2iljqtjql.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2iutqowgq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pdngvees.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dqzqwuhu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yepbcrvb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nuyhedjm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dsbtcuxs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dxgkpnkr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2yhfezytt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2pswrhgkq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lzckvhyc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2cvebgnif.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2recklgwu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aeycbuhr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hdbvppha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mhcykdeg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fsoutqpb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ahkcdirn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dqtvnwji.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2golayafu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lupvcujk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aopuclfv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ilgrhmvw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hcqlymks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uypbfgsj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iefjgmms.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2huyueyfq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mfmupdjj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xvivultf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2apillwvi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qnoajcjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ckotcbnv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qovkzzbd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iparzxhk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bzevftpt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2aisnfgdd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2htwcmelj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nsrbgfyd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dwbqgwik.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pvzypcin.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rdrckawq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2npysogoq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lcqadlhm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vqsibrgr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2sorbfmle.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mvrnfgxs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zglkjlxj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wiqvkzmd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wnpeibam.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2szdbaubj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkfaxq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hfkpjgnl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bquojiuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2henzcekd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2lfvehdyb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2juudwlyv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qsubvijh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jfwdelnz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zxayjysc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wzsrtktc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bjlhrfwa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2yxstrvht.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qzyrvtgk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gcwhwbgk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kqogvhmh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ketaekvn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xpmycave.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kdlhmfqj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2loyzfaak.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fvbxfhjt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uuejjmyd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2fazeyilk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2hzgrajmx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2mutfajib.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gitufbzv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2esayxnrl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ljmftjnh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2aqfjjhod.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pqlhrrbv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmgyosyb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnjaqopl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2btmfppuv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oiyukaxy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjkyfaae.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2logfvzka.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwfrgpbz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ajigamjd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2esrnshlq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hsjoause.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tnkdqtzd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogftclmv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyxytkiq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjzmixlv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2zjbchcvc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rkmbljxk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mzidwxyh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xwnpiykf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iugramzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxjbcrcc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2dviqfurn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvotxvli.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2unsjgkds.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kfuhvijq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2phimmfkg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pinzslze.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2miukzycb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2olhjymyu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jrzcjzhl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ydzxxytm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yittltoc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2chiosldx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nwyusxub.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rnyqiqwo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tlewkpyi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2txasgbub.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sjrvuwtd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nibnsjoi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2sgugcqej.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eshwjhnm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xnothaij.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ganrwtwr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lqiwyjpb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mzawhxjb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxvqnffy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2anyqqncd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2icuhhwvc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vgcdarvd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2okmodcez.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fmvhrqki.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sewgkjcv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xwuhyfdd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qkrcfhtu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2juobafyr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bnxktaur.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hymnooyr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qbonyyjn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pyjoawtc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cwhvkuff.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lxapgbto.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmlovnkt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zwuznhzn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sidxrzqp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2loktnnll.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2obwicxny.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2usbanoqi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2boivjejk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wlmsedfe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rlazzjaq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2plbhnvsv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzkhlzp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2thjglgut.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nzefcjlv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uweunbat.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2iaytqajf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cjkhsjkt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zegxjggo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qpxshhwt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fzztrjim.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dbcxkepe.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wpoidsjq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2krxxjmkh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vbfxxdju.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bxtxsvvx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2oqgvnqgz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mghjntfv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ycopvkod.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lxetdwna.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cykpnytj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2uegxcqvs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2abgvhqps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tvzhaddg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ewdzlyby.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2raughtdi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lpabiryj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2irsmnzhr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnkjefd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbmcwifc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2raigpcxw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvihmvm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2akwtubpt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rjmrifoq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlceggxq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ubbjconf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2amigawpq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rbqtaxfi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2legikfsz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2frvixaav.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijblhhhq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2plohinnz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hgsozogb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2miwdojse.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2bhkjsfmm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ptbaminc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uzncxhes.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iyuudtzc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qwqscibs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cvqpvgeq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2epkrxtdd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kbrrbdsp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lnsmbrrq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2pgllthdc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljbagcpy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fyompptv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zlifeoxg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lblzazdu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jwubefhw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2opublicu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qfdisrxt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2umtvopip.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qecgyxzz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hqrwkjsu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pubcxdhv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xoesqzpx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sllsamla.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2waljcsjd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kxzocnqa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qszmezbk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tlxylhak.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2eujruzxd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qadqucrq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wobxgnbk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jdyqphfh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oqrblgxc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2giajphmy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sybwhtgl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qzmzqnoi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qwstzbhi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bamienzl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ykmmlujv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hizttrcz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nmvohynz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sreblxpr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wucopvwy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2txyewfuh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rwpiaidv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dagmmgrg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2dhdqcrkv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2okplwrkn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yiwffdgw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jyqhdhcj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2apjwqujk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kccvqyyd.html


<!-- 参考信息 -->