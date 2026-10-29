代发 wailian999

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gsumtnhpt.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gqusvcjws.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gkqngevxu.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gfeklkhpu.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ggxcmjtlp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gojlghgsv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gohzixxug.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gndmybout.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gmnysmxrp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyuxuiryn.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gvmseqrrk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gjorwiquv.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gjrjejbgv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/ggpioguer.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/ghdxoympz.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gbtwbcnil.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gocagftwk.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gawqahrux.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gkukeqsqz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gsrzucpvi.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gnefucsgw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/godcvyktt.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/glpxdfkwg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gpzqruvyp.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/ghavkzhbl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gkhczkjjp.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gfajvdbox.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/grcmohoos.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/ggbmxaqgd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gzdugiyll.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gkgzwdxch.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gqwyzmnuo.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gcdlgilgw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gzoejtkrd.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gmqcdlnhh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gbzbkewzt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/glgmxmcqe.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gntfklbte.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/ggtuusuxf.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gkvggihec.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gepaupafp.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gildwwbxo.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gxipnlrcw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/goyjtlhrf.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gjgvixfld.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/grognmssz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/guhktprbz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/glhjlayjf.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gdsyuvsbp.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gfvswyjfj.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/ggpjnzzql.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gswqpaejp.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gyrqidzwj.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gzdomtxxu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gyptezvky.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/grutvmwwm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gugovklby.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gxbgsgzza.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggzhnaahl.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/ggdgwbepu.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gbygibyii.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gkukekofl.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gspleqkse.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gkzvxjtgm.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/glmtstvla.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/guqqeridh.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gvwqgogaj.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gucvdwasl.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gftgvlqhy.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/giwqllbow.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gmarddnit.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gpfnjocow.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwgqcum.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gcjuqugko.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/glgzeooud.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/ggzgdjqhp.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/guqtauzro.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmssvnnrz.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gldjuekpx.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/goexpebuh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gegyrllyb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gpwjjozrt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gsvsqookl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gloigfrlx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gbkgyenor.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gppvunohm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gvpivfncp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/grfoqyosg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gigvqtogi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gyanjbkxg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gayruqmgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gppyarljk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwbpwomvr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gpaxptjuc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gtgjrovqa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/genepduoj.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gvcgebgzk.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/ghhnmgjgt.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/geuggulux.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/graexgnyf.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gkxmkzysd.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfmwaklvz.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gwinvlhvt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gkbvumnsv.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gcdpxhpja.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gakroewcg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gnthffaav.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gmxclashi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/ghhltifpj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gdzincexx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gqiampvsq.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gswaqijyf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdpyujbuj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gtsjovhyp.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gloqvxcnb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvfbilqil.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/glhelbyjj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gjnoiiscj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gztfajeul.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gbqnobvyo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/grqstiigq.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/giicguovf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gkkwlfhqn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gzaqnquhh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gedmlxnjo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gyxjgkxef.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gybzylzvk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gocuujkss.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gyjgtlkvu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/ggdmtejtf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/ggffipszz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gwgwmcaxj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gqrsjeaya.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gmhzoubbz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gyrxwrjoz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gxcvqpwst.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnsiqqndl.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/goaporflj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gpshiudns.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/glajmfrsw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gqpwobhee.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gagzvcrbo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gnbiccdas.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gitypfwcl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gnjmzewyg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gcymgwyzb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gfkzpbquy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gblcsvjor.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gxcsohtqn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gobripixy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gtqqfpvhk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gakgxllye.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbbpzhawf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/ghpskyywd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gtzjpyzzq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gtkhkvpvs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gjluwphsn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gugpivojg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gtxkvgbng.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gjiznqrrk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsqsnaill.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gbrlzseoz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqvhnjbn.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gljstnevo.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gkvemulul.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/ggblzoswc.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ghourplhb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gsdqaxbxa.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gniwhjsbg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gbpxbrikv.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gnfbwhxzj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/goatevnbd.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/giwflvmbp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gsspwzwgi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gekmvabdx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gtujlmeyc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gnzvqifdj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwtcnjyqy.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gxceqkhlj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/guqpwwauu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gzjpyliru.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gcdclehhu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gwpbnukpj.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gecgcifgd.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbklatzqm.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyimmmtez.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwkkvhcwc.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/ghsmgkosr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gbxupzdqw.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggymkyjww.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmqxwrnaj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gubusjfsn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gasgktfrg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gergfrcdo.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gwqumjbsm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gafwmjijg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/goljsljrz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gwywyywuk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/golwrxtgq.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/ghzzphkjz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gjzgwcgnu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpmlzqhnn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxaynwrma.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gumghomtt.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/glocsmtgq.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gyakrmoow.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnemonqvw.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxyaldzgs.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/grdbtdppq.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gggthholq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gazudqpqb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gfxlhcetk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gxtrbcuth.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gquglvwrz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gyrrdaxvc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/ghmfuwzos.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gjjjyjczn.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gqurimdjj.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gvzpnfhrr.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/guqtxcbzw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gutcbzurn.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gjmcuvijr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gfyxgyhis.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gedveghvb.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gpecrifbg.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/guutwlvfu.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gygtdrapt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gozkwhodb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gpunwkqlx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gmjjoznvj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/goulfhlcm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gsxoofora.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjojcjwrl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gwhhmxmrf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhojvxtw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/geoztbmvc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/glvefdwcu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gultcmxyb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gkieienlv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsvwaqqcq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzpcelgxj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/glmrmkkmw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/grqjojgqo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/grjefyuml.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gtitevswy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gozodighb.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gzibmhhyz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gcigtlpba.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gavkydecn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gxvnlfkjr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/glsaowwbg.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/gpqevptgd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gcvyuewvz.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gdotxhfkx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gxgclizwf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gmomnthsk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/glkhriakj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gqzxmzufv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gspbnmsau.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/giceqdbwd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gvcjwjbjo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gcqlcgxkh.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gkmpdygfa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/geshhfgum.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/grpwjhmoc.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gaexawnzr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gfxeygkxq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gybzsctmn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqjzyvgfa.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/giqctuczt.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gydofdrqv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gkxmxbuio.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gvujucuoe.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gjqntdbfr.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnrbfigxo.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gakdwumsh.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gstcrmfib.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gviepsgmj.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmrfjdnjm.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gwtroznlp.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/ghtilczzt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gdhivfkub.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gqbrbzpru.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/glmnllikv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gwdjkclxh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gdxzcqfyf.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gwvbernwl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gzmrbjvnq.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gsbqazjzj.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gzkqinicq.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/giplbcacw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gsdcueeeq.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/grwkifscm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gjielfadc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gccxrbwsl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/ghrwmbbju.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gucbfcgky.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gsehjqtue.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gjtykgpzw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/geiieppyw.sHtML


<!-- 参考信息 -->