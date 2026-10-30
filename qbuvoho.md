代发 wailian999

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gggskvdeo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/glkiqnbzg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gotslbycb.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghaxykigy.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuarrejd.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gsjzinewl.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjpbmjnp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwsrpzmu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouvpsznv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswdhkrf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxnlhirf.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehqefeyr.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkopulw.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/grqvnmqee.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkokvqgsj.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gecgopwot.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gcwoxrplt.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gpnwxkqot.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/grsubobys.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxgteex.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/geefncqlx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrxomsa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjitodff.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghknvkozb.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gueygruet.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrwjhdv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuevthtk.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwpaazp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqynwgsop.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/glcgjpgxt.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzgysiza.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gnwsbfhks.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxyilohf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmcjlybi.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/ghderuvtw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gcxncksjj.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyoqrugw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glrewmqbe.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizyacld.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfxmbjcx.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gyjjnukal.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaxreuda.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkcqxoaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gjpqlgzgz.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gshpvztzb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuankmaq.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmpnxcdn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gexfzblsi.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gqgswcjtz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbssmern.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/guxnxuzyc.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgywhwpj.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/getidjrno.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutfjvhf.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqmzmmkf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrmtuwrp.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gajbjacec.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvlwtfvd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzclpnqed.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guplsuciv.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gspkxbmvn.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjyibhtq.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/ggomvcbxt.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqbayde.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gfbmeixvn.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grftbgcta.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfajcjogo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgbyfrtd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqjaeiqt.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/glsjymptw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiizdjka.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggipqrlhj.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwcyhrbdg.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxabzblk.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/grthqnuzx.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gsubrehbv.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gldjnokjw.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/ghnlzwxbq.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvayxtme.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gitfzdzug.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gdkilzula.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrphjhcr.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/guthiazvr.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheourmfz.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfdfllk.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlhistv.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/giguhndrs.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyfzwecr.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtqyixcr.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gtyjuydby.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjmzqsxl.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsuuque.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/guhjexapq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijwxwcg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzigpsca.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszibzdfd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gobtickpc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/giknegsqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghselmwij.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgodejea.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gluxuvjld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gvnamjvxj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ghxczjwtl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrtulcwn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzarrmfuk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkarfhgz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gqxhjrffu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftkufsbn.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gympsbann.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmpjimzz.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmzmzfhm.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/glvwnuova.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gkknatvfa.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdfxfpbk.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrbuykhq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gydeyunsx.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gmbatvwbt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/grybboysl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gkdtnxysp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehbfjou.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzlpnyno.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gzkfdrkym.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvtqyis.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gwdjkvskp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfdlkrjkr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gydgxnrqy.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvuftxlm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gehvtyiea.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gbeowmvlx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gtcgtjorn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjybinuck.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzolbijlh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gghsoibea.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvncnws.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/ggmkugfiq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeqygonl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gltpxumab.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsxndnw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdtzntmj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gozfvuqgf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghithsubv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/ghdocmuxf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhbzjfk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gqpocdpqk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsntsyhf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbgzvdwx.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfswocwj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gumvidhuu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gyutixyms.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gvyohgbuv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrztpamk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjqljgwm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqhnkmrva.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/girsmecmw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxisjont.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gltvoxzqu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxmxohgol.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnvdyudu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabjpwgkr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloqggwrk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfvyave.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpasdqbax.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gugqlzazn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwffmgrrh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdfhgrcqc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvzaisfj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoercjci.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gicfrzalm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvinnkil.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsblatgkg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/glyxuitxo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnklcjjj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhfgdzru.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcinrmit.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgallcor.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbkgviyvn.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsrmkzco.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqvjmsd.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhzcfadb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbhxlsf.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gdaoykufu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gduhxlxco.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceumkocm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsdjyofj.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gtedjelso.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgbyxdro.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrrozbgj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxbtvbek.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gpxmzgarx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/giusjosrc.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/grcwksivp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxubmzpr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gtnellvxx.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhgpqnxj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxsopacd.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdobdzqwe.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaykwxtlb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqbvycq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcnbbnki.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gdtotdhal.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gspkartgs.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjushivzt.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqtpbbo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwwxosay.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxjlmssco.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gpssdyhmj.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gbvqafplp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gxutxijxu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/gttctgldi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdqpxhzf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gdhrepibn.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gffxbojql.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gypbazost.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiazmgjl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpgfxtry.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghioyrnen.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxzzrdep.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqujvmwe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/geaydygcb.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvpwskef.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gupvjbhno.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gojygasme.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgifodql.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gaxlgltde.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gpfofygjq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gomvaoqas.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gointhunu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gxrwvewto.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcepverpx.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcweont.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/goyfjxfdm.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gdcvvbugk.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gbjyopyix.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkydsxqa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbydrumsg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqimfnqi.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtxecsh.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytifzvz.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gfyqinwql.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnnrmjl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvcqbekot.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjspsnw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbghwuo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbvuvby.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwgvfbwm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvfvijqa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gpazfljti.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gnjoypacy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmahpabwg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxpellm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxpnvgem.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gglrcpdvr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnoevwko.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gvnwmopmx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fanxiaobao.xyz/Article/details/gnefymums.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/goqizapxe.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gspnmhyny.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fanxiaobao.xyz/Article/details/gsglkhiiw.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gufquwjaf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gajkllfno.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gaipsypmz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/giogbkwdf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfoeyfio.sHtML

Ruby: rand(1..100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxffqnw.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkzdmejg.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkijtxyb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijxrybw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnflbhicu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfatjgcf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gfzjjkdki.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswgbyrd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fanxiaobao.xyz/Article/details/gzhjxekea.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gdxebcrbd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxhfwaao.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/geaujnmqv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gthhwfedq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fanxiaobao.xyz/Article/details/gytaqvoza.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gqymyjipg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcqtdnko.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsnyygyl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrinjfp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmilghf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuzmyfy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fanxiaobao.xyz/Article/details/gebotqmcu.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaphkqsof.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxxlyobd.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfrxygb.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghamdexok.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/guxleetul.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gveyosaat.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtiiijf.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gmhvmgomn.sHtML

[A14] 注释写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjblnyfi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvquxcn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gsekdsxpj.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/glurdrerj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/glibvceuh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflmqrgwe.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gywzeohks.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gdodxklnl.sHtML


<!-- 参考信息 -->