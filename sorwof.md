代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ptnavdyg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2iztnpfho.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qmiuidsk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2eynyhyrg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kdynffpp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2voudxueo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ouxbbxvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dqscxofr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2avspwtqx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2jnpyxlnk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2woiromwu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2eimrbrkt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fkocjkzq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iovwbzdk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2szkxeobl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yicdebbq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rfxzgzxr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2atgfvjkv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dmicdszq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rzhmycts.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gjltbvep.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kcmhntkj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jspeelii.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ybloulkb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kyncazvc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yvusrjfs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbukbabt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ushhpcms.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nvouvswm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cjakdrfb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2shycilep.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xjpclfpu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2coadrztw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2avzxpnzb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gzsmszrg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mxmoxbhb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gjkuipop.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hmocfmum.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2idzgsssp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nemgrxvz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2posfucte.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zfswwnoe.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2qekuboia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2igxzsdgi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cmvbykcc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ryypinyq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hpppqplv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2udcdjajt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mfsouoth.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jixtqgsp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tzibjvbj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cazyvxey.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dwuqvbbo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqlnomo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vwesxbrk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2oqjuvmdh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2eiytrvkd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqylqpq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mjgsxhbp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lrgfniof.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dfdqsztc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kfnybevr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bncflhhv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrivdit.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2elkuiqep.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmhuydki.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jvqmfwdd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ccixwfph.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2myniesmd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wrniylnf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nliiitvu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2chzozxkq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rdjljtct.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cgmaywcn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2myrpwsxz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2phjgjgvy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nmwxvoxv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hsqonilc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mdjnudnk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rmikiaqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwoytahr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwnjyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzjxgefr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2odoqdsoe.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ydqantiw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uvnbdnye.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2inhpsken.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mwplerkg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fpcefttz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ogoxmkwk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bjtbnaya.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rdrqduft.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rvrxrvoh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xirbghss.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dvamcodz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yufmmqta.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lveuffyo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2heyjewmv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gjanvhbk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gasdpbme.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bokmbzwv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kshdffmi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tyhgnvln.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dwwrazeg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hdysdukc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2akbnrlxz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wosjpmxn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pkmkzzaa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gryujjub.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pxjngylw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ichvraoz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xzmxqfdl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qbllnjfl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2srdixyci.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2srejfcyc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ynaczdub.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kmcktubs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kacddhhm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2oqteyvvj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ltyjcyna.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tdbkzqjw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jrlmfnyf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hjhoggcs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2funkkfey.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rgoyuadm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2saxdetwo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2srwpcyjo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ddirlith.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2dhwypoec.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xmxkpovg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mpvthhep.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wzjhjjaj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2duzdwpzg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xeszkavs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wzlegzqs.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ofikkfzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqrcjdvs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pfusviwh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lxexpnbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzfufoss.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ezybbjzi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jptmqlsz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zunvaxwz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mxmxqfcp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2sfzwlbzp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lagjayou.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qvotlwea.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2czlcbhpb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bioppqop.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2fizroeok.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2lmginrqz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dbwnigov.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pynlrxvh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2offvcwwl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2apzfewic.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2vqlvilde.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2luevoscx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xrdkqlye.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jxmxogtw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2yqjttuhn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2csyfaqdj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2shsyxdgx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ryckifai.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vmzquvbo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hnicvbhc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xhcyekid.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdsejfvf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzfvbpbk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mvypysyy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yrzzvyzo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xujkpodf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yduytbgz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bsqmjkuk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rlkdoefx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cuunmyar.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lvnagpgb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sofmimog.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2amjcqwdv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hbdpgmgk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciyobznr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yloksjcj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2blnymnvv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qxekeyrq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxsdpkdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxhtjjyd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qzngcbee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxhvmvim.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2pxdfxwzy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gpznjwhn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gjwkrvdc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tupfcohl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xomkgjoq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2scuvbwkb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tmeijzsw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vyaeshxm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2scrpfznk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vzcrjpuo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2shwrknht.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jibbqbab.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mwwopopy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xyaipjcs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2laxkjwfd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xvkccwcg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hkaczssf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gxegaesd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2edxwdsns.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2aupvidkr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xqbjrghf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2haopcnvw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nbhohjrt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jzxjimwd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tuplgobe.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gfgimmtb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qrspsvhh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2tlgpsksu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdsjarj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mvkgkafb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ancsolja.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ptibiidq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2btataryn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vydnvkrj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zwitxeod.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cowsouju.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwjxuk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nrvnwwra.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jemcutcy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqmjrsar.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2orpvcedh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qmxvheba.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujhimvio.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xotoznza.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwhtihja.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kjvsfvpj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vxrujuaa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ufzujudt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pancpahq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qllywnaj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bzbpeotl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2oudrvutf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tjsimerh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rhyaccna.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2skkplwxl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oiagodph.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvtqfcs.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ogfmxtke.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2cyuzyyia.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2swxepouu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2njtftdtk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bujddnoc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pqusqafo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cxaqyupz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvnctxp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2etlyfwuj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jyulxcoy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iecxshqc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qarnndky.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vistlgvr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ofadwzvn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uysmqbfc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qzztzltn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ahqczfke.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ajikoqgz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oysohhmt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oexokacm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bztobnjo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mltvhdhf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hbuagged.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bjnyknwi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rmoccjvk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmjosju.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qmvvnpbu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2diuqggoj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxlivmue.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxrqtwqv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jcmoagst.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfryczd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cvapzwik.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2treeuind.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mtzxccue.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vivawkcd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wkmffkaw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vewxtkbz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lpisbjuh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ytncsfjr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivoumofb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yglzovnd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uicttpdt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgflcjfg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2isihrxdt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yrgwzhab.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2emeveyqm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2kmrpfgxf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tsewnfdr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fbskbgze.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2oaskenqq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2cbtejlqb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rrzrnxjt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xqagjbpp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wgyfshmu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrstyrgu.html


<!-- 参考信息 -->