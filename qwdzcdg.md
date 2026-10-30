代发 wailian999

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gtlkwuals.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/grkgkulyq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gpdivyvxw.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gqnaxayhw.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gnbhneviu.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gdtmctdms.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gizzokeew.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gwdedcljj.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/goviaetdq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gesodhmxd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gkzdrmwkf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ginejqjmb.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gpdgsxzep.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ggnfinhfj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ggjrgurug.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gqcqtpbld.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gdylhcfij.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gawxgojrt.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gmwptkupg.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gdlflrluu.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gotqcampz.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/glewbpjei.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gwykozczt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/ggujtxdgy.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gidsuindn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gzbqcysfo.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gagzjpbbp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gafunlefn.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gqqlzofvx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gsmsfmrje.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gqvznthgw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gozmcuiku.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/ghddmloeb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ghrehykby.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/grrkmdlys.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gzofqucvf.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gurksbtye.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqnpvdoco.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gphlyagqd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/grdbxwkjn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gnlzfdwmt.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gmxhmvewk.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gamtulfji.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbdmrlmuo.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gbsxzejvo.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqegavvtn.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/goyyemihd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gglbboyhv.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnmdbgrfj.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtltzijyv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gagjbbshv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gitxccjul.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gbfwbbyvx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gcknpkbnx.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/goinnxenl.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/glvduakqk.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gitencpkw.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gnplnybsm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gewwmhthg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/ghdgnthlz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvxieqhmi.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gjezyezca.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvoojcips.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/ghjrlapwz.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gxvmdjjre.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gndjllfym.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gdrgwzvgd.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gsqnuvbug.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gcneoknxd.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gwiujbyyq.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gbqfbazbv.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gkveuuqsv.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/ghzuiapgi.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gdhibuple.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gfbzdosyr.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gaqykxefj.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gncomhqmc.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gdgjwplqw.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gfctzruyp.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gupastxzy.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gmlvqtbjs.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/goxgstmwa.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/ghutfrzro.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/ghvyclpyo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/glftwtobf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gssmkfqty.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuosqry.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgwsxjp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gyinjuvzu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ghjjbehyq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gnfpnrdgq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gzyedhzmt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gipeqvfai.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggrmgefwv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjwrlekek.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqnzjyvvd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcbsetofe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gufffqmgx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gmssamtli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghsyhixef.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gqfrdhqby.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gqjnbmpbn.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/ghueamejy.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gnheeoutn.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gnsvddrtz.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gqquiuykb.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gnjznnoib.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjmqvdoqy.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gelhcoyer.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqfcakbai.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/ghvqxdpxj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gdvuuzkxj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gykcrenml.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gtfngwijo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gpjoymidi.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/ghqymmxey.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwqhtyssm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gnxlmvysd.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gkjnshksh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gghehjdvy.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gzyzrnydf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gmmwmpppq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gotzuljvm.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gravpcsrj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gvakqkpiv.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gaubwotoo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gztozadpk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gumxpyxoj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/giuquvnvk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gcyyxotep.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gxsxtgzbu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gtytyzhem.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gdwbbttgi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gnmnbdwya.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gvnhmwlyl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gnfipqfss.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/glrcuimpi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/glqqgkvlk.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gnlgmzvis.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gldxecjbc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkbzenmcd.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gnzuyxazd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gxiawrmyf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gletoiwvo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gygasxkbe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdonotmlg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/guxybvzfn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/glmvbcjld.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gaqapbhte.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/glscawbrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gghczodhh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gaqfrogbp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtywwklcj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggqlhmpgi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gnlohlner.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ggejscscn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnryrcg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gvtfcfwow.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxdddqlar.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gpsttlmjf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gyckihmhq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gntkxdnjc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gheiwrrtj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmizcozmu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwiwtwtpe.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gsxjqobqo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdkcfksov.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gpgkwovgi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gndnmarlq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gdyxwxawr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ggookkvbo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gunnhzacr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gqrimrzer.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/ghsnabuzo.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gkdquokou.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gunvdrseq.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gjtthoxzj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gwidlazmy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/giaiwnbcb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gxfglxpsx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gmrrtnrlp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gqwnjithm.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gbqzgbpbc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gvhnxxses.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gxdtdmcma.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gvqccnezs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gcksplubi.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gdypvmnur.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnhfjjzvb.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gtcsmsogx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghcfzggbd.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gathpklxu.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gkfiuxgvu.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gjpwdmjqh.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gdefrttyy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gbxteiidw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gnkjkjsqs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gmjvsmszk.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gkzgysvjg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gdkksfqqh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gccwnjppg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gxrtxhrpe.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/goizobizu.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/ggdfatmbr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/godyikbdy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gvwqrwwir.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gvgbizfbd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbbzyxdux.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/giwkclogz.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gchabbjmf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsocwnepa.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxxxypmdk.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gjyrhygoy.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/geiqxrjjp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gehjbanoj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gxtnqyuaz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gffxwymfp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gcvkkvxdr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gfehaengv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gkthwafdl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gnxqvwguy.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gulxwmufl.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gysfofvjz.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gfaxedtgf.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gyqcqarzw.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/giiujnhlk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gpupeqxoj.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gzsmgcmvd.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/goiaeitkh.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/glmaadmmh.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/ghyyhymie.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/ggemgkueh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gbqngpfcy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gbjsgdixw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gujvdfbei.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gvzyssryi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gofmqgvix.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gykocwbbs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gneidtmub.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gdplsuyzr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxfnsubqr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkqrrdefp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gobtwjlue.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gejphofqa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtwmvtzdz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/ghrtkgkrj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gwcqlviik.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwvnvyfpi.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gckahdxws.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gzyirkjlh.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gdslsnpzb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gzfuiansk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gymcwnnjw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gpultvdab.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gdrlkzqzx.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gkkcekrwb.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gtlppsarp.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gpesusrou.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/grtfkfmsb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gfelsxxvn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gntedxnth.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gnlgvenaz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/griylgxea.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gkpfhwgls.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gaivnbbag.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gyqjottbz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gugpllnlb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/glarbogpb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/ggsumwlob.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/grhryljoo.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gghibuvdw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/ggomirqut.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/gaotzvsvf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gygtoyrzp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gtcivplra.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gjsrlfujz.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gefjgbosj.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gwppqpagj.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gldvmuonm.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/golgarpih.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gktqygcvz.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gapedjrrk.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ghsxxhhzq.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gochjgmub.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gvsylwsgl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gtuxmwyqr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gilkebwyb.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ggjrjgifq.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gogpufsdr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/ghbjwobyb.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ghythlntl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gnllpomdb.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gzppmenwp.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/guomrlvtp.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/ghooxwxgg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gmhfbjxer.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gqbzidrdv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/glvweggqh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/geichksio.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gdetszsyy.sHtML


<!-- 参考信息 -->