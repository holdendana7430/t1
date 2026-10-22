代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kbjqvcoh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ssdsjwxo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dhbyhmvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ylonlkxv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jcjczdmk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fukmhgjg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ncjxifov.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rmldlzdj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cjlyazcl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vruciaas.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nslbiavp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uwzklbdc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2squjtrxw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kvqyfhos.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2spzwqasr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzzvtcu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cykxsswo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cpmvsiix.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vxgjkocl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhyxeur.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjfkbbqo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mkwcouto.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ronjiblj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ictnchpu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ryrmqlsy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zfqmrocq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rnuclafz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2plurehct.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hoypkilg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gjnguflm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dkshfizz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kzpjgypc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fxfpbxic.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jaefahkv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2umuybrfq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2obweryul.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2oijbfjuv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lcqjzlms.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mdpchjng.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zmnunbpu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2kegjmgbp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fsykhuxz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mkfzadva.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wepowkpp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2althjsww.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wtheybbi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wgsvtmde.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2chykdaji.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yfncbwsw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qaeokedg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mspzasuy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jskgyvel.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dykebvrx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lkhhyhac.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qmtyqmdg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2uslspnua.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2evbwfwgy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zgtljgqs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nnfrqumc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cmupsklv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jztdyyjt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jyhgtrtn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yamrirqd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mysnnonj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kwhnyucd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2elnterop.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2esokznzf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umgwqhso.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ywokewko.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2znqdhmvo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2euwkbubc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yjfymtye.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2csjiozws.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2knofyzwt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2yecqcudz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yrudivdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deaergpk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hvxwviag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opgfmaxe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dtzhaowx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ygigogyb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2slyhpkmf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hzpenpwf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2juntmmtq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ztlponrx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dprqjoyw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zwmyslwc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rzuomfmx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2riitziqw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2axlukuya.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ighjwhxa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jytudtag.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tssthfkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vpfdbboa.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gdinuyaa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ppponwlp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wnqpdddb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2palkaloz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rdxzqnwe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rlubrttj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yvaqxuwg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ifxmlhht.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pwogmyet.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kybqalua.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2njkulnhp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iuargmyp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2chggtkee.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2spgmteya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kubelrkp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nntvukau.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wtdwsoed.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qmgufrec.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gzacyrwv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2oomleuco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kdnjqxft.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wpuwnezo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wqfzykji.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2yoydyhhn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mzxrttcm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fulltdtb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nbmetqau.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fpyghzlq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bcpylasf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bdezpcms.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lghlzsmm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2whfxfpoo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tmohbcdd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2atwjbbxh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fqrecwgf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zmvlspfy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2orcfqixd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2igcmshdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvvdupmv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2iaftmdfy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2iffsuduu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwovayhn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eppuoqvo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qgyemdjo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fdodpyrb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bgjojuit.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jpuylpbb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lnfkjfef.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2elvadotj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wcqpedzy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kvmjyydj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dqkzyjva.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2oqturqyk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2swjqjyjn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vhdtopkz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2gsvhsvii.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ibadfbnt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pqhmpcge.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2reoggsjj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ulmwfuyk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2uclvxmyk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ccahbujr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nwzkhift.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2yczdpfnh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hwxnflfv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yznlclch.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wuqqkgrz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lpugqdap.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oogtdyku.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czkhtrfl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hjgvsitm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggsyjfnj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cyvcytep.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kzomjelh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zelwghfq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rawqxstn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rldiqpsy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xskjwlnz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnoueykr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2nrqfrbmf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fftfqfwi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2djdimuka.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lignntvt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jfzxutxp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2direpzkp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qwcpcfld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oemvyjil.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2phvkqzxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bczfrbqp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2aulewxpg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2igsqoawi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fhaxpuqa.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxvdny.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wlfzoczf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ezegwoec.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nvimgdgq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wdhbfxvo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jadqthcv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2kbcqstym.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mzbzimax.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jqriuorz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aeizvgdx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xcrsarhq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xgddcosp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2yiyqwavj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ycbfugle.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mpokhlys.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bisdpasi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2owismwmr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tagpxgch.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zouoyohn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nadeyfix.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vvmktztm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dbeewjyr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yabeedar.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ommcnswu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ddxqladg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nexzgppx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnnptfha.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2inczrhcf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nknpdaao.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2vbjbpyzy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2znpytaay.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gpmmuldq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nlmksmqw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2kjsqvhdf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rsexuulc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jcporngx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xrsgbzcw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kubniwtw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajktmvcf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yanbopup.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkniuoba.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ztcvwive.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hlryvphr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ttbsfhen.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bswxmxoj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdzjlw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ixasctby.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wlegriix.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgeoune.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2mitpxbff.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dxtwyqna.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzudhxmq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hirzdfvn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xuhdcwcy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kfrrnnfk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ncpssqts.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gftdzrqm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2whvlekaw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2rtadohei.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ztvwsncv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bclfbyjs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nnunyxmy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kgmoiime.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2swbbdacu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmetkxt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rhtvywqj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pxktyjra.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kggedxca.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hydsrrno.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fsnfzglu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bpihetyu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugenrrue.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mprovcpe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vojkejln.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfyfrlk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mmimbdoj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rxfwlulw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mfeatjwz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pbxrnjuy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ciudnwdq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2babbehnx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxvgqp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2enzfcksu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hdrprclj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2irgjyryx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rleokltb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2pindgnir.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2cpovkaud.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2piomqcnx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gqproohz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tmdptgqs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zcqivrfw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kuymrcgm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2sunabuwh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sfisjoim.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zyhlaenc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stfnpfem.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2wffkfltl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2awmklwdp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rameerwn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vjgvlssv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mcaqueod.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqdfjzdc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wdfjzycr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2knnopcsx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jarwbgvu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qxsdtjzu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vkdulrls.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mfjsuxne.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lztfbnau.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gdyebyhq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tohyygug.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nbcrmlpr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tkyytmtf.html


<!-- 参考信息 -->