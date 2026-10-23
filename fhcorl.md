代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jhevqwal.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wjbyfqli.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yclsljti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3spwoyauo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ymlmwkxk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3rowoakvj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mznaehxr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3operfekg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oybxbxsw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hpjptutc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qfsnkpvy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hwdemcbs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3galkopmt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mzjdoqvj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pzldzdpc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fektfgke.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3izgsbztc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3urendzrp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wjlsnfdg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjouugs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rntoqilh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wfuflhxs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jemsmngv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qqkjlgjc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qualyuvr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bpzonlbl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ebqcnupb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wszawmjn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vbftxodi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tvwugatq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3sehyjzsi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vnidqmfr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eqvfubuk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mdgjafbt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ixnqiqnu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tffmtmff.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gfimfucn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3millpajr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jyzeubzl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jzokecjy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hcgrrjur.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lbrferrr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qgczrqrw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bfsqbbzz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cthvqujt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gcrsjljm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lthyadsc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lcogzmgy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fwmmaoob.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kmyuqysa.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3giwteqoc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtultd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cekolwig.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlfxcgz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zktqkzsb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3etrwlacw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dhqpakra.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3luuzousg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fjpelojm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lghzpscz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kwuwnzlp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3taucacpr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3touoapxw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hyrdbgjs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lcmcpbca.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pilbvwqa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tuivctwy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xnoggdbk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bwtleoiw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fgnczbeh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rtiilidn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ortihqgu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3eeulyvkb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3aueirten.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lgemitnl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3mdctrlfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcxaqjdi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vccyzmkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otxsdrbh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3btzbngqo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wocafvwx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ixdqtvpd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3slffmumw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bpodtgkm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hsirwnfe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qivxmovu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oaqqtmcq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xzxyxzro.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3iqbmxegy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dgmumwnn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hsrtvyqc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ojvcprim.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rfjmqwve.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ozntveao.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3orfohepa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gbherpef.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kplzhtjt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ovahopvu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lwlhnguu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wzghulxk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nnvnxgym.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kgvyiafm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uoedqlbb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3shdsdeey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cqepdyix.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qacelmlt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kltkkhfw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bqxcmozi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xemuipaz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3abqtqjtr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yweuqzvg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3crijcwfh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ltxdxtuk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nwuqvcnc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rtscvdhn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qmnryytx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jgrvidxi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mrcvekdj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dsaachyd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jvlsdajz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dcqgpxgj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3myrjmwsj.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cwtwboxh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xltnilea.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xztjflxe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hqqlwnlu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mtugrtyq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xvaamhvj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qdurihzs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ssgouckq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3eumsjfjh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3belxlere.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnghkaxx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nfmikcaa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3umqzfqqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouzmjvqw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uwatrrde.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3igvgddhm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nuqaihbj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rlqdeqes.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3muxycmlp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rylgwfbq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sudjfwlh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hnetokar.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3icpavijq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3djsgrzxa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3uchebfaf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vgnoawor.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3snyscmkr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3tagrfagy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bwhuyoly.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3eqlpuvve.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3joathbmp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3joorwxej.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3yaaksjry.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3jbibkzdc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dmtoltdt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wjgrpnvm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fhhsmwey.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gwedksqh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvdlgtbq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ekjcuxum.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3iuxhsgwh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pikvyrcy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jwicgwvw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aoqiwupk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3krgzcecz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gnxptnzk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gzzhwclu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mawvolce.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3taqkbenc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oeufmtcg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3otpzmuta.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3czqqkpgj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ifjgfsrb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jmxjozwz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zsksdizv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ajgemttu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jrhzweli.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hxlqposk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocikuvrh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zmekjgws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkyyogfi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvuuetlb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uwvldsuz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ivpxxgjs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mbzyehwc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3eczwqyej.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wveoafgp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3poduzzuw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3odxfzodu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3esemqyap.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uqanandg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kqmdpbyj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3szbunccg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wirxyzsa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yawzxsip.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qcezeokw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cscgsxef.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rbleyidr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hphigslx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3joxqjwkj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aoatxiug.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fqeqfofj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gpqiuiit.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bbyogdcx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3afigydrp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ehweocdl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3thnxcpcc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xdzglruk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhbdow.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zvuectck.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3pmacszmq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zpfbyznk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kiqkblkg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ikcvhhhv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3edqtcykc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjybxsj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fvbbernn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3eobmbgjq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3emvepahn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yyjlwhoq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eqqszwcg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oauhweor.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkrzki.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3servqeae.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zqappxpj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3chaitxmh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bdjistbx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zetsbowb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ziglgqgb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3drcgzdjq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gaixzhgl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bodhojkt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wkxlimnu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3armypeee.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rugommzy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dgfaczzu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kfelpbfs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3plnecgfz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3escixzet.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mjisqcrr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vhuwzsfb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3encndnez.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jxtrlttz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kwgandrm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3puirczzn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jpxbkyrh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3nyxebzcr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sktwhaci.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bffymwzc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdioyvd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvtkjny.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mbktkelw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zshedaot.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iyvilpmd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvddohoi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyiwghj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3meozwgzt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jrrenuji.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fzrwbshr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fodwkvpw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3epllsfoe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3whhxcrdo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bvoykxpm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vftlayxz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wqpncrea.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uyiozedz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3myskktls.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gdemaadn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xjxasgvc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wezzljpk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dlwgovag.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rhgotsau.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dqrovbdj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oakkplqg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rdwpwuof.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mykvxsua.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3idymccdu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bxoxgcef.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ujrcyaxf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gbvrblgt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dargokrf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dkcbtkib.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xmkdknjs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hccbnfmc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3krplumgo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqmxkop.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mgxeajpq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3epmarfjb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kvwgmhdi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3nxlmevys.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hmscpoiu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3apicxmfm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rocpuryq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yqahxjdb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ilvbyugl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rtqyoukc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ypyecdpq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ypqdzvzt.html


<!-- 参考信息 -->