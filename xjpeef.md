代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wkojiaml.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tfudkqwm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2tqvncjea.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2czvgbqjf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xzajlwbm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ytqjmuxl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2huboekrd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2iyhrlwqd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yovrhmil.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2icwqbhwe.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2beutvpoi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rzfhpoag.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2stafhgvk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uiugxvxf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cpkbpscu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xoznqoxi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uudkdbzx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tluujrem.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2paminwlc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2usafbfeh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sjbcyosi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hjcmheno.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dyffqqty.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dwhwnjsx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uevqxbnp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mvqimspw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jabxfgew.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2olcavcft.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qkgqahjz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ngtfywho.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yvkxrudi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gemaqwaf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dikdsyke.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pkcijngj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vmcfdyaf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2shaqavty.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fvuwpipn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kiprnhar.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zhoyehgb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gxujcexi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ohbtfjjq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ltrchxfx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ijnrfcaj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mwwudwwc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dhhszzwt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tndkacjo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hoaktpiy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2leyrsqsk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fcjneiez.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eizmcfha.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hoyorxto.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ikkzoitb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ybocumzt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bpdzettq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fqscqlox.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ktuniuub.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fyequhku.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nhutufdh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fyuccobq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2augduzgu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vqkjjxbu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2udfsiinz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2axeskvej.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2whezwhih.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tadkgbzn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhhwgvp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bcmliixv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wirokexe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wcdizcsv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nfayyjvb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2bjgcteng.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rjcjqpep.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qoitisca.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2slvnzubj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dujclyvo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yrghkugj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gnsjnbet.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xwscllbl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xmttteyl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2goxoxibe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdljyjsg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qwqayvza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjktpuei.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lpenqcxu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hikwxnby.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2noioujgw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wafvyane.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ttcwxiav.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mzddvtyq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2etgoesut.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ktxuvkgm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qrueoiqr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lpjvcifz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qgeuktti.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rylazpwt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2klefzvpc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zloqeysi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2eqdhkcul.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qmwtlocg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nmqjceds.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ehgpxukz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2orzrcawb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ujsecoxx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zhjgdcoo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ukxssdwr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dicfiliy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gjetpkjq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2crahujfd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2usgbiytl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zzkzihun.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pfcgunff.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vkyokynh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2asxpndqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ztaoxghy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zoqzmhhr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ipwiqotc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2coqnknyx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ozkhbhkv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2okldanyv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jwzmimey.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bkqkxngk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xisdnsek.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2awjdvlbf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wgggtclj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmbfkf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yylpudgb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2losqqbrl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pvtsqufh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2annuamll.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ezsukdfq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uknkcpzw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qyfgbaph.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ngzpezqi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2egtipgkm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gbudjgji.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2otobxnsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoqjllow.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zwolpdoq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2toclhzzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiznzlhz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ssdppmiu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qgatdaqx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jyawdtdw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2esusgvmf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uhrpvfqj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oxmatlnw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bdplkfnm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vihmjees.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gfsuefjm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2drbczmyn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2iicpfyov.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ufkplqux.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rptpsaej.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2udxqurlo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ffgotwrq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mwgrrxyo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jruujqqs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ywjcmolx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2yqpshocf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dwwepedy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pkzvnkdc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ergipzlj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jdzucokl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fndmgnkz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kqgabjjf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hvnjvojp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jurmiunw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iaekrxqo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrfnvivk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mxkjuano.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2esogrpcl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uauhmyhc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2saoayvnr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnkbohoy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nuiqjwtx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2htsddoap.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2opnkakqn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2zcomchrs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rceslmda.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vqsduicc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kqsbdvzu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2slzognrk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2snvrfsyq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2swnujntz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymfviiiu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qlwycnhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzcocagt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fkduvthx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fsdhbcem.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2clpxybuy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vxqcfbbt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ksyydfnf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mnkwbhcz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ayzetbcu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kmldmgug.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2umosedbj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rqvzdpnl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hccjvcoa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wsnkbmsc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2syajyztp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2knfawcnh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sriknbqe.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vimsrmvk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ntvqxezl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ustfokjz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hjteqqnj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nhcqzktj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2euynxpux.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yrwhjsgk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eymzyeyl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rmgzmzck.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mnxqjlsd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2opxtgqrj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ulevckxs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zztvbqzf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdtdvrf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aobvaxuk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zpdswavg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xciuefnv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jlyoyesq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2apdxyqdm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2sfuuqlzd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zcrqlcvk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2qmeeutyd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lsiheyxs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2netpewnb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ixqzbkig.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rjwhwiyj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ggfmisek.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xkpgksay.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fifikyaz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2joexzyst.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pcqlxfog.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2frdsbcld.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ryjvmrdj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dxdhdfnl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jtupozgv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2npvetgmt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2wmbgijko.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2khsguewm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ygfijlxf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2guesrakx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mjarpfxl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlvbzgr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2cmmumjjl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2cdlmtmhq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bpcrdezm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jtunizdc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2oejoankt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nrcagdxr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lkoxkltf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tduqrehb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbkecju.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gxshqjpe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2knkrcsgo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ihxjwnuc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2roomxfbv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2eqmvnmdu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gvqkkxbz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2igyiwmpu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgdezjfn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgaljiyq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfomjre.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptrremhz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nbojkzva.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lbyvcqer.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sajdpmva.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxahtuuz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dwbapgrb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hrfcrekb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2seyarwss.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2equxvafa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2udzkoiai.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ouxosepa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zdqrijzw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ljosrhim.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2kpahchqo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2poabvsox.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rofcpotw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zlvxfjqm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hsilejel.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2klibomxd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ysjhvpnr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pjcqsbkw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sfhqlbgh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lunwucyw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yspiumzi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mdrsdjax.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zodtgjim.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nfszvvzn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hfsppcfd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2eypotmav.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ufjvwktb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ncrtcsei.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gsbvlxej.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dhyrqkar.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pvdixpte.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dpyrngnr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2snlkjwqw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xqjihsnx.html


<!-- 参考信息 -->