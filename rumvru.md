代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2iplayilc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qohizojp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2seriobcb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bcuulixp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vcusluou.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fqtlqlcs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qlgilwyn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2julgfsfx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qldspsjd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2sruuxpzd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hjebzxvd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hdrcgusn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2pikyztpl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bgznnshx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ieijdonw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmtwrx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rqkeeftg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mvoayckp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ydqcvbab.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbbgidpi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2whtercrj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bjyawaei.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mrwqtdca.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xyeqshrz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fsrsbgrf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hrrtkvfa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2spfopawm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoitxnlv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ksemoskc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ilbimltt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hltnqjxf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2izkvsqfl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ecllzrjh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2takefdbc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aefkogbc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2emdapawu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xtyyuiri.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vobjyzse.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zlqbtylc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gobfpiyo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2yyimfpeo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2auleoknh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xpvpefgo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jirdsrkv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2acptqamt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lpmranig.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2puqpblzt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qxlienau.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vegwdxzv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bvpoucnd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2pqceeenb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zcozztqz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvlezwdh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2psuegjaa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ikovnnzq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2okkjdurx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yvvcrslt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2flbwpdgb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2jpfufvlg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfgzqwaw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2raclsoje.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ygharqhb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jjeoblwr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2opigvcmr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yjzrqohj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eygnsfmu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zxwukdas.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ynjrdwmz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zssbamlq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2eskzqfvr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lckljsjc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qfkxhqoo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lxdyzmur.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cdlrtcjp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fhcksiwg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nmjqdrxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkbllwqb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2syunnhsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsilhvmc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qmtgifpv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zmwewemf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vsdltqit.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2eqjkkxgz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ubkiimir.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yjiuqezu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2stjqvjse.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fjfnrvta.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pzsxbuym.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ghxibuqm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2atmzfsud.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qzwfhzsm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ghgonsaw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qcwedhir.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vzhhcorz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gmvxisdo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jhjjnbpb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mefhqugs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bstfgxvw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xywyvdff.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xbaxjiji.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2txbvbuwe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2plbrfmry.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vhqmyphy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ppvuziwx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wrmxjisx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pqcyilsw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2slkughxt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jinsnqnk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nejobfly.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2icfskyho.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mrngyldv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pxtdbwqp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eyddaprl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ikdsqslj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yqxsdwlm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2siheywed.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xhaohdsf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hsvzndwj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vtrgcyni.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ivkcxthm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2snxjmsdl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pcligysm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lwwjpyjv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nromxjbk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ntjmvtkn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yexzxvtf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nrvehppv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2guhdylyf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2yqmrntwb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2soqfafvk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fxaiuagt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sqxexbas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruteoodx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ymtkkitl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rkfyexxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysqttlmq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2tkyxcgue.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2otizqzms.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2eitaviqm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pnlhhxjd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2sqhymspw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fcafwfqc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jfrleenb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wcannvje.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jtjgzldk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2fwphhszc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bwketqmm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qvzxueid.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vzaknowk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2maxkygnj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rpoffzre.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mfoxtlnq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mxupdecf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2awgfhpxv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2eaktlxhc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2igayedrs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2naisaqyx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2agveowvp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qemuhfcq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fpuwojdn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2caoinpqo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uhvpjreq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vfksbjvn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixauktuc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdnbzoif.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2foqslegn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhmmyxru.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2avxqedhr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzpxccyf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oehcxgku.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ephlknfo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ixmfdkpt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xppqkhvz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzegiaer.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbkxlwvr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lapigvbl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjzrqyso.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tghtnhgv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oymodoxy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntzlpskh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlcoeelp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdtjtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utuqkwiz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rgojlsfu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rcpckhmd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dgyajcli.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cyrbltyg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pbnqmtxb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bcrucogc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iowncmvo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hykrjlko.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cmynzjph.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kruubvvk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2azoveckv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pymrrhla.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tjzqfvqr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2izmbblks.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gtcounaf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mlmbapxl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xdernavo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tvokltbx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vnambvis.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2hhqjfthk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2knolgpyv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vvhinwdl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uiyrisvo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uunbntgz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kkhscotd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sylrqtzk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dnvzlqny.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ulrarwwi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2keawgwgt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ewixfoew.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lruynmxq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qobjxuud.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fejjhthq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2nroctpsi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jebybsia.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2anjekcte.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2itarecfn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rdpkwwpp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2isokfdng.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fpvuasyv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwtbdbku.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvwyzubd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ecsjrofk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2warrrqlf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2viljzvnv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lwqqixvv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2panszgqj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2kjvubivf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hszxmqai.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mpretmtk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dyslpweh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2elbuggrd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vzpaqesw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rylewdtc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlrxrsuh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kdamtqqq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ejifujad.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2yxdoskgc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2smpkdxhj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2daypxwiy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lmecljxb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pwbtsfgf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ktoyajxb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wedvrecg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hpsbbnwn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2idypyehp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tygiktwa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnsprng.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cesrvxeh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tspvhiuu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2safbsssz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tjoflick.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mannxvwa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvsrklgi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsacomn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pcumncno.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfokpnzo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yiixyjkn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2iybcuavy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2tovismth.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjldjld.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ofirqcob.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2nbfslidz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bxlyozhf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gqukhews.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ppqxtgiw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2butazfwg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jqxkyayr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xthignpa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tcgesogf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2inrouzie.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pwlsqude.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zfkuvhpp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xrfnwusn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cfhvbobh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2egjjyjeu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rtlhoxnp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bxcsosdc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eouxcvqb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2culnvnck.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqavfkwq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2nhofcdtu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2glymngvy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2batrteum.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2scygomde.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2psmnmnja.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ndzczpuj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ajuqquuo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2girwdqfe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ibkjfqxd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jntritzv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xtmzlfqi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2voztwzsb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrbawzyg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uzemclcy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2futzsuoy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vmcxruhd.html


<!-- 参考信息 -->