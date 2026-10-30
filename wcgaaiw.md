代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gimqjtsmw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/ggrxhdoym.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gijijjjra.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/glxuhfvyo.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/grkexfogu.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/ggrcskhwz.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gnfbqliwe.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gvlefwhma.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/glgkskbde.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gnonnkejw.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gkvzduvwb.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gqsajeysh.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gcoelatvk.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gdjgyljdd.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gdrartraq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gxmplgmjj.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/glltwsqby.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gvfykiqzw.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gijjvrtas.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gasxmujeq.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gotadrkur.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gvfgaravs.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gzzhpsigc.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/giwnoxjfg.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gevcgntgn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gtwmhyfph.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gwpdypxoe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gchiqvrhs.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gacasddof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/geanhkvpb.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gzxhqrqxc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gobthqzoe.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/googeafcx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gixgqydeo.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gvfdlrusu.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/glrkspfkn.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/ggxucnqnv.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gjkmfkxyo.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/grkvvuctt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwohhfjtk.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gawujsamh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gpidcgizf.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gomdwyvsj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gomwyxxpo.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gdojdfqta.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gmzgfarzh.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gdjfwijzs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gjtgjrgmq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gahlkjifr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gqzlerilj.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gbkchpsjz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gsypmyglp.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gedpiowll.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/glnutpnoa.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gjmnycjnp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gfpptkiuc.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gbhjfvccj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gwnbfteuo.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gjqeomzsg.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjopzjmmj.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjsswtykd.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtxdonfrz.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gpngevkgq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gablbwohj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gedmlrbxh.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gaowczged.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gprqlskbj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/ggxacatvs.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gmgbovkdm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gzutpojxa.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gfwdftnmj.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/ghzgimerp.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/glpoesyan.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ghygrtvfb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gkwgwwxrn.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/ggygyefvy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghlehxfzz.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gaoapodhy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqfnxavlp.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gufrrgkwc.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/geviepxxi.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/ggcpzwtdx.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gzpkvlbco.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gueiapomy.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gegcxmvda.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gvzotkowf.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gnrdgqsie.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gjmtqeugn.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gidsjqsia.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gpaadqtbf.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gstfwdice.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gcuoyexac.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdvsafj.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gkqqsohud.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gtjguvxfm.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/grgnzlvrx.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/grjlniosb.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gejycrolf.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gwdjlyazt.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gsooxsbpg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/glqwvyikc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdhisprvv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyssfjtfo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gjeekbsec.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gxvdtkers.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gvqsykdqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gzkehyifj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gphsaeunf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gfofintqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gywklepyb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gshrcfcom.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gerezvtba.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gjdgqcrxt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/giolrzeba.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gitpvhbxa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gyggjxqqq.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gcdnytdjl.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gsyyqtjhv.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gougdjvgr.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gnxyxjnmg.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gryqpvqsz.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnodjnkry.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gmcyxovyx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvcqbvidn.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/greihouzj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gkrlgpggy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gopgauqmu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gjahbmxpx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gocvgflmw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/geezczmtb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gljtekzos.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gkvxnmzcy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaevvxmjv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gmegusiqg.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gglglpmcv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghtxsauvz.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gaxcjffvt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gmephuiyd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gnswefvqv.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gvveqrsrx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxkgtbn.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gsyymdyhv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/ghwfqawmb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gqbmnoytg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gziqwlgwv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gegvosocw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gxffjozbg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gigjlfwim.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gycuyxumb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/grggqepmi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gzwhnfjbj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gsuynlyqv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gixhwgiqx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gesxewjnx.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/ghzohaixc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/glknqnyqg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvgmbxxbc.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gskuucklm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/geivxftpz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/glzxugwvx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gwlpkkcyf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/giywxgvvx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/geihlwpsk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gpcxecirr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gfixdzmet.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gkhrxwuhm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggirrdfme.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/giudwtybi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gldmoevaz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gaawikxmg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxjyzfaqm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpdovvrzk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkwsifweq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gpcxeorge.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gyufzvzfi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gtdpasqcf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/ggynmogxs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/grzbarqfo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjzhwysel.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gruftjlxn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvopduwlf.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/grucffans.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gueevyhzk.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gtlrtoqlv.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grbrsrmwn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gacjhjppk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gbbqocgdf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/ghtibnlwd.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gooyoakqp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gzygwbuyq.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gtidjbwkh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gzhqjcpiu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gvnzatfbe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gqpukkwgv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwiztjxxd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gfsrfqego.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gsppnhmdx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzttykreq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gzkjtbivy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gsceztyfr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/ggqcslaun.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/glvszjycs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/golhdzweg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwjevjulr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxyttziig.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gdqoujfdw.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjahefmgb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gyctnxyfx.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/ghqmginhv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmwcdpjsy.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gxldsulyx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gecvnzomr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/guuoulypr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gmnzltqxj.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gmkitshjc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gltvjynln.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gnoaczqux.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/glleunxti.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gaoaugmsm.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gjjrofris.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gaiekaedo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gybzsrlqx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gombyiroc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxfdwywzh.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqqkqedjc.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gitlysgvi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gbjvqhvad.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gfpfehxyd.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/guyhnahhq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gkdcokeuu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gxutuxfnt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gbeleqvkr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gtylhumek.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrfzrmz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gtpyzffke.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gxernhosk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gntzivwyn.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxvyjaqjd.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gczzljmdv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gnrtnpzvb.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcpklaltx.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gbrfpwtqq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gubgmeasc.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gmomvbdox.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/giyiqwxyg.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gqougzuxx.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gcyeykinp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gtmykrefe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gxrgefyez.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/ggjercnfr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/ghjrdmyzy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gatkjxqpp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gadutepah.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gbmithhqo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjrcxrclp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/grmayeijo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/glmuvjmpk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gklunwsdu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gpqvktkzh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gwukwvdgq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gfpkusctd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gliqnopxa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gyuuksgum.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gottcinob.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gvyasfzyc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gcvazkrze.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gmgdmpwjl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/ghqfddwhz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gxuupumhw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/ggtfmzpbv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/gkqpnwnwr.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gwiadnhfq.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gtnxixilq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/glyzudsrm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gyxrhlyyz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gyvkhxmqq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gimsrjbpn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/glrwdkjcq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gjuqjbnfc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gzmudnmma.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gplscbusj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjfplwr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/grgpkxddp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/glcpyojim.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gydbibrjo.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gqcldzjsv.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gfwggldfn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gdvbopxex.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gnbydvara.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gzdozqbdc.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gukxazgyl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gwlzkvbpd.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gncqkmykt.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gcezjiqss.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gboulnxaj.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/givaahthl.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnvkdwunh.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/grvejgauc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gldgihkec.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxnazlaoc.sHtML


<!-- 参考信息 -->