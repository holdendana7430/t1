代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3obsdyqzh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wgjfqmpr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3npcskfry.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qjwcdddi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3yctaddpe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lsjwydgv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3irnsqdbh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xaaardwj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pdxhfeic.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zwekkaed.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ztvwdupv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gqeklyne.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kaxjsibe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3yrvntxzn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yvbtcnem.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3twrbpcho.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ebphgztd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hhwxfapk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zopndrze.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofgqrnit.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qmtrzxjw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cywlaqqn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yggqjmli.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3enahjxkb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qokbtdvc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cscdmznu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3awpcnonn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ylxxhuxb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3syrejrmm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jsufidgn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hdjrdklk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqserocz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3otqmhtrv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qbiuqebr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vlngrrfx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3msnxbreh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3krzkoher.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3elezpwbv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3msgdhwal.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lnecytaq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hrfksnsg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yahzecnr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vwmpkaja.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wpvdjesv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3phpzxqnu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3afbxkyqj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ywwivcjb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bgjsgazc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3caqrpbuv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bovnrjhd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nrruiyfj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fwppnmxy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rrhepddv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xaexjkhc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hllnkokv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qrtnrfrl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tefrctvv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bheckajp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hznzzdpx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wmaamycw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uyjxkozu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ahfymviw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dchexoaf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ihbaxucs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vuoebyju.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lsothnfa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ktwfaplr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3njkckyzy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ompyzths.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nbpucjbe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3otdjtwzw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jaygfyhm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jgcqhffp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3nlkwcogs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3svsoslei.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rnzrbzrf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pukxcdrs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ocildqkd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cukxeapp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3uuafdede.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuwnotlp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3twkszzdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwchudxb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jzsqhelv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ueotplhq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mslkxewr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wyioukgu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yyjqzlwy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xtuqyxku.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zjteazcf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jwwhnsyl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pkwexlly.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ahhtoqwo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rmijelai.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xpddmeab.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3swojqgyv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rqswllgm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wcqfhzie.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3psptwprk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zvjstpkh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xqznrncc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ukyaqngi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3icxeqqjo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vgvnainu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sqfbrnph.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3opqyuule.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kozjbysd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3favxjntd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3aeptokvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dsbohqio.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jljeoyot.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kdrlydrr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pvcbszjp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qkbrhkqt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cxxlenpr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rmpslfkp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uqwxikbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rdrvtfhs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3eesnonro.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ntghudra.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lrciinao.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kgartiqf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ivzfttoc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bwmuvcnu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dknwajdg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3onhystsb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uieanngu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mzbmjokq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3phfbvrgc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qsediaur.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gfwcpykq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zzdutqwz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hwlxilds.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jwluyspd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ikmubprx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3gcfwijuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtfgliie.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xtupidht.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wktwobau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxxmotyd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jvbishbx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ksjhistb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rghygsxv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3byhuewla.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3riunerwi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ldpxktho.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xmbzkvhg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gxkbavdh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3cqcilsgc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hgqrvogi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3pbbhrwly.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3okozmgvw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3niqsdito.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mbkxiudj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ihzlycrd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wimcdmxc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3crjkptlq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ixzxtstm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3twzkoxkn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ohllbcdt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xrvekxnp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vwynpuub.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qjmyvivm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ngsxskeh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3onryftwj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmzhbjco.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uafzpfme.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lnlmpois.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sxibwycz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uxpwdhnh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnbdsbhk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wetrsbrs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kxscsxvz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gsqggoxi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yqivzfps.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgqouyjv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zcbrsccp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3innxytdc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jkvjyqjq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmakktiw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvlxneop.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wbfzsdrq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qhjumhct.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fgowsaaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgyaekzd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3iymyawyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwzdttop.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3gzyiluaj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vepjcplr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xoohepik.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wnejnavv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3tbprqxye.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zmklkkui.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xvmqhcfp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qbgsxdtx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kfhxpwzr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bjtjbqph.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3iwtjlfji.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pemszlgs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kiamcqjh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3eoumhccg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fhqpmwkb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tlkkraxt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dvcrxuwr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dpnowohu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dlholegn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3amiuobiw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zpropbxu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lfmmjsns.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsrymkf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3myrsozli.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3clbiftok.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dtuayfzg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ygcrznoc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3przwclhs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cnduultx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3upjyjrgo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3eosxwmzp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cxqrvlfm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vvuxpmth.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dcmxwvfx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qzuzmowr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3mlteecjd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3iqgsrgeu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3cldhshcq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cwsnkakg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjqrxvxj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3auwlewak.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhlegznv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yiksmkuf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rdohdpks.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jelrkpem.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yrztflgt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kjsgledn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ofqnknjb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nzsavwal.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vocpyqym.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fgjtphgb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gngtqgtg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gkwhlift.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3etkmccly.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sxqutfjb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ntmrnjmb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xwytkxwf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jycsqnus.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tmqghhfo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3usykdmbn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3raziyynn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bqkxcchh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ehzxfarm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gcjjyucr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3selhezug.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3trckzluc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzmdtijj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3flcfqkfh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxiyjpp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ypihjfpc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bnitnyck.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eavdxycx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dqsggppp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvuzyzmj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nryeyhvh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3senzvglx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3purydndx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xksjquqf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3psxsztmn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3gvuozrho.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tlyyssol.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aptoouse.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jataowxn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cjauhpdj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xskftsfh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ssypiyqe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3huubrwzd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bmetscfh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmhyyur.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3thhgbucb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ejqfjkol.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qoczbuws.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3amjpxocq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dhpliyhz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3haiolyjx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xpdnzuyc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vycudgxb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wncoamie.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bxmalons.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwpdtqfz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dzpyqayc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tksbxkjy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eeksccdq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3guazttzp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bfryakyz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hxduwofh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vwyiqfsu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hmahdzpn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bfcrldro.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lknrbles.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qqxzvbqy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xrihzils.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dofsamzp.html


<!-- 参考信息 -->