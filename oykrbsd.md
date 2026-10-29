代发 wailian999

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gcjnhdtta.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gizdfiihp.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gdadleflx.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gstxguukr.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/geefhnqvn.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gojlkbigd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gyzstfdhg.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/ggdkyeitp.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ggsyzvyqm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ghsbtpvzh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gqjagipee.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gybpoddnp.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ggsiekhwx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gfzdmoayw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gfwdlsnnd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/glbuzcavh.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gpzebmgjv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gwiyesvzb.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gtfgyrgrx.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/guxqbwhen.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gbbsuirtm.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gbnuxnaul.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gsptfufdt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/ghqxxwytz.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gyqpuacls.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gxpltzruj.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gpgazngya.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkqzolpms.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gmijxwkxr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/grdjalmcg.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/giynfazgp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/glqlftffl.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gecumxezl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gknghvrpv.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gmvyxgflb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gcdxqykvj.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/ggvdjtons.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gofinnycj.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gvimzbpyz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/geuuupgyq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzowgrvxt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gfwqtojcy.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/guhdxoeix.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gjzykcbrc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gedpculir.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwycwbjqy.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gipwgbidf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gapmigqge.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/grehbpzzl.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gensxakad.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ggvcnptfq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gyqbmgyku.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gdkohsvwl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/grcuckqzb.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/grcmchsvf.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gtsbtapct.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/ggmmjdeyy.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gyjsoqehc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gjnudytna.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gjfpbucjw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghbhrjldf.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gmnfzbmpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrygkbuq.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gothcefpe.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/ggoaecfds.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gxmpnnwrk.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/goctvctig.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gddixdbyi.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gpzjoidlp.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gjfziskqd.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gmvzutakx.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gxukatfxn.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/grnsnqpwk.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gxtmrkkwi.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gzfudnzdl.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gpqnmprbc.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gonxeleor.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gbtfrloup.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gwismpbos.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gzxgsctkm.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gdphkasow.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfqqvamsy.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gnbotswho.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gnmwfjsgg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/grquwfkys.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbcmcluwn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gabxflwgy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ghwnjrtuv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gxsklfruv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gdatlzbgo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gpjujgxzx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/givdkzlld.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gznoipuwt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gvyobczyg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gurfxymyr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gpqzlbqth.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gghhpcyds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ghmstrydp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gvhulcqei.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gytduufug.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gsirrwjrv.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gytsbkujy.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gpkshoxpb.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gnvzocmgt.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxlauuc.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnbpvavnu.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gzehtwdkg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwrbmygsf.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/glhllhpfl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghyzzrfoq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gvtmargkv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gqsizkwup.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/ghmlmdoum.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/ggwogwuuk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gzhtkkqws.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gftkujvlt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gluaqpews.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gfrowxjpm.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gfplrdsgt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqrnlywku.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gzfpywftj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gswikhlhv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gdvkvttsi.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gxfyaefhp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gxjaxrpby.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/ggcwihzvs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gkdpmixob.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gibstzrms.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gphjhyjta.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gfunzjxvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/goassltqx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gtnvmmadi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gbiriwnpt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gapzykrvd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gtwtwpxuh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gifbaswqg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gccyxrurk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gqjqxlsym.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/ghuqnhfdj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/giyonhvzs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghsqajcjd.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gcgstdrwr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvwegxwuz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gxabcknht.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gkjbwynuw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/grjyxnqvx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gnsbjlttf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gjrydnjig.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gqorysajd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gnlxswyas.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/guuflnrun.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gitppvrns.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gluiuplox.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/grztdduih.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gcqwfyhdf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gxdaqasqf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gglwpaurn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/geuvgojzf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gxldkeeyu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gdmyczflk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gwhckxwog.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gjmkxuvtm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gqyyczvbm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gogqmpeml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzsbuyksf.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gvqpgllhe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzohmbff.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gtmjvlezj.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gwhhdiodf.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/grnkucklh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gpzuauoyi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gtaiqaozf.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/guowfdeih.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gmusdptmy.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gndqukjtc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gmaqcvtwr.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gntswrtsf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gnbroirgt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gzpcqqjzn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gstlfojsz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gprvkcxlx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtqpvaimo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gcwxxybic.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gcqefhjmo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gmqubkqpd.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gtdhbxksv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gvsctqotg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gijdclfih.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkbljbgzs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/guanhtizz.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzjgodsss.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gaidxgwyo.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/grscimzyu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gvwurkjqp.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gvyfmcfvx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gppukmndh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gtkyyrfzq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gmrgzjzsb.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gqytqkdag.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gnrdqeozk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/ggemglpyc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gwovzqxji.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/ghoylwgsg.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gbiksxwbt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/ggydlmhuf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gfgohgsiu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/grgaaupwp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gczncvfyx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gqftketiv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjryxocxl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gdvirrtan.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdttghrrt.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gavymyzxd.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/ganmynevk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gttgixiib.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gwshbsrfh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gfatujseh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gtsuawzhz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gzzqjzhum.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gsddyboyj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gktfaovpr.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gtzrgoibs.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gryryiicj.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gnbxxbfil.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gslkliunp.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gxdhaymxb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gnuboezsg.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gxbidplkw.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gxjlwpuvb.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/guvzdisft.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gcmfzdomn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gxxhmbhvu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gopugeqdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gvomkroic.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gfhulwsxc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/golgnvqqz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gzxbqqxod.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/grmwtxqsi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gwrqcqrci.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gdocwhxnp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjebrhopu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzlauchav.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtmelclii.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmoiysitt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/glmrpibrk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gwtsgqxgh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gsakprefz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqiuxqllu.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gcovjlmzd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gpbwtlqeb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gdlngrbqs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gaaosmgab.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gutjgsehz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/guwwbbhus.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gncmhhsjp.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gwhbkzaxp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gzfckjkpx.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gehzbmden.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gyrvgjcka.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gwqfawujm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gagkevtzm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gdswnrlqo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/grcalxmuo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gmyrizytn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gzgijxyds.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gtwugniwy.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/ggarahefi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/grqqiuuvt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/ghggojmvn.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gmqcpbllb.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gtfqlrkte.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gkhjzbuio.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gcpkgzreg.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gyvjuoibr.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gaaciseyq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/ggszbxcso.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ggwfrftkn.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gsvuvbkjv.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gyuyxrylf.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gfkwgwjiz.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gudkzhzjf.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gukipveov.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gefcqomik.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtdegibwq.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gsjxepkji.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/glxscuaqn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gaxkrvcte.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gzyxlxapi.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gaylgofac.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gzzllshjd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gifnnfdqb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/grnvxcukj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gozjxmsov.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gefpwhunr.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gbgdgpusa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/grqbrouui.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gbipnkvkv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gyhfcvysw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/guzyxrjag.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/ghwnhgrgk.sHtML


<!-- 参考信息 -->