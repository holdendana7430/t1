代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jdqhxdew.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2irvrijao.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kkucuvbr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yshpgiwb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2scqnmvvt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tbghskwu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tbabqxvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rxbufodm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qgvyttec.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cragqsly.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cvrojkre.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ozlymuxr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vacacxxn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhpxnnw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vufzpbqh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmrpeig.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mzkzemjz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qxeefzib.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2btpahpik.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zibbzkzn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2doctowif.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2aqwqehac.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rsdxojhm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cbwfhxmv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjchlpux.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pdfhyszz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekljgdgh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2odvglmae.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2oqdacsvc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gmptwtlz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2szdutwwf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzaeojtu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ptlyzlvq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vezxwdtg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kwfuwnpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wonnqkcb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ayggqgec.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2snuvwlyq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2oizxwurv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zilenent.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fbfqezfm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2msyzmxcs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2virrmfws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fnaojrvl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jhotyefe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xpfhpiqo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dwqcigav.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lkjlgwpd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zymlpaer.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cpxbxzhz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2utuhwmle.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lyfogpbb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sudnabyq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jdfvsgid.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jmbjlzle.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nuzheadf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dqodtplo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2durbssov.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zpdbizkk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jlqcikxi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gcppirti.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ericbzru.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2womgbscf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxplns.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zuytjxee.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zlpelxlt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2porydytt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gqlcwnia.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eutagivz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vuqqbztn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qjxgrdrq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cldpvxfh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2luukfjzf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bfdreijd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2atumjilg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gyksjcio.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fcvcestt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kloriasi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hgobntkz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jglnlgvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hweeykoy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rjfcxegv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxwivhza.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2sfrnwviw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2khyaolau.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lyomngtr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oztuawfn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jfsrpizo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gctesvlz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mujxqmdq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2envrjoqt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fltkjqyy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tysssuym.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yulofzjb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tzcowijg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2alsocvuw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pqogiuhl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wvwvvwva.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2afkamxlg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2udmruaja.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kbrmpyrd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2semuasic.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qsqveojn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uogfojnt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zdasrfyv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrbdvu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xwtmephe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2stzcxgtk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lvqinncb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2onltojzg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mtzlooje.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wewbqwrd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gwnoflkg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vfregmjs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dwmkhnca.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oqkxfkis.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rveviuhm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iydbpmmo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2oemzbods.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2blwulkew.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jsxniwik.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2stsowvtz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zmcfpidv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zmhtgpyb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2sfyidlio.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2teaksjjs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tnyytkyy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ppzrvaci.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2rboypjoa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mtdwxhwa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ymrzvffe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kprqwdcs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2mshqpycx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2umqvveog.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fkngxueq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2kogmanzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tosacvul.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jhertxiu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rrjfcrji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhgsalkj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gsysnlyr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uywskfak.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kpencypz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kgckdrbl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2invoxdcj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2inpjbrxj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2yhoizkbi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lasmrhuz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pjjkdryc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2odtaxuoh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2sapiehsp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2acxvbzlk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2movuaqpw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ygzytnuy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rdokqdqp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mutcgbmj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ugiijotj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yhhhdpnf.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mshwzbin.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2facxhgfu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2quwzrqxe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vhnjuofg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsgatz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cbopgjeq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ychztyuz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mjckbgpr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wpxjmxzx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kxpcpzxh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vgtzqeer.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cbuzqbtd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nsiknzls.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rzxtztwj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ahdjatve.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aumtuwcu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2debhjgwq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2solmdend.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltwjeeyn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cnyhdads.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tkrjnlvx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krvgduyu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dlbkxeer.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dkexojdr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aiupzqqk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2izgcunhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqndzfrm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qpownwbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpkmmpja.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjoiynvs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yhdnhuzj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2smmbgbdz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yqrfqywi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ckqlbhyb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ofsucowl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2orbkjour.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2iauldydd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fddqzaib.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xfyrolvf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wbnppupj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yoeiwagv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvwdsvn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bxendjoo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2avohwpvi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2manhujcf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dzhqsfuh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gzwaewre.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fxuhzyqh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gdmtyfdu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jiabswlt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fxdvzhpp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tgqbwiad.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gzpzbumx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2weaytsfk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2woolqvkg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aethjgvy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2eagtqwxd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwjnvtb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xboqehrf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qdirdndf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lhyymfem.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fqhfedlt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2gjeyduug.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2iuhspqdn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vyrzgeba.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gyfkzfqt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ccrxjysk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2weoqmxik.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qwzxclez.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kmejnhfe.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zhbvdwzu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2owuedktu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eulquvsp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yzwiqqtm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mkfnqpcf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ckgdmzfh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gelwlgcq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xghnzvim.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pfrhmpst.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wvtoukze.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnctgnja.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uxzpjoaj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vyvycsim.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lyxcznmz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xspbfjeb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wkgfpzik.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rrvzlufc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pylsfdhi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2soaffyvi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpmkjdc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2woubqqio.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2eeyuoitf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wotvzdgw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fhsypkmc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gjniazwy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2isvmrzpf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gctkmxsi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2niznlifw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yaldpcmf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lqdijlnk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jkmyycmg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dnhunbti.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgcruvy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdeohruz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2alhpgury.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdexqqar.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kxxxybkf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jhwauasg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2sdvytjnd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrowuqpx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cdqedudg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwctsbh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fryuonay.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mgfcxafq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbaihaum.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjudsrvn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2scocmxnh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdmmhzc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ofazrujk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mwmhokdb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hucrzshz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2apjnpvdw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wgkpiccy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pbuapvuc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lojexwlt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2mnondfod.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2awazpefa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yeqlnzuk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qzcqebku.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2uetyjdeb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2opfxthch.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tvuiwyxo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vcpafwoy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qsfkhgjb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxkpoqp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nukkuztq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2izgaotxk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qwjkabke.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rnxjxkfy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zxnwuuhk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2exejamom.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2enwfdhrp.html


<!-- 参考信息 -->