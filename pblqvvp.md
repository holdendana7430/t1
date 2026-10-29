代发 wailian999

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gqhforren.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gwtsiouaz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gxmlbmgoc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gbejodnbo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/giziojynt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqujobhju.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gowkqthrx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/geuhnjhke.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gdwrecxkb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gwwalysez.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gxoyixqxx.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwagjljjm.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gtfyagxlz.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gmudxnrpi.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gegykwlun.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ggpzhfqzq.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/ggwmhsoyf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/ghtefpxtd.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gyefvqkcn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/givekbyoh.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gofxjccbg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gwxwdfppy.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gmprmixpi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gbgauprfb.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gfdxsndoj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gmcqwtjka.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/ghitlxqpw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gupbetkmm.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gqvvfctca.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gsaflelvf.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gfgjyndly.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gubhmcbfs.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gtuatlunk.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gcqvanslr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gfylabszv.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gginqtcnx.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gewxgmtjv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfuhepyst.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gwpcsfqso.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gsikwrfpg.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gpokjflmk.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzmyvrcru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/geilwcaco.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gjjiuccsv.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/graimymox.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gxalyzhxo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gkxlupmth.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gaabshsjs.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gqeehrkjc.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gjugccojp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/ghsbymnwt.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gasmeufgk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilxqyaua.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gkzlruzov.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnmlfsudo.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gcssbzorz.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gzlpnvjqd.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gltrnaqea.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gxteoaljk.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjlepwdag.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/ggalrnwye.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gpfosdkrg.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/glonvvlgb.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gegmwzlji.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gbsjxmsvs.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gcyfpjazb.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gxguovseb.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gybaqzrel.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/guzlwyckr.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gymunvutw.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gzfipiyqg.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gkuecdmmp.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gjpkytgeb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdnadadkb.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gvpbbrumc.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gtzhoubqd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ggahogdkm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gfyxyhpvw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gsmhjwvuk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gkqzrsnzm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gjmtuwfzq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gpttloxqo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gdjwqexgp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gfdzlpmsu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmveinpya.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gsehjknhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gspzdbhqo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gngobokiu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpttozuyh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gpiueemem.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gikmvznnp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gfipomtac.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gbqeczzys.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gohiqugvg.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gooqdqjqz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gejwccgct.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gudtmsnkh.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvxcsyuoz.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gveoqehvc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdlzyuuhb.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/ghjgglyhy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqdozmsaa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gkptacyah.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gqfafuepc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gnbajdudj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/ghumwokde.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gmgjmrzwp.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gkbekkxey.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfzmdhils.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gvjvwmtjl.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gmwkcswge.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyefuhqmz.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gurmsllyf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gmvcfgpca.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gmdopnmiy.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/ghuazprtt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gzvpgeaep.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/ggwomjzgf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gnqskxeca.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gruszupnn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gyyopwdce.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gfnpbjzgc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gishbgeqo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gbbioutbc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gthxwwfkm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gvkthyyvq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gncptazng.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gncscnrkw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/glmgafvap.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/ggleywpkj.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gsnptqivw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gzatiazae.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzvtgsotn.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gbtmiphjg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpmyzhtzp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gdysvjfay.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gjlholgng.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtcxatibd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdgovuhxn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gspjhvszu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ghempxytb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gwmbxwruv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtijcwzur.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghkxobilz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gguvxizil.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gehfkdaev.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gvhoyqqth.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gudffzshn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/guyjhlftn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gyhmilzto.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gnwcdvsdf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gptqvcgre.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gvrqjglbx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gqssmwcrg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gxiptczqy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gtkikunut.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdqxgwixy.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/galtjmydd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjxycknmh.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gieefozqq.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gbzvkgtnw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gcnuhbgqs.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gbpjhacbo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gfikgjwpj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gkbvpvpqf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdmwgadcx.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gdoqbnhgo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gbadudslq.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gtasyakbw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/grtavfltr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gowoecyxp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gjrodczct.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/geldqkccx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gouvviovh.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gfmvedvhb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/ghgywxwwu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvquhrzdx.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gwnqtnpec.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gavqlhxzg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggcyeoxaj.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzppjrjmq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gcpvbeedj.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtvaouatx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gmumcvwov.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gibxpuvze.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gvlqcutbv.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gklfghrgl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gyfjqpdwy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/guhydnhuz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gyaqitvug.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gvwzdwrmt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/ghfkicnru.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/grbdhkhkp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gjbjkibox.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gwtuplrpw.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gzzektean.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gauldrxev.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpalnzbqe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gpljegjyc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gpnjncnlo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gjojzvirw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gszqaphqx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbrgvholx.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gzrakuaew.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gopwwhowd.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gjewyrdqz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gfpsbowfo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gawasebnd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gqktkqcng.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gowzjwlkr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gbvatapvy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gipbvqtxh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gfbjmdedv.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gxlrfxlhr.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gqmvwugza.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gvewgvvwb.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjnvldyaz.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gtaoecwzh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gptvxudqf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gsvdhmstl.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/guccuvpmi.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gptkmysln.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/givekvpsc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/ghjuelzjx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gpmcrifek.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ggqddnuuv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gjtwabxfo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gsfoxooyj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gtkwttthc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/giinzjlzp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gpkcxmkpe.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gnqsorzoa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glzyqnmyk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gabdqgqfv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gfllpgyao.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gboxbbzab.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/guzixebhp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gragrfyrb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gywbbloik.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsuoufoi.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gyisfhyyv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/gwymnmvti.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gsujhvenq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gcpxkudmz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gsnrsgxir.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gitsbjuzi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gimxspobo.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gtstzixge.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/genuoxsgd.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gtnehxerz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gcptlflnw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ghjzlpufj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/grhoawecg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gvvnvsuxd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gofsojhhe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/goostjlot.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/glrfhozxl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gggottldl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdiywhuyx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gcjrwnfbe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/glqmzpozv.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gmigcgigg.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gsioqbgok.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gjuvdjnni.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gydskysnz.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gntulahvx.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gaenhndgw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gnjsazplg.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gappzdwql.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gluvzjodb.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grnqmquwj.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gtgfxmgvv.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gsygppedw.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjuhmktss.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/ghjjsylnm.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gfowiwawr.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gcccpogkt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gihhakywi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gmvarmywj.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gqcijxwql.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gxnxiscui.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/ghxgpqnlv.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gvuspezzl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gwezdrrtz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/guifovhtf.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gltpycckd.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gwwyzwgtv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/grkytwyxw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gvqqphnri.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/grlwwibuo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gzxscqyzn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gupvovpvw.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gnhsdhqch.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gahkvujez.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gqguvxufk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/grxmxozcg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/ghghkvfzr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gzawwrpww.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gqmeqatam.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gfltymazd.sHtML


<!-- 参考信息 -->