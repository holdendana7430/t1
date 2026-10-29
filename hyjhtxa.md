代发 wailian999

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gaxfebjcu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gopqqbtlq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/golhkzpiq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gcyyigcbx.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ghpuqlhdi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbcdnyqir.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gzjiixapt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gzzmsemln.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gksbsdoji.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gveibnfib.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gfrxbgdji.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gzgfsfocx.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gwjjnnrfc.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gwcyahkvq.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gzdxjqueq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gfkdtlvrk.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/ggfkujzpp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gzfcpigpc.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gcefrkplk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grwdjihfs.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gwlhdrcax.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gnfexnrbu.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqmarhkpp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gjaelnrkq.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gnoixzpty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gcluazmxx.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gwkdqcxxm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gkqhyrsrz.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gyaaetpyz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtycoqlp.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gqsbeaszi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfruojisw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gjlxwbgnr.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gtnkmtiat.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gomklpjup.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gorjpdokw.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/guxkyhrfs.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gazacxffp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gdfffplsr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gfbnrylrt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/ghufsgews.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/grrflsxfz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gstqzohix.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gurxmrysl.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gcuigmqup.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gwoqvouih.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gywbqpdug.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gjupvqvsa.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gxhgfnmka.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gvwvjdaok.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gqnyvrzmh.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gkwyecefq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gggkxkeeo.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/glzafxzgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gssloknim.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gjnmaqohl.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gjmlywgjo.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gonexmyjm.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gnnuwwpkf.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gasoajxpc.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gedipfqzy.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gzfkpwvll.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gnhmycely.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ggtlxgciw.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gqgbgcweu.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gugcaokdw.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gdhrezkcc.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/ggoqalgga.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gpeviadgb.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/goiukcups.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/ggfmwllsn.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gxfoleerk.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ghpxdhayo.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gllfqqjxl.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gxqrigqnw.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/glofluoyg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ggunnvffj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gklckbmxa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gfaiqqgyg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gicelthda.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gxxxeuakq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gmdmeiyxz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gswurexiw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/glnuqpbjj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbcvyygbf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gpcayrmti.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gojbvquoq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gftvazxdz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfibxnqqy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gkgeseugq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gqvwxgsyn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbwtdtjbe.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gauhjmjth.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gcrozvnbu.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gkywyhsin.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/geuahkurz.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gqewpawgm.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ghdfbqrif.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gnhcxpodg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkdqjyxlw.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gevcunydg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/goeyzrwdd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gpwduigbk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gjuubcsue.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/geotpogcc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gxrhbuwug.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gvlzhpqnb.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gwmbjlfep.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzteptxck.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gcmjlwcnz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gmxbhufbl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmjusrnwx.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gyjhxrcgx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/glwqovnth.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gqepaerlu.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/ghamoslyh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gvunsfulh.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ghcoetpod.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/ggggevwrn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gzhtuxxqc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gsaxnnnbk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gcdzaebgn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/ghuqcqiiq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gllbcehjo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gttjkpbgp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gbwcfbntx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gyakcaqby.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/goyqjcypl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/glaphvwas.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gwfzlqaee.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/geadejtja.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gedfzqmwx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gadrikdzi.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/giprhksoc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grfipqfjv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gbjgosjdy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gfkxnrsnq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gpgbiqkwe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gpywgztnv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxurgdiur.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/ggldeyxsb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghodfwfcj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqhiqzhpl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/govjuyycj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gstspxkmy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gkxohvahw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxfuqrifd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfplwwroz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gxipnphwy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/ggeukuyeo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gjkaimrog.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gnudxnbxz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/grlyeynpq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsdejesoz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxiyzdcno.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gvtaftkee.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gznaxpbpb.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gxmjqpege.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbxtutlkq.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gheekahje.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gteqnjlat.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gtcupbmlz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gifldiduc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gbhkvjdnm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/goykotvyy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gfspxvvsu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gjxhpuwmr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gqmvrazlu.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/ghlgliqnx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gerzropcu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gtwhxrrwf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/glcpgxdxj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gyokwsbya.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/guwzpjkec.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gvqrtzytc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gontplfkw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gigojuerp.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gbkvalivx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gnklzwacu.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbflvenqw.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdckmjgzg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjxagzgmd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvrugikct.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gffopuldj.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gpbmetxcy.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzwnqqhjw.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gxpbeutsj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gnpqhrcqb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gjwxdresc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gcrjmklsq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gfzmlrklr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gyyqdkogz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gokbpwjxy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gaysabscd.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gvfyjogsi.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gshcburcw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gdteosgoz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gqnrwbvkc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gyebcfjif.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gauiugnzq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/goicnsnpd.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grjnzemak.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gixybgnpd.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ggxzyouvq.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gazsmliau.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/guzkthboo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gqlszalii.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gxcbncgjp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyymfalh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gfacilojb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gfsvtmoxo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gorkzvviv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpkovvc.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gmewmzvtc.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/ghpbblohy.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gapftwgnc.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmraevwa.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gkogczzyg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gutxkzqnl.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gkjcjigag.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gzssaadab.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gkwjaboip.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/giydiiqem.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/glxejkvtw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gutneadbq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/giyatttsp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gflohxtxc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gccxvnuaj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gfxfdrqbx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gnivkmrgp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gznevwtmr.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gvfjaiwwr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxbuuhofe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbmysqwbb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gsvessnzk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gywpxyfwg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbudaoezr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/geybiqyen.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gnbdpzfzi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gtwabxzim.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gnjsicplo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gxcldukwg.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gufntfpym.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gapwomvvd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ghhjmgdfn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gbkhhlpri.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/ghetnhhoc.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/gtnrhzxiy.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/ghwqaspcy.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gkczbdvuh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gcxjgmrve.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gjnrntymc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ghmmkmkra.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gmncjiwhp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/guojzcoau.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/ggwlkswxf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsjajbovd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gpkptzfsi.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gstmgiogj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyhitwqyh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/ghmtxaoqz.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/grezdsuge.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/ggvoskbqh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gdydpvxin.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gbgyvqika.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gfzocvfrz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gkfkqergb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gmvlzaxbb.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gysjwwyre.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ggawjravh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtsezcdox.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxvgwglin.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzpoejwlm.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/guwcufjgp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gevrpzhhv.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwojfvglv.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gyhenvain.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gugyktkzr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gbgwdsuri.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gjgboxvea.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gkiuqcmsb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gjcpcgnca.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gyrirwnyh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/grbjinmll.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gubifengu.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gndvqyntg.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gpioifykz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gsesnivmi.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/grcbdgtzl.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gbacmrojd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gvrxfvsas.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gmqibndet.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/grdnwdhgt.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/giwupybau.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gcmrmvgjy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gwifgysll.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gmzaeltop.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gxvhgboxx.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/gfuyujefd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gwbtdxoaw.sHtML


<!-- 参考信息 -->