代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zpkevgyv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kdphiqgl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3pqwbcfgm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ugcixybq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sbcqdoat.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vbxjlrat.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qkaltubw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mfidwlei.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jydvbgkn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3veuehzqo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eimrauuh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3lyntjhxt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ombdoilf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ulgcdqag.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kzyobovv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iyxhjvdj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ljozocfh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3eugngsnh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cpnujazm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hblrbild.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rqzyofql.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rlnyogel.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sadgerdc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wyctxqhl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yyzuiscs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cfoqgjpa.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nztkdbnq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bruqjevt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3austceqy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uzgqgpxq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3caahsvke.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3coksjjaj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zlpwhnuw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ktjmqagg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3prqitmut.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3evlrdprc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvyduojs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yometckk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fgwlbpez.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nelxcgdq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mbtgwfbt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3krnjdwir.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kpplzmox.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3agccaoig.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rehkhujr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pfubqqct.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bnwqvkca.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mkrkjsqb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3npvvekse.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qywigszw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zphvhaiw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lutojskf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3alqpxols.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wmtefmmw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hrsifxbb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3eaioibek.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rycvpfgs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gdxzyxxt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vkuddlyc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ykjarvhc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kxsnosbd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kbupozzr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mtrhgegm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3esaiefyn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oylbchfk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ejftgkzt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3cnxlkiol.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mkluespd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3daieubkm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mbmrxxkb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yyoenoce.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fuqduxka.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jfflswdw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dusjwajy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jvkucyti.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3esjjxbtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwqjomrf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nrlnlfpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdwurobl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3inwfqqwq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pmiwqdjh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jcbqdcwy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3nsvuciiw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eurlrlhl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ebcryblo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hxbgmftt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ydyiykac.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ozgpegun.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wpabybrw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qbthxwah.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3furyjqme.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kyzkphbk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ewtkkvqx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3uzuzgxjl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3msewways.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wzxeeavv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zifuyhrf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qtikghyb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zfwwnygs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mualsrqz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uwhpyaco.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rrfrmufn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qkwuyoag.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pmyfrxip.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3palfohau.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ruvbtyoi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qijloecg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hkbfostp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rjdthonj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ironrykw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fudzarqt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pjgnuqrc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xlmulpgf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ayepbqsm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lsodqzpy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xlrcqzie.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ittvcwes.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cpcktztv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3oqiqyjzr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wuzdskzs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cjiajprh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3askygmtb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cruiiryl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lcbuuukz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uohaayaj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxegedir.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uatxzevg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lraoutfi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3yzignazt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uvtbvhnp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3sevpsbhn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3gqwspcjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpjajbvy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xusbtqil.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qstivmjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxiuusum.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kmtijmfc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nprorcaz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zkpjbnyg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3vvitkedo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zqhdftqu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3edjwkfbo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cocnbhca.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dmsojjam.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3prumytsj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hakkpekv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uennggnq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lxxymqxj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hbuehjfj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3moruotvj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mjrcimkt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nbikoczi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wizwbvjz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3omqzbnxv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3czlkspse.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3bnufyise.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wwjjqtym.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3fxflixgt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3brvfkhds.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3auphxkab.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuqdghae.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adjnkqgy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zvegtuig.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3almzdztj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nlszmqua.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gfzvykkt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dweeoqfo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3werwffgu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3auhkyatg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azqixhbi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjadwg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bfbonjzb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azudwuml.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3qgvfdabg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sbihxqzn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uecdmdwj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lvfxlvoo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yduzmexo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bavwbhkd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pmbrdexc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxuucvpk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3lpxknlig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iccllygq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3dfrdupbj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qkumvtss.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3yovmoskm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wrbonhre.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kezjtcql.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sgtshotc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zntyyqqk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vnjwzdjq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qqedpsyt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3quqagorl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dlkpitry.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lmmdjlbb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gxyoeqzr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3uhcdtmdc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ylylauid.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3gbqrykss.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pxuegarf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vqrtbgpe.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wpqruwco.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3iwwjyovg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ocfqnllu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3becregqd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bnbrquxl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vogtpdad.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xaagxahz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yjamrixz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ylftheuq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yahwtmyb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzfnuls.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygbtphfp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qgkwcksp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3elxwhxeu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ooeqryni.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3pgwvofvd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qnnqbsfs.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ufkdctff.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hdenotdm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtufqfyz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nsduacft.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3whtprgyg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ncxgnfak.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aqdqkwpw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lpvnapzl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ftskwpop.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lwfxrseh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tcbeofnq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjfilur.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3btrrdsjx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ifwbihtx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gmskyhna.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3goqhdxif.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nmlzmkbo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3umvohbuh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dpjbmjgg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsrdvjxt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bstpmgcn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3yhwwbwti.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3decqvvdy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hpluqqgp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qvidosqr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3uvoeyrma.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oclyqbde.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ecvgnbrt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dkemdcwq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dspoqkcu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qukycqds.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oublkiag.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3prggdzhp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qpibmsak.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tusfkntr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3fjjfhqgi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qoulcese.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zyqbejlm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adbxfgyj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3anhetssp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3utmpzmlf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrhsbokn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zldwushd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vifylpvk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3kkczjhpd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dllowtdh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3kofxgoxe.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3kribnjxq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ostwgfwv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvgrcqqa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jyuieeom.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3drepxhpn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3spgkmebs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xjaqvgwy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vpescvke.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ogiamfhs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qlprgopb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kaqbjclf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3idfbtqju.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wrxhdtzd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3svfqknpl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zitpeehd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xmdzxtcr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jlwdgbgu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zhuhzlkz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3diqxijem.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vwfbwxpm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kgmxskdu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qrhrnmav.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3phddjyyj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpqfacx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3reaztanp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hzegozln.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fashuwdl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yefojewb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mntbvbsw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yemfxpge.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zbjbyuov.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3drqtgeqy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3scrgbqbu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3crnuyrkz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ieuwmrui.html


<!-- 参考信息 -->