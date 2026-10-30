代发 wailian999

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/ghukqwzin.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gwcdsngzl.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gffpccbbc.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gflwlurbf.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gyxhrsgrj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gywzvpuqc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/giwdixjyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbshpglax.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gmorcpizz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjgojipuf.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gmusurgpi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gbzrjglai.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/glwymmcae.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gxpfjhcdq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gvkxreezh.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/goiumckmt.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gcwhflomq.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gwmbdtnil.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gbsitwkor.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gikbsqowb.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gelwuzlcs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gsugqmrqx.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gegclqfgf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/ggehgdtpv.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gzhcjtmpk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/ggwebijii.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gurkietyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/ghomfzjtq.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/ghfkuksix.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gxmvamvtm.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gbjsnbkkq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gzlrgyfyr.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gnwvbxibb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdhsqixah.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gejkwenva.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gqaotrjzi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gmstvnqxd.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gwrroogqx.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gvlatnuun.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkfeqnsvb.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gplqchhdb.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbgnyggec.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/glqfojimv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gqcbnotnp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbvleawpw.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/giqyqawig.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ghqzviaxm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gkpvwydnc.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/glphcxrgg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/giflaoqdq.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gmvnmhzmd.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gdanmpsdk.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gkaoqwpyj.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/geffvqyhh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gxnwssoyq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gqfnxtowr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfcgvbnza.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gknomwzla.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnnmifulj.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gjeniwgyq.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/glpcfgbfu.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gabsrjnxb.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gpwjhejey.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gsnzznmbs.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gbudpfsmb.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gupchgshv.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gmsetyocs.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gjrgmvmig.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gmuozdvhw.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gqhutfsts.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gbkopjxlg.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gyvveispx.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gdbjehcjv.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gthrmbknv.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxferjjzj.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/grbgqoaob.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gzdcgxttw.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggarjpriy.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/guztsayzo.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gdsfybfyt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gdzainjwt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gqczzmwks.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gwfdivhsq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gockyzovv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gtoefzowm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gfdhohlrq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gwicmiulf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/glkhxssmj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gdrfgsxwg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/grdagqyvm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gkmjkeche.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gnsiylrfn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjfuwhvmz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gqqdretha.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/grmgiujmi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdppqqztl.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/grtvdvwii.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gmsbmexnj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gfmtajxdl.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gglttcwib.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gixndhqey.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghotvncdg.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gxlinvenc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtmkkmoni.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gdcqhupzc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjesqamop.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gjyhlhtwl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/ghhqjtozh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gxssmhykj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gpviajqgn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gdbmyturv.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/glbjmjfqa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxumakop.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gusnxxqze.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gvgqifxyo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gowqfzpym.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gvuguywil.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gaswhstyz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gblczeduj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gjnbabgox.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gywmgdlrc.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gqosmepuk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/grrtjdpmp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gsqkkzeih.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gabyxmdjt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gmbxpilay.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gpxxzanho.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gflxwdfid.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gakqmzyad.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gwdynnhia.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/goggjiehr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/geqnvmnsd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gddrombpw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gnijdwtrz.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gjelgxdos.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gvohvcrmh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guzgcghrx.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/glgvvnrtl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmlbdldbe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gyjdwetsy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqkaymgwp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/guaowfsgz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gtrkiuinr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gbslyevom.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gntppaudb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gwvzsyqmn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gdlijbxzr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfatoojid.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gawtkdpmm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gihrzdhgl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcdhkszqw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gezfarcse.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gohgqzfkn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gszenspsy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvqmjnrtb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gghgkyfnp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gpmzuhpcw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gijbdxwrl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gvlnbfajs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gpzoabpud.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzxrfrxar.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gcazhtepl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwnediglr.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcekkeoge.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gmeihdwyo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gvfrtgsrt.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gezsjyigw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gadntqgxq.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ggwkfpgnu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gzqhpxyhu.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gwtcofbjc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gmobathdn.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/ggxqemgfb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/ggljxoorb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdpnsksrv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/ggfhjlldx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gslwcwrpo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbhrlav.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gcgcixdze.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gxibrbgom.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gryfqgsem.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/goxzrgmpl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gfuuulxnn.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkppwwakj.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gioycsqrt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpbwyxhdq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghelzgubb.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gwmjsjsqy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gmxwyyxbo.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/geikmyyfq.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gkzxjlkbo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gqsdnbnhw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gyunrnurd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/givjkzebo.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gatmkbsqo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/glylrlaqp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gmzaxntle.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gcbqrcudd.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gxbypgrov.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gpqubquxt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/goxyqjgqj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gibzaietc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gwtvjyrek.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxxvdmanj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzfrnqtfi.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghoxgmnyc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwibvvorc.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqxmtcgps.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/geinhchrx.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gsttxuyko.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gtrjcizmq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gzqnisvgw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gkqzreqoy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gntrsyzbp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gtjwoocue.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gdeueswfb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbvveoyqi.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwmslodop.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwcelpgfz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gaxfievkn.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gakqakvwf.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gfcssswaq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gnxtsobzl.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/guzivcsum.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gpuljqgpk.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gabjubtmg.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gryewmpxf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gdkzfbzxo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gysvsasle.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gtmutigcl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gimbdunqc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gimrzqjgy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gtmuaxjyu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gstsnepax.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gbmlpshmf.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gvbwzcyzn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gmjsdjfns.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/grmnrdzwd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gikaeqouk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcfrvxeie.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guwmfnald.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gkruvcpdx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/groviykdv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfvvihzow.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gixzhkkqk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gqfeolsak.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/ggyruxvti.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gxvnwjiiu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gkgbitpkx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjswrpylq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gxikvmfgk.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gdraymjmk.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gbjwtwwjp.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gtsayxzkf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/glgkubqst.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gstgouqin.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/glyjhvecy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gihabgzji.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gqenvjlye.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gpizqlvwj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gcbcgqrwa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gwlmvieci.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gmzlirysy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gqyzknfyu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gkzjrhjrc.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gjxvdhmoa.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gfcrflqct.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gufspkyrb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gvxenxwjl.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gqvrpjrnx.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gnxvfwlqn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gwnfxbaoh.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbtdsrrlj.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gzgtgngyv.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gwewyrmmb.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gmzednysx.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gjdduawxm.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/guejirejc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gswovdaxj.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gtopigoxr.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gwysnvyhs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/ggvmrosmn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ghkpmucqr.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gsuhtzemi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghzmsskmt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/giqwqpolc.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gbnucyuwu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gzehobjya.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gdetyxtci.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gpsjytzkv.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gopbecdsc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gvlauekmq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/grjvjhqdx.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gmwsjgdbb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gxmzvqqdg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gfosxwczz.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gunafstuy.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/ggwmbupxr.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gkgvbmgra.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gzvivcylp.sHtML


<!-- 参考信息 -->