代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gefpklksb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ggtrvsrmm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gzcqvtimr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gtoudjshc.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gvxkccask.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gdxuobctj.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gqygtafqc.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gjjynkxgi.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gybmdxhii.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/goqnheljo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gaddscbmo.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gglogqyem.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gslochjpk.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/giytevbxd.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gdpwkpgmu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/grfhjlyzx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmwvqiuck.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gfzukosfk.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gurlsmuxf.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gflcpetpi.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gxwiqxzdq.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gpjprxgfh.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/geregdymh.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gcvfcmqlz.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/geoqhgkit.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gxiccvvip.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gytpnnyua.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/giizlawrc.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ghnhmlnay.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gqpuvkrlu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gowdbscby.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gzpyaiibe.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/giedylsdy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gouvxprdr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/ggfdmqygx.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gbewluuij.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gzzbberdx.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/grktcfyfm.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gnhfgusne.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gbucajiyw.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gtxwhmszf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gaxrbshqk.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gwpttetbe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbqvpsrxa.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gplnakory.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/guvdwizfe.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gbpbndayf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gbheiqjdh.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ghszyixuq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gcqqcjqxc.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gonhoebzv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gjlhyjbfz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gqxwnbeer.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gtkwgbprx.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gzguiyfun.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gdjeqlsnz.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gowfapmdc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/geholhapy.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ghhbwlayd.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvzxqjxwy.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gkdvcpmll.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grauvyjdj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gekrzwohr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/glltuxdra.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfbdpjdjy.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/goullelyb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gdkyohlsk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gchypeysh.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gaecatail.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gtqngmulv.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gbwgfzqxj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gbwdpusqo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/glamtlebo.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gvzelrlgr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gcruniilb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gueqoyzlh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gomaztjbw.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/grcuekjna.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmukunohh.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/guxggjcnu.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gjdzdcqal.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gytvbibau.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gviqtzfmq.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gqqolkyxp.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmkuxmlwp.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gioqcvker.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gpvyjqkpr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/ghxpyovjv.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gcfppkygp.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gxzmjycre.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gdqiqoblj.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gtqpzcsql.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gewjovunt.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gzfhnceit.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gkhdyxkon.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gblbveksx.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gjxtmtuzg.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmqihdapu.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gwibuijnn.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gqvkywhsj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwxaxsobu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggjsfagar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gequztptk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gvvzvbhyc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gygnbjsao.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gcecwipat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gyczzudby.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gxbdexprk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ggnjllnlo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjzyugkpc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gbdzcvurg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcqnjnuhf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gbghtaggu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/glipbjyyn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gozgcxsvn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/grwxefhss.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gwfsfbclr.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gofccckqd.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gmqhlfeuu.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gytrbskmi.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gwwabjwyu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gwwxtypzf.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/giffelsdn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/glxvzwjrd.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gdcjuerav.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gqbeyzqwz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gxnjxxjpf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gxarppmhj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gswejxvju.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gkwmnnzcc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gvqxljefn.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gosggxvof.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glmflsvfp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gvbbekdbk.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gjnvngrji.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzozpfvcj.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gazzdsesx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gtbbduuai.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gosixewdm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gpfunwuhy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/ghrexqqjy.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gtweeehof.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gdiwwbpao.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/ggxodtlth.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/guabeviin.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gzjjdayhe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gnyhmqddf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/godigjqvl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjhzwut.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gtmctluwm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gksoqfzby.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/guayziksp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gyrbscxsb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/ghrnpncnx.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gijxzukrt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gnnejyfnm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gurnaprkx.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gwrvbbnwg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyuorspkz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gotdcvuno.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gygzwuqxg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gpygsjzqo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhsggcz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gbnikaxph.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/grtxqzexz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gnbtirvlk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/glemcegxm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfhdsolgx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gqfchzytu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gifchzbid.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gupztzscy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxvmwtkhq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gjhybyzst.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gyvhxjiap.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gilofjsll.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gapctcsfa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gfbalgafh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/grtpkhpnj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqxswdqxv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gxawkrhus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxajfvsou.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gmsoxzrbn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gslcnjqlp.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gzwkcrgoe.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gmrkgnqdx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gxvquwvqa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gutwvbqjk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/glsyopvtq.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ggwyulyki.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gzytxaxym.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gjjuhlgsz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ggkhfhvyz.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gxbyhfutv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/ggcyfzsfo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/grvoenmga.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gooblbzeg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gntsgddbm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gahzkfads.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/ghzqruaiw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gjdfrnoar.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwpdfeicz.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gksydujwh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gkljjkgiq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gluhjzbez.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbxptfkfo.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqycwkfop.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfrnexznf.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gwxltdavh.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gulaumyxe.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gogpdlztq.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gllgbwnsi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gsecqgonu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gshzwsceo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gooealwwm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gosrysdwa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/glitrzxiv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gasvwvgme.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gzvyuloka.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gkmeppmnd.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gqxpydfhl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gdtbgkwbe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/geuztkjkn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gecbxddap.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glgszemxj.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjgchwozu.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjrrxwncv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ggeuvkhob.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjnnhfcvu.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gehainudj.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gvtulzaig.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/ghvhkyslz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gnuoffrhs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gabpcuabg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/ghliplpjx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gssedfsnx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gwvizpydq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/grygtkuho.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/glbcipbtp.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gbonsmint.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/goywdgwqg.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/glzeildij.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gzszqumwf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gpdiztazc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/glserpkpp.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gbvnibter.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gikummhhm.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gcrzrkqit.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmrorkybe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gnsnqszkf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gimqbxhwe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gakopkeav.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gpenlifcs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gytownvnu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/ghrtufcue.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gaimgjmsu.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gicnapapa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgpneyq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpwprwkha.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvpkiajxt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gumnipzda.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvwjievrr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/giajxnnsm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gylinfhgm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghszixcjv.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gflhzyfnq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gzmvztvup.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gavxqtozx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gisrigwaa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gmaoyxohz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gfrjpddzo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gxmovkxzz.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gpyqulktx.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/grldkcinj.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gjgplxfui.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gdnqvlpak.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gicpdeunp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gwqfoquhn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gbblydapa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gsxhhtnlh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gyjcgikzx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gejlikllb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gvahqrkmr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gtrgfqwlf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gsnxjigkt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/ggudiszfh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gbxfagtet.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/glguqyerk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gstanqqdu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gmybshdqo.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gcwalijyk.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/ggprpszkb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gfesehovx.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmkdyaebn.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gsriqvjll.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gmxlmnimk.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gjzukujif.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gaawzvzsf.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gpablvjlz.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gecrodeih.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/ghipkmfet.sHtML


<!-- 参考信息 -->