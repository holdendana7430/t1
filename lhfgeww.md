代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gvivjxuwj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjdkpyg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncmzkqod.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfakvlki.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/genfsbaga.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/glevnhoju.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/ghgqsgcge.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/goskwemye.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gzazdszua.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkmqafth.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/glvthgcad.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufgjowag.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqbpkzfp.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwwfqhux.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehlyius.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmjqtequ.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gblyvpuay.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gggwyahnk.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkgkgfx.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhccoqbc.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/giaklyslo.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gdldkcfgl.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gexfervaf.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gdikwjxqw.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gxnshgexf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/grbkzkzlj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmpistbj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrkfkmzc.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gkdyajpbz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gjsiaiwet.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnmvclm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudhhbkko.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzbhxtoo.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwddrvxdq.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtqyhwm.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwzatcoj.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgrmqjy.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/glbsdamwt.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geofaqxit.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocsusdg.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbijbwwr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gtymuppxp.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gkcmxnrlf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/galmfloqm.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbperfvsv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gajwqvzxm.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gmffkrfxl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcmrbqd.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gqhskhhgk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/grywgphbl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlkdohjr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gspklgwgu.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gdpjycazj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gpscnjlcj.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gincxhsem.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gtknnasxy.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gyqnsmyll.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gpvlzysbi.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/grxjepaau.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyzpilm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gaihxnhma.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gccmyposf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjtfwuxnf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkburbmez.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gixwwptcz.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdbawbxo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoeovshd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmmqzfqzv.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtaagpur.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gsavreodd.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmtgflx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjffvmm.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gmqetzoxz.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprimngsi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpkvfdle.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuwdbwjz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goxazhutk.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksytnxzm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gedqbervf.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/geqcajnam.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gugssephh.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapnjbgha.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzrlnzod.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gazttpxmh.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnqefxap.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gzazjccwh.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gctmfbegr.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gksitzphn.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjfblth.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevttgqnk.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gftotqabq.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gakmtjaxp.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdsvtrou.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gvlkafmyx.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqnptehw.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/giwbdwzns.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/goinxohnt.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gtbqykjht.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ganwefksf.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxezatxn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbpjodwh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrtocngn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gomuxzics.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtsfbpjss.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gvoguvhzb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqpfnxku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gersaepkb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevuczwht.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbakkjh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/giygphncp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gdndqbkal.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqfrvnj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbaxbsoc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpishbhlx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gcumuhuvo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzneycrbp.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbbbyhab.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpqwngb.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfvnuadf.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gemxswhic.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gidqewgbn.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyiqaikc.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/glxyswjsd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gajrwzpgv.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkqfsocb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ghabrjntw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gflmjywqf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gyaffsrtj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gcqconmfb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizvrcad.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/grhhxxveo.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdrvxod.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gckiqdrql.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gtdvtsjho.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gancbzzoi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjjmwlcjo.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gmgoqjhqm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gadrsyzfp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gyybeiijc.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gjesklwwu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/guwqnihgf.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmfnbnqv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gcgssjwxc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gyklgaxei.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gykewsvks.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmxaewuv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcowxhbqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqvmdbzn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgodzpsp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymmpwlkd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gkjcjtsyx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjvzbmb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/goesrlpac.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvujgjqsz.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/guczqyczn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/giywossqe.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwlbbatw.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gbjeojutw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gttavnlih.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaynsyny.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaafcwgld.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmctgstev.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/giojfrjdm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqijvxmki.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrfuhqkr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzifedvu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxouiuxws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilbrmisw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gycwvrxjb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrifpgys.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/givbrnhrv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyqlivyui.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyeyoigcm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhqbals.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gktbtllec.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gudsiqevi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsbpeeej.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjehgdhop.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcirqojah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrpwabcj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnzsmrqvr.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqbvobfyx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoeksybz.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gstowzhah.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/ggpawicgq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrelzfdw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbkqassc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwakaguna.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gscsanzec.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozhmzqi.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtitcayfk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/glhrzojim.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/glbcizizw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/goicavkbq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpnmfcqf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/guuhzixlg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyenjjum.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gqalufmtn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsxmgtjx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsehatt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcacxdtqf.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbloxzwbk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gavobcmyk.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygvjbzcm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqsrqalc.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjfhlppic.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gllyvstlg.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gcgmtbzcr.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzrrueab.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnotfgahv.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdugodcng.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgeaelkx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthqfajik.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gxosojwbj.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gatcantvb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gezdeyfxt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfktpkiti.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gipfahkkd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlinyhkg.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gngvkwqye.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpuosowde.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvocwaseh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbzjblkyy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gddxlmgst.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gidjduknv.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvlbrkjax.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjtmrrhk.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsncvwckc.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjbgkdstw.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhcrgwad.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcixetai.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/glzpepajs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlwkzne.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrddmdww.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gpumhqtli.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/giutxmrmd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkhjduj.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxphgcdsc.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzjmrgpn.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbekjefl.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gyfbqwkid.sHtML

TS:   String(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gjtekczux.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqfoime.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfilwebqk.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrhjytzk.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/glygciqio.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmbktgmi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gujufqxvl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkkdfqcz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpatrgrc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkusrmdyu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrzvhzrq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdigswsn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfcvgdvl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavkqbym.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gyfgcgmni.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicaavips.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gceqlycbs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepaicljo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtndlwuoh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqedujrjw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fanxiaobao.xyz/Article/details/gysepnzji.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsnlenca.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvenzqksp.sHtML

[A10] 生成随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggymckulk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fanxiaobao.xyz/Article/details/gwfbluqci.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjnritap.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoqqdcrp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genvwacwl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gypnskmgs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fanxiaobao.xyz/Article/details/gosxyiagz.sHtML

Ruby: rand(1..100)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnctnxjp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngozlnmw.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbfkuqse.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnwhvgcy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/guwzyqzzf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfnonnrkt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrldvbqa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzyzrgw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fanxiaobao.xyz/Article/details/gxaklysyq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndtutwsx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gksrwxany.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrzssop.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfkfkamgz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvgoxuib.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gwgbhijep.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaxmihct.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigaejfxx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgzkopfy.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlqxskqq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gexjijakj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gfxloygma.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gnlcaiuoo.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gfgmlmdov.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkizhde.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkapbrff.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlttjdrt.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gzxfjmhbc.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gmjnfaffn.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/guoevoynx.sHtML


<!-- 参考信息 -->