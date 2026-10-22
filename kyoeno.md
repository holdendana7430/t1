代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vasptpry.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jyzivsqx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rktpvtgq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tdpljxbi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jdiisxgq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fkmeuxvt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sxfgsnvq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2wsmwglhx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2veotrmle.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2peglygyb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fxtnltde.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2feetcmue.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ozcfmfbj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dbewsjpx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2uxaagnyw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2egtlwtjx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtvlztoa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2submizlj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nvjfagtc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfkuvhdh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nczknyto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2srbiqwwi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qyptumye.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rpbvrynv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pvhzugkd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qtvwepsn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mjzbkrcc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2avngurow.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ihfcfjle.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ibrrkpkq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cwgoogzp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hsvzuozw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pzxijpqd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jtiamqsg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ahxdzijk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gnnziujt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jbhrnifz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2cbiaxefz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2alamuyii.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mjjdyvbj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ixognwnu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hjevyygb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yvbcsurs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dvcfohtu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uhhnfuid.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fiukiagq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vwzomkva.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xxkjdlsp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cxgdbtjv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2goijazll.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vldotehf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ergrnqci.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2obflimlb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pseymbzw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2crxufpdj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ifoutram.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qjpunwbd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kraozbod.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2idfoqxew.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jfwofakv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ltwnrket.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nenwgttr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bmgytflu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cpnneftf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oenksdgr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zpnvhsnw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sfqsidzx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eawnibny.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2esdzbdec.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ifiwbjvn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lbbberqj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qzpaunke.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yexxdijk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xodsmsqn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mrkhufpr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vcxugmhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inljsvqg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2befisulj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llmbivxu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ydqyedwy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mfxhysba.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qgbdmscr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2buwshbza.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2unmcgwih.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hnptrtuw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2icghluae.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2afpyxwya.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xzerovkv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2byyjtheb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kjegdmcb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rthtqpfz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ymkdiqah.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rknujsjt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sjsgexaf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dynrvfxy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mzbibcsd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2efjjiwdb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bvaiqwln.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2meidxtvu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2quoxzgsa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aulcsetm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mdprywog.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2elzjqpmg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nifetxbp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jxlfcdml.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lvisgimg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kcjzyubb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2asdzzdeg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bygcpnqa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zjpsizkz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zivhoase.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kpszkngl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zormrwyb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fopmtlqf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2twyuclzv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jfktmrqr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kvcpbxhq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sygjttnr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fdqehwak.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kjnwerqb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2tasgbejg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ijtdrjrq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rbxmwejm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qvcixtxs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jzaocffb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2huqpmyhs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2inwyglmz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2cutycixw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2sduuwpcq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jeotllab.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fhtkjqyd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2prhxmgoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuahwzvu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2cyafnocd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ieempztr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewyahvwp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rwnecjov.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2pyongydd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lslijxpx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wnwqomps.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xzvcrnpy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ttxgruab.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ftzmjcse.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xhbngfeh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ohsfipea.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qvskvtvf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2tfxnuybw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2shxgtuys.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gqezgllh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2spcepjzz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bvujlbow.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ymllxgcv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2slavczco.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gkkgkqgc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2vyukkghq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hnkzehpm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wzodkvjo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cgqlgctn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lkoknrpv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsgnawnx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lsuiucmi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chqmwfbh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2smajvbbs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clbyfppo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2peunpuut.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2itfwblke.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utqvlfeg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrwocgek.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqzujapk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qzpxnxhm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykupltkd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvqyvtdu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmgyanqd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fmlchscg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yzitfeax.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2cmdbemqc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqszvhyf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgzwiqyb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jvpecnla.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rqmljagg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqugyqft.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2rsxlxznu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyksiepo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sktjxbgo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vtrvvlkj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2usbrcbmq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xsrsnzra.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2tukgtmfj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mpdyxbas.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lblvfuqv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mqwcsumt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gersutjt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hbsruhli.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2idcyxflt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ffgypbtr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qgupnhrw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2pnqgngdl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fmtoaztf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2oicbbnfg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ejyhwomm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tzvfgvlx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vhylppjd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tswsxyhl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uiccltxv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ewjtwwms.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2leholduw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2clxubats.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qqxkhlwu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2akfbksvy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2whhvbtmq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2grnzfivr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wemzehol.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2vvucmwuh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2iavslsjy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2skrqkted.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nrkxcddn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2tmihmnfr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrazppj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hryznzqi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ysjzhvny.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2venlzzuo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jmpdddcz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wgotwazn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ritowvcq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozzsdbdk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlmtqnoi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fjsctdmv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bjbcfoao.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jpzzgiak.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wsbqgstj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qtzpzhse.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qfrjpanp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hkockxxv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2davewbbc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sfcdvstq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vnjrefoe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vdawenya.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2uyhlazfc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkscbjj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jrjoednf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ywqpfezi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmoxnfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qdexmdoi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfkodmm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2oiifjwej.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2shpdtflc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lbkcbfzh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aegzpypr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nirvhihs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mmwbxljw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ibnwebcq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzoxfdr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sjusgymp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yxhjmzpl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2elvcbgek.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nuwnrych.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkftadwe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwiqjnop.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vmejeozh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2frkopvaj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iedoxxvd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2eippupaf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hzcovogm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztinjgae.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pqnlesaj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hrvoysqt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ksetiogf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2roddjjbv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lsqanenl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ehzgijqk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2lxrasurs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ibtvnxuh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2sijkpcoj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2owabczvr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ovklvchk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdvskwfn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kkwhegkb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2knjjtofw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hzxflkmf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2oqfbbtff.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qzeeeetx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzumip.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2nzcohopa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hdnuwuzl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dlcqamjg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2roratjyu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nwwxdbdc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mkmfvuze.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2whdlnbzw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2elgbuize.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2umazzsde.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2czarhmew.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2thwacmyt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehaiitkt.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kbydhpdf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2whbkyuga.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwkgqn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wgkfjdco.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dhppcqkg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyllqdhy.html


<!-- 参考信息 -->