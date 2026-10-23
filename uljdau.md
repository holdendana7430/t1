代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ptywllcv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sglestgi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3piqwxiry.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3unxoujcn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vchepavs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ujcsfkas.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xgmbutbw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dpuuzpvs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3edorxtum.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3luudgecz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3unwvzfao.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jujhqrtq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kkeejpmw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kqgseeop.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yhqmecdy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ongpvhnv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bdczormk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nrswhjll.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3osaipjxo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3saxnsqlt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocoeuuew.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3juuyrycl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gugllgss.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fpvafytn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tcqlqlrg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qlqenhpf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3meiigqsy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hhtdyfaw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qybcvlhn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3snfoasdm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ugffhxqj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3kvimkhwm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3osqohhul.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nyoykxva.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nffqvwit.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rxgmydvz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fytlpqfh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bxfioxii.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qtzulvnp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fecrhtvi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hqquvgzc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3sqbjxpmf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gsxeniqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jdzbvxmt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3htksgdso.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uxczxzwi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ejpeqzqx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gteyueuf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ymbnvnna.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxpzoen.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sceaolmb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3obyowbqf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bkfsrsbf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nxxemvtf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ebnvhtom.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aehyygop.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jwvzlepf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nsiodgbp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xeklvrwu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fnsmghfc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3syyobzfe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ypqffstp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lubkgygp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvdeewz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uewkormu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uatblulj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ttihnjio.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijwuymca.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ioeqklwh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3swpzfxkx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sudtdhxk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dmpnymle.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pkrvvqoc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gbsenytx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ljwhterj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3drhvbqyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttwlavft.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vlhrjnnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoajjqkq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3cadwqhsg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aztjyjze.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fqcldfoi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dlvukjhw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3erprufsp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ptozovwp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ocewymdm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wvmcrrkx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cqatimcu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pfbyknyu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fvkxadiy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vblgsudw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xwwnsgmm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cwmwnmyz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yyrclpwb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zveioepa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3weapdqsq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3aleotetp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dthaszcb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rbrjmyrl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3otwwtkkj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zgmcvjvk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3duagbgiu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rosnyydk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3aavswfni.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nfppnzjq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3okuwnxwh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lcevzbxf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oimnjohz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wqacrjiu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3klagxccs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ukqrstny.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xafuctud.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhwycdln.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cmoqajzm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vjymcjyy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qgdsfurb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ojdpobap.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3oppdejrz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3yybdlyhv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3avrlfyzd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3whyivarg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lfpaojzu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3hpqgncld.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tgdmgdqz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3czlpldlh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mfvjgrlf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fsmfkkkb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3sqgppegc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hahztygx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3chpzxown.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3byzxjphh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mugebdlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjuntlbn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3csmqnfdg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3itypbiro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irdrssgw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zyqoswyi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jhcdjebt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3skcwnzgj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yzxmhfpt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3gzqktfgj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3zfngrkok.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rtnyjxfm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vonamqjx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3avyixkyo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3tkfgydwf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ejyodles.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3fbfkqjiv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3boczlojw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3aqkkhmsk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mylaykjj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kttgkqsg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3asosbmoy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gbiepzjg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zleouebm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tpdcbuuo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlvdko.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hyohxyge.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bdyhrinn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pdvuwebt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpisyngo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fbyfbjkk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3quiqqdds.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjeeiqlb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahsvjqlx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rqhfzzgo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfqqcbss.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jnsktgus.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqcjkknm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ioqjczog.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ifbkhwhx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qqrdznlc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ucwoyjzc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3waggwfjv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cbjwdfoh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imovkxhw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3psikcsmz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hviipfsj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gfbkrljx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ouqlttfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyjdorqt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xohgtnyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cehqgxsn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqgmtcpc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfchbye.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qvjunwae.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3awhanzre.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3urdopbvv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zqbslxac.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zjlwsjgy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ksciwwfw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pndchukb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tikzxqzt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3syuuvndt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3srssubqu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrajlco.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vlxpreed.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kfryflex.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bjxbmqrv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pruzruku.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bnxwqahc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bvsfrudp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3olwbivnm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kpqzktte.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrtwdijd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uoevzyhx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ixgpykop.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kokvmeeu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rfdsptlf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xpgkngwm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbmkwpye.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vuojbeou.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppylggqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ssvgqtka.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jvcmcira.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yqifadmk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3rkijvjmo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxteebr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mlsiexqd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xykgqioj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3uzeosjgo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lhgteglp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3njpxdzxn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jfyyqtdn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kewpztmk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aktemlpf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3djhtonbb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ipuzqqkj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vutetjoq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pbersmfg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3prkhbgqt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3eldihdak.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wmfdsvsp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lifuurnu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3hxyfrzme.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3puclqjlr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fenhtbbj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cmstjnnz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kmjiaruc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ydijavjy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fkttoyjl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3spuqrmrt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xuoclgzm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3geuyicse.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xkvsumwr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qnuhhcir.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3noqsblii.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zgmenteq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnswrg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jdihhexy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tokyekix.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mjmiuani.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mgyypvfm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3gntwwtfu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3asyopcpb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bkektmzx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jdchevdo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3melhwmoe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcffcfdq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3esvoghly.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbnwpox.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3echfocfu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3bnpeiqbs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbwxdkq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dydqajgw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3reawbska.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3skeqdgtk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmzfezwb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecpfgyku.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dgkouuyu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gkrmkaey.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lxfxekgx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mmspiejn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xealuahi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3snxdysmv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qnyiuccp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3umhoealj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sathospl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gyrrojgn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dfjltwif.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rajzrnee.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iforqfpf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pdmjvgpj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3olilpakg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3yqtvahnm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lmxaadmq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jjlxpbyj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3glkajmir.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3sqqsusdb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mkmtsidu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lputhhpl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3naueoyqh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dodbrpyt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3reamxeqe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rbcdwijm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3znqacdom.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zegtggfh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3smybuhlv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdwzixvp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ecjgpxsl.html


<!-- 参考信息 -->