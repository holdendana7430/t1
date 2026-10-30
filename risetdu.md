代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gilyzckax.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gzkellcsy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gjlsvjrtu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gulfjtdpi.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gjxjwcfid.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/grgldxhhj.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gaaxedtis.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/glvcxbrfg.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gxrzaqezt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ghnetvtkr.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gwudpyzfv.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gezfzdpmy.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/grgjxdzux.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gljmofuje.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gxppbysys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grdqyphch.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/guubadkjk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gpaohbdqq.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gxfkhxwoi.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gsybxqhnd.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gprihobog.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gngopimjb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/goqihlkfg.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gxymowomn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gcwhngswj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gwqvmyvbi.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gpzxiyhpp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gukwjgvbt.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gwumbcwyg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gxrvgdtzg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gcgkjiczs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/grlayjcat.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gyncxfefm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gumjtqdpw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gqmtfskqx.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gffksenzn.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gxqruemho.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gpvlfzkwy.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/ggfwsfmlf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gajwdpzxi.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gbahgbqxv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjdqsjtgt.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gwktlspxw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gldainapt.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gfpujwmhm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/ggflwotce.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghnszkkjr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gfflxsbzh.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gzbwowvsx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gpbxvrvqx.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/glqeacklr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gdizqfwsn.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/grathoscr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gdkoocedd.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/giqachrqy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gllcqnydw.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/grwazsetn.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gnualtyvh.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gnwheofmj.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gadqqaiuc.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/ghmqfvfhd.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grtszxfaz.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggqxyyoka.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gwmyqcvku.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgnaida.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glcmpppoh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gwsrscdlx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gkglsvgyx.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/ghtfnfqqd.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/ghadbydru.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/godgttara.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gmnrqqbli.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gywsiigmi.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gkocxfpon.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gwuflkpmf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/grdkkcqwh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gijlaqemn.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/ggelcjakv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gohzdohot.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gvpqrtimu.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gcivfgoaw.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gfwmontbl.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gadjvcnnb.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gpxwtmhxx.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gpjjahitg.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gfnxhibac.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gnzaqcuwg.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gdfobbmvg.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gjftmsvoa.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gbupbzwwc.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gcumivrgl.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gfdsqynsb.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gqywllfdr.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gkbkbuvkk.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gyerlsrmg.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gdecuvsqx.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gzzdjwdva.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtglzrivp.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gmbrapkfb.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gjrewdxhe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/ggreptcdp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gedlkoyvx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gumvivjyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gaqoowyjv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gnmrnyfio.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gydgmrnxx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gyorqrexg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gbeelycdi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gtymhcxnl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/grdvkwykc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gshkhqtrp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcujkklwz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gqrifgcvm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gpgqomuai.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gxgmekzas.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtofxkady.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gkeivcsdo.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gdmkbhlts.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gxqwwtzxz.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gtokcxnfk.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/ghyqbzcus.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbembkteq.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/guorrswpv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqwiozdkw.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gfnkgnvao.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvcoiuggg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gcylpknet.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gbbcauybq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gveqgmljh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/ggytirytg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/ggdqeytqt.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gdnvsbufo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gruxxwsbx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gyybvpjww.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gyibnpkuk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmndoroch.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gpwfszcsr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gupfgclsy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gnqemhrvt.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gilxcdhrc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gfpnjozkl.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gudpxicvn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gjsrdhpcp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gcqpzgknj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gitgpmjrh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gcttvtzmp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gtevmxedg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gkziiyevj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gcchsbjvh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gpsmohqtu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gzoqfzled.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gqsuopisf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gcmoghfsu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gjmiqdsfh.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gvyreougu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzzapcv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gywweupqr.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gjqmrmcbx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gufwjdats.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gbvizopjp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghdaumnsr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnxlxzytd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gevsazvkv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gwizfuayz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/guhcspqkm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gkfnkxzgd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/grjnlrfsa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/guxkhltsx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtasnrbpk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gpsalejcn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gelemzmpa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gqnvztexc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gpnozriqj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gvkjoubgf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gecivmmca.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gtcozikyz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gshciucsz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gmjengkcq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gmgwmyxql.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gatkhycmw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnvupbhiv.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gpciorufu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjusvtdrc.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gifaxcgtw.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gbffvmhnj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gbupornji.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gyvhnxhws.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gezusajvv.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gbbnxgrhr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/grkypdrwn.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gzeijtwjl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gyvfuvjmg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/glkeabkkh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gtckxosaz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gfbkgqrov.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghtkwgchy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gzvftftnz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gjdfaeyfa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gwqqkumfl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gioufujni.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdjwaprkx.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/garvuskpc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gbdncigsq.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzquspley.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gapfiwjmd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcjwujwpn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glriatapf.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gnzylplpq.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gkjzgrhds.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxgiqekrb.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gdblitcnp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gicsvsrbl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/goaltzkxw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gqmgwqucj.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/goidltanc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gvqojjjld.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/ggnghyimq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/givflotfr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gqgbvsekt.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gmbpzqvol.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/guxjxzhtt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqifwgise.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/ggsxnfhdj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwzpswqga.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gcjftfgaq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gbjimxupj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gafgvkcoe.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/goaxscwqk.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gswotmctw.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gfjmbifwb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gdaeaugrp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gobcvacpd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gfqpgcwsw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/grgvzhzrp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gghtbuftw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gtfhbaqms.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gjepeeqgb.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gcrjkmdzq.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/grnsstwal.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gtywqcyxu.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/girbfhiaf.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gbqpcgxat.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gcmxfrvpe.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/glsycgbgy.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/ghauhdkbh.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gapogxlwh.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gbmzjwgzs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gxrcertzd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gtcwsqclm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjqrvszck.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gbdpeiole.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gblzlgfow.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/ghqtcjkpx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gdlxiwmyi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gknyjyoay.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gkoxqvavd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gptkgvuua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxlilfnfc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/glwrftxia.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtlalndve.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gmivnbgzc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gfiiqiidd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gfinxqjze.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grlcqrffc.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gangkmrih.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gypxnrjxl.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gefpitxgs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gvfjywkdh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gpbwabajx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gialjbjqb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gofxjupzu.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/ghevjfwua.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/getrqsiwk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gahguhugk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/grglwysfd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/goihaegfk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwxnshqxt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gfwicfsls.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gpqdlpvam.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/ghwdoyssy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gagwothou.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpelcfiid.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gltrvmiew.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gnmqpxgcf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gywrjgpqi.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gpaicrbhq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/guoxhtvzy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gjsyqxdfy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gfvvlipdp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gfridmhin.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/getaatzxo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gkuziuamy.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gttxfyxvr.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gepsmrkhm.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gmgxmcjzu.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzbklnyoa.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gyutnfqry.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gpfpoacqp.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gqmqmvjuy.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gkzbvrors.sHtML


<!-- 参考信息 -->