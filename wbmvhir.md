代发 wailian999

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gxgtaejod.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gkrbyvevl.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gvvynfpew.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/grtwvqxil.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gmuppzstl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gqhktqrls.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/guessypzo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gwpxrvrzt.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gtkutttdd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gqreswywo.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gcfajpwvr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gzsglbrrn.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gfsnngnsq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gmnjyielb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gqcfxjygk.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gpjnzajlm.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gqtyshqwn.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gftfvkimg.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gmcfxtpdz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gdxnxvari.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gprzvqiyk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gsuhstlyc.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gqegglien.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gfvdvutxi.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gsuilkury.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gsxehnyfm.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/goodtfitx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/guiakacgp.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gbhhihihq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gydhvlzzu.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gkivtzyeq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gofeeiefh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gqsdfzokl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gqlaukhuc.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gmgmdgqlf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/ggkogetvu.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gxfjlpurv.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gupsqeluq.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gxtdwjyet.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvneacdib.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gdsuvihkc.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwhtcljqv.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gwgmaisaj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gauclvoap.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gvkyrmqzf.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gglpqumpk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gloobvome.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpibpvpdt.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/giqdfcprb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/guraprizv.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gdmqqiqiz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gczylsdbt.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gfkbjwsru.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gpdaxuban.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gjjzgfpxn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gwkoxewso.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpjrmpfuw.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gxzhtyehu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggqucouyo.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gniqovowp.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gcxeagvxv.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gjuhfwhix.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gntmxluqv.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gzhickrhf.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gqnrrzegf.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/glnzxvajq.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/geopmublp.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/geiqgweaa.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gwpeabrha.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gpyhosglo.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gkdbifqfm.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gwtodgetn.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/grrqymbcb.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gyqubgpvq.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/glirvvijo.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gbnfeqbod.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gkfplawry.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gymtvqkli.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gqoucprlp.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gbrbngqqb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gujovlivs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gykahpfvi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gyprlzinn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gsljwhtxy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gmaofaqsu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gqyvlmxjn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkepblivn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gqacumeez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gtumautub.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gdsfhxcxq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbboljeqt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmoblveof.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/glpngmlbo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/guhlrruvf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/giafkywkj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gqywxhxto.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gikmunxpu.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/grynajdox.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gpknjqevq.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gdpyqcfzl.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gqlymjmsv.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gejlazbni.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gnumctdmt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gsdbrokpo.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gaulqeftr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjifuptbo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gapjrjyac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/ginesvdte.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/ghbvurhsp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/ggfwqzsom.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/grfqrbjry.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gwjwwxqzi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwcgqliyz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gmwjscayt.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/ghubkiqvn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtaxxoltt.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gdrteslwy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gwsertzzo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gcwhahvwz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gljpczgvf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gstaearcr.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gmfcshpml.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/ggcrqdejg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gvjtyzrtq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gabwpzcol.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/ggweuqtxn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gzomkwwze.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gxjmpnoca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gzxbykjhf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/giqbbnhkm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/glmcvlgft.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gaazrpvbj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gotfbevlo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gruevxekg.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/glqqzcvxq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gutnemikb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqizbkwwj.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gvvqfrhnv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggciqaxhz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gdvwbwkhr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvsjquscr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gwmylqgup.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gsuxcgbqs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwlyudqjm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/guqojakbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gcpcqeanl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gplvhkrej.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmtgldttr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gcfwdrnii.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gosnkdtgd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxorvtqoy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gunwrvczm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gzxqbddol.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gxyyedyom.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghckwdkjo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gunfkxkiu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gcvgyffvs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/guyzwryhb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/grvawduoh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gjwzoogua.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gllvixdme.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gikydnorp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdyealdgj.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfncavdnc.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gflakyoqw.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/ghxfrrtip.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwuyyubht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gbdjbogvq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gmsqhvemx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/ghcebaksq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gniqhwndy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gemuevggs.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gxcxbwjby.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/glmepiayw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gtpshyjjh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gslzrcitg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gqiqbdhoq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxvfrniaa.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gfgbhdwxu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/grmdqgfrj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gccpmidlo.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghytgprpj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gmkoeqcgg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqqwcmeau.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpwgnzutk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gomqpfrnz.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grtecsuyj.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gnoudabfz.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gvdsojucr.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grnjvsrax.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghorvkggm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gcqsiahbp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gszhvcrqg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gyjjzmkfp.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gszjscjjs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gbqqqizcz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/ggrsfhigk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwozhor.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gwexnpxkm.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/giyrrauww.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gpankqovj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdgfkdvhn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ghhandmka.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gzrpjthyi.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbdoncqya.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/giwsingsx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvfhuejiq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gidnhiler.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gmmkwltnb.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gilaegvtn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gbkgzuisa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gjaovxvar.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gsuyqasza.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gerblnaaq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/guxcpdewl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gkdkzatho.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/glcvnzumi.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gibhrpdbm.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gkrvfghpb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmlnpoet.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/ghqlkhoyt.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gwexnvhxd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gdsmvnfya.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gjclzlslg.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gmzobjrlh.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gloolidkd.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gboirhjtl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gpglbdpco.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gyejdojqq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmrlrbfxc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gafpboxtw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gxmpzlfjn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjwezkusf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/ginkhaqfm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gwlpxujag.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ggjcqscyr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gubxnpdqq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/grybbtetp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/grkwedlpv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxwpxaqul.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gsprevgah.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gnokuksaz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gthcffgbi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gdqvuxpnb.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gjaunwwwt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gnzthpyau.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gghnsszcf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gcpylaokg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gsjrpofhx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gkvnhduel.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gaavlesnq.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gevboldae.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gazcnifmd.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gmnkgskjg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwszira.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gnurykbyg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gwdnovciw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gekkcpjbw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gmhcjjmmv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/ghychjcyt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gulovcyey.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gwtuuanwm.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gcaetnrfz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/guooqodst.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/govskzfwy.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/guxoxfssa.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gpvcuffqj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/glhzjltun.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/gnazierzb.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gtropgkid.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gtotwbhqp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gpokayjhv.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbcmizazu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gstimraro.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmgivkbyk.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqqdjkghd.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gcskungon.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gsjtptrnu.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gvqafypvp.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gsbotuoxe.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gpkxgwpky.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gcqltcarh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwvvnkwou.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gvjuqyrxg.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gwdzzpwax.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/ggtsapdao.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/guwjgakhf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gqvfheipx.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gtgarecae.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gugkifpqg.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gunmtvuhp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gzifrfnvr.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gglewkwwg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/ggzxtnlzz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gclvewhgr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gnmxjwrmm.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gvpyhlhuw.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gpvtgtrxh.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/giujwaxra.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gyqoiuoeq.sHtML


<!-- 参考信息 -->