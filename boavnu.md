代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rtcmajex.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2thrpynzz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uwgmiogh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qnimpcic.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ivuxppbr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kitzjoec.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2blquibqy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gbyuqtxr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gwnrfbij.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lroraykv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nwhknluk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dlgmawfk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rtfjnbkl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ahxfvfqo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mssgeorv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2erlouwrf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdfiok.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ozzyjpwn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2niwmkjub.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bpptoulv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ibsclkom.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kggoyeuo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yvhdzqyl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2azeadoim.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2crhbcqgl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mvelxvuz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zhfatiny.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zciungjn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2imaihzfq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kkwsomac.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtuooz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fztevuve.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yuhtxijw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lvatlceg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uquanxcw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2iufjxbyf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gbddknrp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eneizrgv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fvqqwoql.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2iezuxrsy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ywbzgukc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gjbrfyim.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vqrahkux.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2usvtvlsm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dnoefkvc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2opvybrcs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gsncevzn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2licxfmoi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wlhkptql.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gnttvrtb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ndceuzdl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2evqveivn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fbguahcf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gbeoilgg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wqtvaned.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2klgajqph.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ogwliraj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kyyaoera.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zclstfzj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lylybzxc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2edgimtnd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exzsyjar.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rtxtjeeq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2icfjjiod.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fktxngcc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xscwvuwd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zorapmtk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ynzrfjxj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uyanstbg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vanpfknt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2yayaxmbg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2geeilxbi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2civgdrei.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zbvlyiea.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dxvflktj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2afdejdzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osmhxmup.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uykrdnbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inwosqaf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qzvuryjl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2shclmhqx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wjcojydv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fetvtwgd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ixnatwsu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ubiliwvl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2visosyty.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ytznkohf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lhmayekz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bazcrvrg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jizanrkl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ovddvvbb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2grejsknb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xilmwftp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tmssrksp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wmsvnpob.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dulahnyl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pyvdxluw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rpyaeypf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2utolpuzp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lpzeczqj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wmywoefe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wwiknsze.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wfmqhbvt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rpolbolq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qaxbvacb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uhwcwttl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qkdmipsy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yukgcrsk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fyhhzbcc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xnidywpi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gpepvgai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kunfnvfu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2flfeldlm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gkjtkuzs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cayealzl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mipyodrq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tsvhqeul.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lulecdyh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2htxkhlpz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vhkyzuge.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mrskomqe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hyvolyjb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ihrblfqi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2asoeqvsw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tnnvqsdj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2twlkqtrn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hopkcqok.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dbmcuano.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2exritvqa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mbxdabyk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ybymcsgn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2yqmrjuhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpdqniss.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lbymlrww.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cblnhtdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxvqsmib.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gsrdixjz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2afuoogrj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nynlgzcf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vvqyjshw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qnlcjmfs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kavuyiaf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lytmwvot.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vfdmogex.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pxssmpxa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jwyaagtr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jyynmxwz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2cmdnzeoy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2irpvcwsr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2grjcvdha.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2guqknzfy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2vrzjssyr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pqspwppi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2izxtqpwr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mkcibrhh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ouyevosn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vtefswja.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2aexseywm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zllzdhfd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2npnjjpdy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gbpipbso.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hxteujyl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qlrkvovy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2yurbtlhh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugqhcbei.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eknsahhz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvecmbyy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lpjxeycr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hbhxgtdd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ccowqiap.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emqphrcs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkeubxhi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vwgbmpgk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecxyodpu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dhpprlge.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2osvegwcz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afhbibnq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zamulqir.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2avgmnldt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qnflfebg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enwymoen.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lyrjyunl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htmbkysw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wqkuevyg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mdclmcvr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2smxloskz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hjmmguft.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2stqwoasm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2crnjwgdq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ppathlvh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2pexqmhhi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2evyjyaes.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2fkjekukt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2iceorusn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aehgbnzl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xzsrkckm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qrqdxlax.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yawmezga.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2llkvxfmb.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gmqujjgq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2btbmtudn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2blqszzmq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bfvgjhza.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zajckkhz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hqwqgdic.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yuuqnrsb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zjrseiox.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mmumjtwb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oobyhtfv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhofkgm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2tarkffga.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2onsboemx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2abhhixna.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vhwiqncb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gvluuzpw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2skgknwho.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vfsvouva.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2mqkvuszj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rotuiqof.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2hmkcmowd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zuxtahsa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zjrdshtk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjeasvxl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gelcfown.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppxyexvw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnvhjsgo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bigplkxj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kpivjkgv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pqompgmj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wwpatdmq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ydtdvhpf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lzlwvtea.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sodeseea.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eppbqvnp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2buohrqxt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2piahzept.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jkmygbvp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2uyfhzkvw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rhqdcoxp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2arjvbuke.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2innynmhu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zmltmjfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yaktmihl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2jvfylaar.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2siqllnzc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xowverhg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kusdoasl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jtvcxwvj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqragjpk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2txvpjohv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2kddkgzjo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cxbnkugx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kmzaxmpu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kcpwkead.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2atgahhhw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2toovviik.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzkjntp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gynoikgm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dvetnwfn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esrvqccs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smakfqqb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2mclyoqup.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wwtqswto.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apmptryv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2aaeybaqa.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfwuvbm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2svyeffse.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tpfkujch.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqwyklxh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypqoccur.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2oqxvffaf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jqwkxpmh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmdeimu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2pvctnlqe.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zhzkrksn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qgrjnfit.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bfnndimw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2apiaqebg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dmolfesw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ixsnixok.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rmpfvldu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2svgdagqo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2tjycanga.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2eoousqba.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ugbyjvmn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mphwzzwe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ipithtfm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2yqawmuvk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wbxyjreg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fsvssjtb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bwrrpsed.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2slkcmzzf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sdrqhhiq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pxqhbnrl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cztvtyyh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzoykyld.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqsuldsj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nfalooio.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gvgenwuf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ijkwlbpu.html


<!-- 参考信息 -->