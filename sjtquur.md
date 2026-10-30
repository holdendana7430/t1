代发 wailian999

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/grhluouax.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gfcglrarj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/ghevrvxrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gunqgvvcf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gcirpyjnd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gyxrnrmlv.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gmrmvgfci.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gpukybmqd.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gtxfiwyil.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gmpkktwmv.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gbidxmrzw.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/geqymlmry.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gfkzdhhce.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gnxcjwbru.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gquhibviy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwoetdsff.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gwdmbfimk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gejannyhd.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/glwdltoso.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/ggeiymabt.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gdhjvxjrz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gmqsiythx.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gztbqjtow.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gwmlyolww.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gkupdkges.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/glvwnyyeu.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gagrqcblc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gnfxfkrma.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/guatylpsm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gvpieezan.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gachhfoxa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gyusgddoi.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gtdlngxak.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/grrzbqbll.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gminzicmc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gqusetrwk.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gfyoahshs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gbherbgpm.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gbvczpofj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gmwpzgrkb.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gdhevmqca.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gboztlvvs.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gjotnsysw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gggayqsfx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gfbcnczou.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gayvxetjz.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gzmhbbbmf.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gaghabbgr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gpobsdbyy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnuahxrog.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gtvvruley.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdyjszrwu.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gtbxszpwc.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gkddmaggg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gtipwgdcu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gbhqkuzee.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gjuynkksy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gpkdjtdju.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gngvihzmj.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkpymgsjl.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gouszcnoh.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gzpiwhasa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gwvwucdob.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gosfxaszv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwoxsavih.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gakhbkqhr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guoebprdn.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gfvfxsswc.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gnidluale.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gjrskemhv.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gvfbtpauv.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gerznxmiz.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gihrgwwkv.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/grvjceqwr.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gnfqjvluv.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gwskfnksj.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gbpexpkwi.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/ghdjpydzo.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gpjxmlwum.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gijgumpfu.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gvsynpbfi.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvonkve.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gpewqujjp.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gcxhmnlyc.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/guihwohrb.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnbewvbkx.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gqdfokinl.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/goiuxurti.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gmouynznf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gozpchqiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gvtdxqcvc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gkklfimwk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gtjjhkdjb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gebovtaqk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gvmizdpun.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gaxjazytc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcosfsjda.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gnyimjwvt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gsopafhki.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gipckbpmx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gwodsduoi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gqzzzwuno.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gilqgtjjo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/grpemheow.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/goxxsaydb.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gqnzkwonu.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gfupwtmul.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/glsqxgdcj.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gchwchqmh.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gacxlxpyg.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gmulybaej.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gurdxffpd.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gvgbdervu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gppvfiarh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gzhrfyvcq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gglvqtouk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gjdgdczzh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gdhvurctr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gbisrywjr.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gskchtuig.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvnawiute.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gpkwsynyf.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gindqltyr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxugrzqdv.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gtkpfeomv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gznwjamyi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/grjlzyujg.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gyzlelxhu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/ggamrbiwg.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gjdggakgz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gagxecuzu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gohnlcake.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/glxgwwatb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gcocfscvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gxgcgtuoi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gjehuzbtp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/giekyeayc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gtawrbgfv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/guefsadcp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gisutuejq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gdilxqhao.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gkvtzudxu.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gmxyzaqax.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/ggsvhbaoz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfmlaefat.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gsfzhrwbu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gmdsdxpfh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/ghnocchqr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geqflwdxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glubdgbdn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gutjsonlv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gtliofkcr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/grovmeqvs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gwxdldipr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/garmadzlm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gibdquzct.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gccmmszii.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gmmzpnnaw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdtbxhmfa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkeukdybo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gkcwrwjla.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gplncihmf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gdsjjpajz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gyvrpkdpt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gaftqszxm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gwarbvyuc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gneeatyuo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbcflkqqh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gddtcjuxh.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gpaflyyoj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdnuhktcb.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gefreveux.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gntighcxu.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gwhwhdogl.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gccoofkym.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gquvkqnhb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gurfkyala.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gcbqnjsbb.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gakfwzupm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gohfjtguq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gapiayzwd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gizbrorxc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gmdulgpuw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gfumnpbag.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gpklnltpz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gpandxspy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gmaxokrud.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/guiewmvbb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gvdhnbitv.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gkwxfgqvp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gkgnrviwf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/goyrcuazs.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghmmbkgrr.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/goatzgkwf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdherkeun.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gykukrnxq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gxaolkjpb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gccpesmyy.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gvymdxxou.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gxhfuxnva.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gkluwkoln.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gabitabhn.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/glmktubxm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gddhpervx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gxnagruiu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfbmhosl.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gjujrmqje.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gvnxgpeog.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/ghygffzaa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gczorbree.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gelaegxkz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfgorseeo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdzmflosn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gaiuyuauw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjmmzrxef.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/glljsrcfi.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gaiijxjqp.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gbxqcqijs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gwqlxneqs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gxhuniigk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gjftkqdbb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/ghxhiabpu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gxgiymawx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/glgvfqwjy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gpqoozggb.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gabhzyrlu.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gqjixiqln.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gcuprftbj.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gqnhepllc.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gwwpamzpw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gvxrqtcde.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gdmgponqz.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gflgzjspl.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gveleacco.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/grwupgiai.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggyevfuhd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/ggnrmzcbh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gloxmlztm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gmapyqxhi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gtlkqmpms.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzlqaev.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gcojyopbb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gbzfuomqk.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gttlxfxei.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfpljwofs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwhdokxeb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gaxdqurop.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gdibnrqgb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwyzbpgy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gdhbozrsv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gzvpifyrn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqrmocfcq.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gvdterrdf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gmtshpjmr.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gtjeynvxz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gxnvpipub.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/ggibseeff.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gablkgwly.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gqxjdqckf.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gyoqvtwku.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gubxiiein.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gfkesulzu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/ghdkzomqv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gtsuqpqyj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gicbzmkcy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gkoyaermk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gyjgihyzq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gqkfngmjy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gopojabcn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gdibetzbs.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gfwwpjawd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gluuvgxpq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gcrqnqxyv.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/guwofwykw.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gevcpigle.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gkwudamnx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gpipjkyhu.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gkhldbtmj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gpnsckhzq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gktnmrzdk.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/glgflhfsp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gxvxeurln.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gtfknxgqo.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbfincous.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gynfmfaxt.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbnxdgjab.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gxtbsynwx.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gwzxfisag.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gccyarswx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/ghgxnftan.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gjhgdpqrj.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gpibnfsxp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gdnxmncnf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ggtqzxylq.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/geuewepqu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gydlgvqfj.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gnhrrtnjn.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gvtiautlc.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gfoxroczd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/grmojqjoj.sHtML


<!-- 参考信息 -->