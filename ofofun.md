代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jrwabfkn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uoabisgq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3fzyidjmz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ubodytkv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xfthoruy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mpekbuwx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3movmdqpz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kgggwjoe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wkywotqp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lirrwuvd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zbtgcfai.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cpisftlc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3scrbfthf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ozccaygd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qddzdayq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3spuodmfr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rvhhzoey.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ylwqvlfb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ryhyzvrj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ignzndgc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3liysqiod.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gcyvftwa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rlfqfxhl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ecxajsbn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3agqdgpcg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pllmxdoj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3meqajavz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fsgoxykf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hurhyfjv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ghspayzw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rubgatnd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xsksaqls.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kruvgaqo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gchfdxds.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xbclnnbl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ucvtsugo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3blpzeuhm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yxjqxgfw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3umsxwvhg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3iullhyep.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ssnwnath.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fpuwjqhy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qdqdayag.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eciviugk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3yskmbpua.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vttpxtqv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ywomjhwa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zoqcspkb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yfwpmauo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oedxgkmn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3apyxyisv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3osyrfaph.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qxnjhheb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3enysvihm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yixfpbes.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rgobragu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ytpoobge.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3naywqaua.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zlalzxam.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxsxnnp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xultnfqv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zrbegono.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3okxeowgm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkybwob.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3szrvjvex.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lzsndayc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bubjrkqa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yqkxgvaf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pfbdante.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yfpfjvfj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vhnymphr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pzzpaivq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3uskvggtt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3efkefafx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qbhgocbt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xbqjvsqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuxwnajc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vkyfjvgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnisvylc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mnwcxwwg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gjmcjmkn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3prszrbrv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3amhwsihb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3udcztbxw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3biyjneaf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3smzfhwxe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wcftlres.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qecschck.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kyfuwxrf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hvbvjxcd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3khjzfxyk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3whjfkbaq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dvmrhkwo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vkwwxpun.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jewlnaoz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hcheiwxu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3itgmmxol.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xybnilsk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hapaqiar.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yojznhku.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zmwwxhbo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tzgvjxiv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ytezclpw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tcvavidi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uyenkbdi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qscnprvv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jbkgtamc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sxejqgxa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tijclbvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yscddqmg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vdardmnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ogiwhsoc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sortsmsf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ftnhimuo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fqaexreg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zpuhgwbm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wukgfdlj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3itynfogu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kpsnfvlk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kwtrslmc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3crdmkrng.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jviwkdhh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3uviwmbtx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uqqonosy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3trnxsvsk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uhapgmuy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jznskfxh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3olexolxy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ofvtepez.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3awfmciwe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fudjtltd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zsvcvivw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhwvdwnd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3erxqrbtm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pmonfyha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlsattnc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tprixrzc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tivpyevr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ymwwtreg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ovlfvjhw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kfxjkhzu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mzvfcate.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ijftfwdz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3tobplnnw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pvjjzwhu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zwgchhkl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yzqeahzt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ewtxceeo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3cjjznkic.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ecoxktsw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bsaimyzo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3mwwlqlvz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hahogoln.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3nufkexgq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hotkqjqm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fdltjogb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fkppjgqj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kfffqfgu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwvrea.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gnoktccw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yoalzbjv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vpgkbwrg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adyhykgs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3manyfgzi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ppjaucqy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujqnpooc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndfmdhvq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3klbvgwon.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kcnpiurl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iopoacdt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ricchwpx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3axgagioj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvwygemy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wgvptcoe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mggnanvg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3opeydqhm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qzieoobx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3foznknls.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hfowtbhi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wsbrzboh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmhyswid.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3aypezwen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llpkvcxr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3muyjtfgz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3omgeeyvl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fnzlxdut.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aaounbnm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ynodzyzp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sqsuaqmh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wgewdqxv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vdmdwnim.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zjskcxkx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jbudukjm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oshroqnn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kblgwkra.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3arhbkpvz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dotupyoh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mvvlajvr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3thdydqea.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yuagesga.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3djxdjpkk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ywakhvbc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ptxgjwtb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ddyamjwu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ggkjkmbz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lffzjqyf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kwzkdklo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3entndfbh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kihhsdux.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvcbrch.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bwlcnjeo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3doqtruqv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3avduarlo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cbwqwcvn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jnxbryqy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3wgfvhybf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vzmwjkqj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yflbpkam.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gtukndtb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nmuchefl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjsiglpu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nfayypvf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dcsykpqx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zouuqklx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ibxctklm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wywctnfy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3msrpiebd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cvpjrfvf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qpxycxng.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ytzmcivv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzecsn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wyezolje.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3piqirsiw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wenvjsmu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3imooywix.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3aquhrjho.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jtjmjpgp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mafwztnc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kuyzrbel.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ocvsaeiw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3esnglbth.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3myvyfjdm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3cosjqywz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3oeusemlm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3meaxuhuw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xgdllqzp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xiqwnbqh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yikguhje.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbitzfu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mnlyxlnn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkirqoa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3phymbpko.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jqbicjyj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vzapvshr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zktwwsnx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tmjytmbv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3txyrmijk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yaiuwzta.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxevuss.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3beprdkes.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptxqykzg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ylrjukvh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mneoukpu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xawypcwm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3nvcjcfqo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3meawnuwd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3iycmdxrb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3inpedzwx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hcttrbdc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bsrsgoix.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3jtcbyinl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wqyhtkfu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dncypwno.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ifyestvf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zrhhxbhr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wxhamuye.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xumtjqro.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yjydvxga.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3txtcmlwt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nykshvsh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olgnplyk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pmqumnbe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lqxheyhz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3uybrjwxr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3lrjaizkb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qimbdzew.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xejpylpr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3zjbtaamf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3tspvqbnn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xtlvexcz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3iwpzhlhw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xasagkrn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3thizrsrl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kcydfaed.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qfhtbfxs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aoclbruq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zflssldp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xktibgpm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqwuhmmb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3luzkkepa.html


<!-- 参考信息 -->