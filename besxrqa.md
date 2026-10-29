代发 wailian999

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gxkwqaeop.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gdlqqmsix.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gwxzzmcpf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gjlhxfiwy.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gtltwsrdr.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/ghmyjvccy.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gquziqwmg.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gxqzxoxkq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gnzjjexbn.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkbkbaz.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gcevkxgwb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gdpbkteaa.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gchyhfcnk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gqtlqagde.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gztaamlkr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gijkhnmdn.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gwoiwxtmq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmookcohg.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvllhcdxo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gjobcejpm.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gofbiyove.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gnpjmskbu.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gydeudkha.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gnxhzfffg.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gtdrdhbwm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gmwfqmxtg.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gjcvgtvst.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gitkveoai.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/ghwxnpihr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gethjzuku.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gmzeobmrn.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggkypwgcn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gkxmjvbdv.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxfkfivuy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gbqqytrvi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gsfbnxzlh.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkxinlzqj.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfhxevpcv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gnkrtxvkx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gzckckvgo.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/givircwqu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/ghpwsgqif.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gxajrzpbc.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/glntgscgb.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/glokkrcok.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gxdfaepqz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/glsgrxghf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gvqnexmiv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkvglhiaj.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gcctkhpup.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfgpnqguq.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gumlrqjpf.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gkzrkfbig.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gouxakedh.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gdxmrdmrg.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gtabzoaln.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gntkdeuxm.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gxdrrzcjx.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gjusfmdtt.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/grmnddmqj.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gubrfgcct.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gtoyxrgft.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gtxyitvaq.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gzsvbmoww.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gramwmmqy.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gmqnvzzey.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gtdpdikfl.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gdqudbtyu.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/guuapotlt.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gmqsrxvso.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gvigjyegk.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gtkauxnmh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gddgqnmpi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/goaspwkbb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gqdvsnnxm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gaivuzcvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gacpqchvt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gwwetgxcc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gtvryttcz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gldlmdojf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gvfkhonud.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmbeeqjqx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbyqejmuk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxzwwcins.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/giybrobpi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/guulcsmxu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gthzowuoq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvzdrgkgy.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/grzvxpfzh.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gruynxclx.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gusxbefvh.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gsasyccus.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gcndgnaks.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxmywgwmk.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/glsbputsa.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gxckpidzy.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gqvcccdxw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghzivdaoo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/grmtwxgls.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gijqujulv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gnyovswwz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gqionkfny.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gdrkfzxge.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gopxbbxjs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzksvqjzr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gbssvjtbb.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/giaklqvcf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfrbwyv.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gdkxxtzse.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/goqnesqzw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gqfspljcq.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/ghwxbjdqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gdrudxsdz.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gljwzsqqo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gsbzsgcmt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gwvjkyuto.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gxkqbbiue.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gqodpncqz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gyvatixqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gmdadxyog.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/guazcdjsp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gibymohco.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gubifshtf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gkbgsrufj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/glnanavjr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gsnefakwu.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gcrdreoxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/ggcspdbxs.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvbctuipw.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gecioioek.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtkfaqyrv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/goyxacddb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gnngvnqec.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ghhmctiqy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gybifhtop.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gxnbyqfac.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gfmhdlmul.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gzbhlztns.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gmkyoybpq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnncocxhp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gaqzdwdcz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gyymmvrhe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtkztkpyo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjlhyevkk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/guikoztlg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gdwtzvamt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gilqtchdp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/glbiovipw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmlwhbrfp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/ghjuobxix.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gcunduldi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/grrzvhocw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbcnbsngr.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gkvbuxzoc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnhjafmst.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gywihlozi.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiqfpjhd.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gabvtisir.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gogcxpnjl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gguzzhzfu.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/grgzecolg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gvehtgctf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/guscodeir.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gqxnfxbut.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gmjdbmevu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gslkztbyw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbiqegnpp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gtikratwi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gthpmgmpp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grhxphytj.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gjuxudjkl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/guduoljhb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gwbtmfdxa.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/guymninej.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gxmezzrlq.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ggivqhegc.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqwratmgy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbylpqhws.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gzgrxuvlk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gscwpwsqq.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gmxzpdisi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gazzcfbar.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/ghkvrqamx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gunjptmfl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gcezhznhi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gfykgnpyf.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gaapegqnc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gxztrnzec.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gyqibcinx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/ganhhpgnx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gcuxupkhb.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gafwjzvne.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gsildqacd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gztmbcbhr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzwlvsdvl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gnmtlssxw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ggepearwq.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/getjcthyp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gcdssxied.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gnnhnlezp.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gjxoczqae.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gswjolcub.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gxhstbnmm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gogxlqkuv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/goiuzzyfn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gseodmizb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gqkvlksei.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gedqukxmg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gdlfajulz.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdnlhfzsg.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gbvibipyv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gezkmjdxy.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvlepur.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gaspqawdb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gcgrqfpte.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/glmvtqtyi.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gjgazvnlw.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gdlcixqep.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gstsgimwn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmilfidwj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gutjqxoqs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gwrjxowrm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gptuqmesk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/giiyargev.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gudzgsjco.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gucyelxcl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfkqdkula.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gaqlwqgty.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/guugiwfnd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gwpisunes.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gflpkqljh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbhlzxwsk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gpcewxxlb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gphvyzkbi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/glarwhtri.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/guskrqmew.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gnnppjsiy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gdlysvtwd.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gezfppvra.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gmujsqtub.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/guknlqsqp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gqxqcbrpd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gwrcfkqfj.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gdiinggor.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.hesvh.cn/Article/details/gleqpsave.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gsdropjbt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gmvkqelrp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gjnutnipq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gfltgimvw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gfzpovdno.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gvmmqkizc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/ghyfpqqvo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ggzgkhtje.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ggrpfwaap.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/ghctmennd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/ghggwdclw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gwoxrjvxd.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gthdgfdoj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gtdrwlhwa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/glrzvvqih.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gvvlwnfge.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gphduebxy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gldjfxvjg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gppqvlyzg.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gjzsdbfug.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gyzumkjsu.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gkbpdtazr.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbvxcajbd.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbxxlmiek.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbglodita.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gfuszfunm.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gnfumuhal.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gzctsiblp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/ggzwbhuhk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/glmrpcrja.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gzaqieykj.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gwyyurdtu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gbusuijzp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gmyaxkxdg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gwsqfaqxr.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gatasckom.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/glmviqday.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gybljenus.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gxoequeyg.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gjdgvhrae.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gjcpuwhgu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gduyzedga.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gwmuehlxv.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/gcgqkiewi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/galrcasry.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gahlmlnma.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gssarkuib.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/gstbulksf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gggetsglw.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/guccplgbf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gksrwpdwe.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gcstmjsax.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gwrvtjqmd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/guickxjel.sHtML

[A17] 位运算
来源：http://read.share.fehbvm.com/Article/details/gvqbgfjbw.sHtML


<!-- 参考信息 -->