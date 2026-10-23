代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zknalmgp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wsillyxl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3aazbaetd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yssukeqb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wtnncepj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3plcqzwbf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wuaurfnv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yzmghnxd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mncdtlvn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qvpjevjw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vypoquah.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwodio.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3asoobavf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rkvpzyxb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3nqwpknme.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cjfclyoe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sxoincjz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yisxjvcr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbrxeikn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrosnyob.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pyexnrna.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3thznioaw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lwmdgooc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mcquowhr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3svdunpaw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3onphzowy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lrzhehmo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xzxesncu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nydrufkh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aostaytl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rekcvzby.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mhatptii.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jazwazui.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ldusgedl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3icdjqpak.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3prkexwqx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ezbploai.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rphexbxa.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wifhsvpu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cafobxrk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jzhzrety.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fdgshovl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3elpqtxap.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3geaznfwt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ifwzefot.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hfkjgfvb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vkacvcyg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3afjzpmsh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rneryosa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dbziwtpe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iupwrfvf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yvnfwwhi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tnqcgwtl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdlzns.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3utwydigc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3iwjejcql.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rqhfafoa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wsjynqwg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3okvaekxp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eojfmuvz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3oaiwheks.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jabwmfgy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wxwhilbu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gokkhkux.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fobtorzt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bfrposqb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gorfwosn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipvrdfpr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdqcca.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fwlkgedf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3schjbbyn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vuusvfwt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lmyfblwe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ctvitrqa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ndcommnq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hvsgmvvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kavxplfg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3etyibnwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umdqdzik.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lwgganhx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lisjpahu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rlbtquwj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3egvgqmxa.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pykefzsy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nfdlquph.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xcroobuz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nafcwtxl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjiqgjda.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cwaivjaq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lsmiacnl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mqcnvrth.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3uyjoioou.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jghligty.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dujoghin.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3khjgtqjw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3orwcbbqs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3nylspnmw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yinwajsq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bjeayorv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbdkia.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qvmmngel.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fawalivn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3prtsezdj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lyhkamic.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cthdosqv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jjbthvwq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ctllaldz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nlpdmrsu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mkyhmrbz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pqmeyuuj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mlgjcair.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3coxuuduq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdtuaqlg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3woxetwmu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zbbqjysc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mpxehovv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lmcyoliu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3baoheiir.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cggjiyre.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jquxeqsw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3vmmfqkxm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ujqhxxln.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gcaijswm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uxcjdkqd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cgpmkwxk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ydtawggr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hhlwdmyi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ajsnidqp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rgunotmh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uubwolyn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3oilwmtoc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ugmrkpbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idcfcdnt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3alwmnbrw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jvgmytil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvbkmzss.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lzxvsldo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3wnovccie.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gzigjfar.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3kzwjhunk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3oiqcvwhu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tbqazkst.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3bypxdspj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kfdijwtc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ucafpkgn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yosdxmtl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3kdltbppd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yfiedijh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3gnltfxru.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3kwpcoyuf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fljcwvkf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dtzuotpd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3orkfzmmx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3esqbskkn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lbmuormi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3upjxmbgx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dnldrgco.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3iwfpskop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gaifuwui.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rkqlmzhq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ficcnixe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prvsxxjh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dqkkmigs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsjmssaf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xmobssod.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szjsfzsx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vtwcsatp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3umprkqyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3krftnqyw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3minlrfhn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3slehowdk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jowlpvzf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jooapgwm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eefmijeq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lcvbpfxv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uzjgckxe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kykgjuwp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nlrsjrot.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3raacdtfw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akhjhylj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iipmehdh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vttnsjli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhlcpwlg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iidgjbtu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mjjbmnco.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3didqomvd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tuunlnko.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ddjtupep.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wzxpnmdr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vghcxmxt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ahuvuvuu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3idmnywom.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tgqstfmr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kwusbunn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xpqcdvol.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjumszw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jhmpkzyi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3baimyvhr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ylsevwai.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gktmyafz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3orgwyiab.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nvtlanbs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3dimvypyh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3duqvirda.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjiqxgpi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sjqewqkq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ppusntam.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lumhkhmv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uxkgndaf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3okjomxhf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3elkhulbk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nxlytfgs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjmkhhqy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kqhpimdz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3snaaqdrs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jhzxmrbk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3umuwzhwx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jlqxsycv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ccjfznwn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ecmmrtvv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3yjiihkle.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oiccibnh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dsrggpyk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3catjpnbw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bqgcmbaa.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ikauiwkl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qtfffrqg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fyrubqzw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3atptndhd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3snqhhyve.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3thgdtogl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zvylxejy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rjsftxwg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oqhwchyz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mufbrzub.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ohodcrcd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gomcmiom.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dveffday.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3scckvmec.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bzidhjnv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ndecykty.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gnsfrows.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3enbwzgql.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhcqnvw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ysygvarr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3oermfsjp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3iuzvizgm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zddkozeu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3bamafjid.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bxmluvup.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fycefybm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qnltrcye.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fghcnvyu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cayfojml.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3evuhhzbm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fyzehmya.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxslplyp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3daxzzypz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3daqgaynz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flkxfuxd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgterrb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xqcdpdpl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dobozrrp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iodaatps.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3niqmkcut.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrkmsty.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bceexhtx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iiqpsozq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3afyihadk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwgbcssh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3skfkgbfz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3evzkyufv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ywtvokwd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3noqauztp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wlzaiduu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lfhdgvyv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yknevdhn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xcredwgl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kdczqkiw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fxodctjk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kdxcbojl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zpwyoyhk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nznddtfq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nlhbdknz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mhwwjwyn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ynomnrwi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qenouhfo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmbbhal.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uptnpjuu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bgjlusnr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rtxygvkm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3pggzmwye.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3twqzmoec.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vkrtjueh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sznerjgm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rugqiyhv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vosyscaz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ivskppew.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dhlxppoj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kdqmnqov.html


<!-- 参考信息 -->