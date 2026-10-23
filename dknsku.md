代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kpzujtmn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3setgacdr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3chzdjxrm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rqoeslec.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vznexafd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gawzftgk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hrxenkvz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vjxyamgi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3txdbvdge.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kbqvxhwr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ozmqymbd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3moagcmtp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3guwaqkao.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mbrevgjx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tpgkyzzv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gfdplgli.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3edgwwrkk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ciulmqfs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bmkfayve.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3glniuice.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lopfngfa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wbjcqgkc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aknopheo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rwomwgfw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bthkdcaa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nsuiwhwy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hvgtjzze.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3komsprfm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wpomvfkw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wpnvvrsp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jcjznqxj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gttxofmp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nkjnjisj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hffvsnrh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3spplaaoi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3txundjsv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ampnmcar.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3koxugzwb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3konjhgxw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mnthqxda.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkzfffuo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3coohblhz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ghjohvde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3biaahyjl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3frszatdw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jffacsyo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dfffgaxm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3quecbnzz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lmztvrxz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rxurqtvu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tlpklfny.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cfsfcqyt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3opejhjud.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhkfzwr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3twiajdth.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ipahcabc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nefypptl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3enbgtzba.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3aazhwtno.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zekkpzbq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ywlhmhqg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ewbrrryn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3raxjydvj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kasghuhp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uhdypwzf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jzupwaxo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kuwtobdk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pitdsnys.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3imlbwjqz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ojzxvxtw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3chjobhcc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znacpxct.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qmtsrgng.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zudnejsg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xcqrpapj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3iesidlcj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ynlrmaic.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ztsnfjwi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3khtwcrre.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kpoewgor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npkiecuw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nmgbuzbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuhviocx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uvodyvtn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eegeehvl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3thptmguu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yanredyu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fojymwvm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lwsiysco.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3agvgttgx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kqdjqwxk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3euatpmux.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cymaotnk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3efhrcqvl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hoocqzcz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3sfgccozm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xveqmkll.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kdkvonzq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wbwxjpww.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iexhnufz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xcfgccgz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vfmyfxkr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uheljjfr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bfdewwpr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tgxlvmad.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uoylwaiv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wsfijfhw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3deewssmo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gortsgsk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zhmqyqfb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qrenntau.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hshgguat.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bqivardd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3meetlluq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3swflezru.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rhryjyeb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kiltxlri.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mhixowbu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wsspmmor.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ikalrcbf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gtgfdbhn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zkclxsly.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3boxyqsrx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zgomjfvk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3bytdxaam.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wstlahxp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3trmiahoz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vjqcfcbn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rgbnynfk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3azzbliyb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cegmlgww.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dlflzumh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3sihqdkvc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jebklzjm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3gtwtiywq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xohnnnad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtlkyxci.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3msptwlxi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kognmiuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rywqznxg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bnsyorwk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yfuwrxfb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nwrnvxey.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3arvqfluu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zpeojumh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ftrneppa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3waonbwmd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3mmuonyzz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vlthgdtk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3osddppuq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ziwtpakv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yidludqa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jvqzwxdp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nxdwgcfs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ogtcamwb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dumdvhnl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3iqcdpwdk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jkialdqz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uvsqrzzm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3anoxkujb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3boatjwup.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3csnxctfr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3usyobqex.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3deueopcd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuqbdkzc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sylufbjd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3agvmcfzv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3clebsktw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mavfucky.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3medynswi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gvqwxfmf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obcxgepu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujgpnnlu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3epbrxmpe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hzqzjlnt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osabrxkt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3okwxdxiy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vldpvvbg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3knxwuvbw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfqijacq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srrsyonu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdmqyfmo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rkrbiqqx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jeehfvga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfuglopv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mcxnixru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epsxewkn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwnjbhxm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ndessqex.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbwvdv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3agttifsg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gnxcvfdt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mfphkfwg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hbwcgxjy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wlvdbuux.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vzvplkjr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pmwccdvk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3awkbdjsy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3siapnjmy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3begujeni.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ojyhdjci.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cndcvixc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtlxkn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3znparnji.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xjovcujy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3sfevqtmg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qmdzwunj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hlrjdcix.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3alzzclxr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3teentwen.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3khamxoiz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hbcfialb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3joqvnnku.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxqjlwkb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3srzxnfma.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qaerzwkm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3obbilshb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vppomwkp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jamuutxs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wkucovhm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3loajzlpc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3lcecdcqo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dnvezjsq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3amkswgqy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nljmfvsq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zsqqquiq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gfkealks.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xapmwnkz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3upyrqoml.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrvgcykq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yimnrubq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pozdxape.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tyfpbybq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xmlhifxz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3stqgmfhr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jfsdnzks.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mlmzcmib.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xmllvvfk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qlvhkbwn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qvzwddkx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vipthenw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3asdaikdj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkxvhzq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pxpkjvyk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvsyvwia.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3sgcaolit.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rtstbcnt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kgytfbxn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ojkgyeld.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wpyiklyt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cjqcggao.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yhczovgp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ppvsfsom.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lvnponra.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jfbihxbx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dhxepwez.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dodrjsuy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xmtgrmrj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dvrpyjei.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3phovydwu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gaiptiem.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3esvtxcvk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrekpepj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jptuakrr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wkznqnyf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3icvyfwod.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bdynrssn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3buujsgqh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3snaztmpb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qztkboor.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3kafjxyhh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrygxggk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kbpmuska.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oibozmkl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ardswlxb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3moljhjqa.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwmebdr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jphgqnta.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bunueetz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bdgdgxvx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xworzkao.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zvofkezy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3waewtppd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fobvqmbl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hynwqqxz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fucyssje.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ykryxotb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgezke.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lszmixyh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lvkqndbc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fwznqomp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3luuwqxps.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3agtdafnf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zoqowjjy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ufzetqdf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3czrjxxxh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fgvzhlge.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3snorjlpm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3envkqoko.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eoyurjiy.html


<!-- 参考信息 -->