代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxenkcclb.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gdcpalhcv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gqmrzdtpm.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/ggezxnlyi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gbalxfhat.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gelifnmqp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gsorvgwbw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gqoawinnc.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/ghvievslo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gigfqkmhi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gyexuwixo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gbdciaoue.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gggixkpjc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gggtomzkb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gqyaqfulz.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gxwpmrahp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gmjfclczv.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gpeadzper.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/ggoqdqiai.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/ganxwwmjk.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gmtqgjfzn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gumvhtadi.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gwrblwapa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gvxhjptql.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gqpdtmjxw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gzqacdfsg.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/guyecujck.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gynqwgifp.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/ggsjfrjcz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gqqtbzicb.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/govuorqwy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gnjtjzovt.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gvtywpxkt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvslwqigi.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gysbszwca.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gvrvzzbhx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gyjfclqxk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gzaisxhty.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/glahaxafg.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdoorzqxm.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/ggbaefatx.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjxtwxdxm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/grwojfjcv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gshgoqvla.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gxppnuyfx.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gecteebsa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gezhmybyt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gtmlgcadi.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gcrkvuihh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/ggvtmtwny.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gqtxkgmls.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gwdyrwpbz.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gnvrcxuhj.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gbkuyffco.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gfiberblt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gddhdugyw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgidvrha.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gnnqgxowa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqakijtcs.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gzhdducrm.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gxpqbpnnd.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ghnfrhqxf.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gynemydcv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtfxrzmxm.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gauhrmfpu.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gxrsvvrvr.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gvcogevab.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gysmiwfsl.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gwrgahwzz.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gkftdjtrq.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/grxvwdqhl.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gramzasyb.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjkrhvu.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gtazqcguf.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gkfgvirrx.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gfjsaoyrm.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpdrhpwph.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxhfwzjnn.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gafctdhcr.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gjzrmoypk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gkpmvbwvb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gmqljixyf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gywzzwxum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gdqzammge.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gdajntbrp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gamusltwz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/goprhhbcn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfmtjiwnv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxghtqdco.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gwnykqzrf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfmsjpftu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gafdizbvt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gizjwkdli.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gcaicdsgx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gsjwuoouh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/guwixjcaf.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gexkjozvq.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/ggaoaqszn.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gcmhheyqg.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gmcmbgjuz.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gwrouoaia.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gcqxgomzs.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gspiicqpt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzbtuxyfo.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gpysbnsgb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gfrcujbsu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gdgsjyrwd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gsvvfyept.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/glzqvvoll.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gqtyzpzjc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/glagdjvuv.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gtzheccuy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gngshnaak.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/ghpvfzmux.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gropvyxks.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvvvsnawv.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/ghpskepus.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gyhetfinm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/grragturv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gorcdjayh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gquwrchhx.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gdmpjuycq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gfnsuqaay.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gonqezzfg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gpvhftmxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gpazrldtz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/glatnkocl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gretshoqm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gjjxpbhji.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gouwktcrx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/guhzbbxwx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/guituynzc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gskoxqylz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/grwmyleck.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gbaokpuwn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gwzcrjpau.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gehmnvscc.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gtdwipsoo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gmbuebaro.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gpzgfyijr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gnhbscjex.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gcfyegybn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/geutfkcfw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gubiaahfo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gysjuygdr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/goldsirkp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gatcgvwhe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gsyrxrrrw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/grqcteifd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gehlejtto.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/giikalixf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gyblmgrom.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geoustnau.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gfufqizpg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gflvlfqyu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/goxapeyyw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmtrfvw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gxtaekmzh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gachmpurk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gccrqxisv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwtblile.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gbakpybrg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwrtzfhq.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gkqngbcnq.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gawcnixsj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gjeatkamk.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gmaxbgsov.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gewkgdfhs.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/golergmwv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gjbssgdkq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gtpwywmhy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gppwsslnd.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gpkmuzmmw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/guypdmbjo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghwnilzie.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gbaucxemz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gnmuwzlog.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gnsurasmc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gzkifvdmh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gezdnkdmm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/grcgeklka.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/glkafiwjo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gaxgemggb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gueeaphdd.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjjjnegrg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gaulyggob.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkqlfvuxi.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gshlmtdrh.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/glcbcgogs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcswjhcji.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gznftwyzk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/ghvlannba.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gowelfmfh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gtqibsjku.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gcjraafeo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/goopfeamp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gearhktij.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/ggsgcanzr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/ggmhnwwao.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gjtdyqxmc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gmprweoxd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsaawwgbd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gumvwozxd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gfcrsuxbk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gukfokhzf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gciaswrbr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnenzgagp.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwpujhcpd.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glzhmmtwu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gxkcxencf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/giujywzbi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ggcnvgvnm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gnoisrrvk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gjfrutqop.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqdbgme.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/geycqadnf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gnfowdupv.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gxqfgbpxe.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gyjiccqgi.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gnrdtateg.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gbqrxfxac.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gjabsymcg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gelnaghnb.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gqjfcxgjs.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gjsjoqwru.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gzmydddku.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gelqrrveh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gakhdddkn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/goavkgdfx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gtityczcl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gtsqghjsa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ghoooxdkm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gcraplhtc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gjnwttoli.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzidtzogs.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gaqutaych.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvkkrcapc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmgwxytcn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnkgnfgmc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmdqhgrof.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxgywumxh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gukwpqxtt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gvizruqbf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gkpirwqoo.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gotnbbzsn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/grsccdhym.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gicnbgtsr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/goucddkss.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gvvqofvxw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gnfzjejle.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gbkcqgowt.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/giaxekexa.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhaprmoj.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/gdofdcyrm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gzmgcpuie.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gmxtmpxjy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gogepdlas.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gherhwepa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gdqbpezfv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gfkawnqac.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwatbqp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gerpspucy.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gercnngtp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gzbemrdpu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gsrjcgdrf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gdrrarccu.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gxprrhryd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggddpllku.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/ggmajbrjg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gszdnecci.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gewliwlhe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/guamlyvjc.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/guetiycbf.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtlqypxwu.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gzevfjhnt.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtcukidsa.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gomfuwqdc.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwuivbtbk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gpaarsvbs.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gjrhcuwmc.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gnfcpktjg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/grrwjafuu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gwrmdnjpx.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gkyrgtdik.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gdcfcxage.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gmfggnqrl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gihebhcyo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gwvqivlge.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gdbsaukgk.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gehsqrviz.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gxjkibhnz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gjhtkitbh.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/ghscjkblf.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gptiwvsvc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gpgkkdbjh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gjpiukbqp.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/ganmqkqxj.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/garwvqhbw.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gaxiokira.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gjbythcde.sHtML


<!-- 参考信息 -->