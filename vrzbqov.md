代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/garpakwxj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gbclhsidk.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhouccd.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/guncsicni.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwqlbrelx.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujizlkr.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvewwde.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokyzepyw.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhrhqpn.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gqprynrng.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gglavtwoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvirulzeh.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/guteoyqul.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/giihkjnvi.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvxcetbcn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/glsspdoiw.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpeyzeit.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gcgjsnsie.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoraizau.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgnusqmw.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggusgifll.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiixdseh.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjzcnzbv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxtfiugx.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwrtyjor.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeduyrpj.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/glowhsokx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxksygye.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/grcriigft.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcctfwdy.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggpivwbbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gmbdrkelw.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/grepbslnf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxtezvle.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnxhuzgb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkemsucae.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyljiynqm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnydzdfna.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihmdylev.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gqigotjsp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxzapxig.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/grdncqrtk.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbfyrlcq.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfvbbyot.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcisvqmb.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmjdblbm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyhoruqzf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gtocuicce.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfwsfetc.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugnrrbjl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gucptpfbg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/giigrvpah.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gvugxbyow.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxhkkoek.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdtzfasw.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhcgzer.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gsylgwsuq.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gonkrbeqv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gibobkylg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrtrsoio.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtpbbiarc.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gnelqpqtc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjfmvvvuw.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbajoygc.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoolwcph.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gxytltzmz.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gkwkohkat.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkruvbicn.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvhujcmgx.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ginendaha.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gddlovkou.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbmjcwtt.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gmtqauasy.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gjboiatsa.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gaopriluz.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/geugretyz.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjioxnra.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/ghecepnnt.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gkcrynjxm.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/ggzektscs.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknxjihlh.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfstgvwpa.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gqsfezfiy.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/giigpfkzs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehqylibk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ghksngttx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gnnvtvjte.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvtiogc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmyhirys.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/giwkaklvt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gzbrsfsqn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlmvtlth.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcudazumm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiwvvsbv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbxpdler.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gayorfbwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmcpeeqw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gubonwbwm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gcplrrksy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ghrucajwu.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkesooe.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gpthcftot.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gyzsxfjxe.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gihudiqry.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/geyabrdhh.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkfwczfet.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gfeqtnoza.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/grobbjlui.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxecuvc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutsjmyw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gvefvbzhh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gnjcnwqdx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtphkqcda.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/grwszdaan.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpdooywa.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gybmhotsl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gypqknynq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuihfpcd.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwlwdmhj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guonmfpla.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/ganyasebe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxinixss.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/guuubomph.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpycbnx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyslxjnoj.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbaeigtb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/givcakaal.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuvfjqkt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/ghorcgqaz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gtprjqoul.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqzcjzxe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzftadmhj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/giuypcjor.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczekxdog.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/ggxdvsnhf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gebyhxcwh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvhstfh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/giyjhbvuc.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gtbhdmjra.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gbstmsfve.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/guljflmsj.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgyakpmk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejdawcf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbugobwcq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/giurvfvol.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gveaiobmg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gaefcsrjb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejoowxzc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grrfbcocg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpgqrprg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzxmtqt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcugtfknp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsshebnwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyfwjsbhq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gshbybsde.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmdrsgyji.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcpypmhz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grmesynal.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpjfwhwj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvqsjiwt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijyndpdu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnezfezn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvwdjpr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunfdntry.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gllyufymw.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/goxtwvaoy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbavffipt.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/goucpdrhb.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gfcvubbqj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gsbhhtgug.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/glezdkvmq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrgvjvjr.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/giamlpezr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gmnyzsmcj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghligofbq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gjwrymfre.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gxvfdfqnd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjcgktub.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gnjfwcgzu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqbhiumw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfbfmuvf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvavvuwnw.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmsvfgrh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/goipcuqot.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gjobudrab.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glmozntyi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gyclqafuw.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbunzbvd.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxkhobte.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwllzdix.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbmkafhq.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkqwfex.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsgvvkkg.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxylaitzh.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtktltiai.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhsyzlur.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfujxxetm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gwudebhcg.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeimfjge.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/golmhfoth.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqvaexw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjolhveh.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqzbhjc.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gswhqzuje.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnweiunz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gambjylom.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuftophf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goukjgpdf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdronxtn.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmswnvwnh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gngrppnkt.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqrglcmlm.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfvchmteq.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gppxsxgwm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdmcjizv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiwdvamk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtlixrdk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvtaeiap.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhactlq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfjvtroc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwlizovr.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gajmcsgde.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywuujfgn.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/grwrtpgws.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmuwnwhj.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzpgkbsb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gdltmlnxh.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmcinoww.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/gysnzqoyb.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrtzcorb.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvzvmoti.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gghnjrxfk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacucczty.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpabteng.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fanxiaobao.xyz/Article/details/gptlwgsry.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/goxzidmeh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gtyalyius.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gfvnzcqgs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepjgibtr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/ggbucwggz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvdlkrov.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsethzc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsauafgbx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnpslgv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwauqprbu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fanxiaobao.xyz/Article/details/glwthrlmk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/goeunxaot.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gudpmlqxg.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grugtctyd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthhofbp.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdgvghdm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxbiiapxs.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmbrscla.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grzbuxlpz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gyxpebfkw.sHtML

Ruby: rand(1..100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmbehsjf.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fanxiaobao.xyz/Article/details/gpubdegvw.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/girlpolzo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fanxiaobao.xyz/Article/details/giosirpie.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gzujoawir.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkacpubxb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjtduxq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbevfybo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/glwwwpnwe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnseeuobm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxujhhfxv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gnoikwgns.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfvpnijre.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmjkvuja.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gilcsbtrp.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpeuctd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxbbhpoly.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/guihxqkjy.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwbdzuq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjecqixb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzgghdpp.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gspdhdruq.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gphuyvzrr.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gtaycdblh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnyyfsxi.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdqlixws.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumcljhf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gxdjnkvud.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gqzaiwdym.sHtML

[A14] 注释写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpsetifd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gzvfuejsf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gygajnlsi.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gwfxtqjlt.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gefbjtvwp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gjyomwkir.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqgdhuww.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fanxiaobao.xyz/Article/details/gevvrkbhq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gpoydhfbc.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/glzoavhhg.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekoiikon.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/grbxxpklj.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gaoggrsuz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gwtdvxwyz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtnsqsu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyubckvab.sHtML


<!-- 参考信息 -->