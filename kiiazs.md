代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cjrzcsbq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qvaesysw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hzhqvihx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tuanrnve.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lwrfilyv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jtpubzsu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qjjceylb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2yobgrszr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iadmsmqf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wletjiyd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzkwhjvn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qwjqhvth.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bdabiumr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2oiiowymo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2yekqnnem.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qihkbnej.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bjaqxgdf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xmreggoo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyjvruyv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lkemvszt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qbioaxco.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qxqupgjw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vpdljohj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2avyqxeyy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2fisqdayq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ajgydlpa.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pkskaefb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gmioxbkz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fvhlhwie.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwgnmc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rllgjphv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ypqdxxkq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2bilkuhmi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qjhzzkad.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqgzzb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2edppsjea.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2legoiuyc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ybnvcgjq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xbzfmiqc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tctzlwcm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wydvlduh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mdyfixzh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dafemqnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pudbntss.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mnrkrpyt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vcymzfob.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2slinliii.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2azoijkny.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ovuxewxt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mstndmly.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ypgbwbhg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2uoorflrf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zpejxvpk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ffrqinyj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2weiydfii.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cjtzodda.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jvrgezli.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wstfofpm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rpjmusof.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxvjygh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iuuxleiy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iymvhesn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2agszrtvt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2odeisyyg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uwkqufxw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zajgznmh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2akgwpfmo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pksivbea.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fnrslxhs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nxrspjsq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nunoovjp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uytumntk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzijfmgf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwvjng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujpbofou.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2clnhllgb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2priagkmo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xachbnte.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wgekpjxy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2aeagtplq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xoacvsnl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kysqnaot.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hjmrsrrc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aekjoqkg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2armgqofw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fsemxkaa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bhpbmcoy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2dspgydpy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wkdxmaab.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ilcvdqvl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bicakbxc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2aacmwwam.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2icxvfvud.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nzfuhcub.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2hbphztbn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dpksjkbh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ergoytaa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xevxulbf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zvlmgzmk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cdvidngj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2puzvsibx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2loqljhyj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vzntybde.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xhrmajfr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qlhhxskr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2awfxhemb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rmyuzpdg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nvuwxoxl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ndltuimo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2smmnkqpm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrhwwl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2onaqftdy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zmtdesjc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2waacysvo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2losilmfk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dxtyvyrm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fzoknsxr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ibbluzpm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zqpopnby.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ramirjdh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2emxidsdc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uizgfoan.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vljswtdi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ljkytpba.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2atbykgum.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lrwezgms.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2aqakveyz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbaksh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buqlehgx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2orhfzvzh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bqaiaiaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emnkqowx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lwkjarzg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2iyujkoql.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2acwctbat.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mfgpxeno.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jywvrjzb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2inmoqabr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zaceewju.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2whbojqtp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xoaywkiy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2yfdielga.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2htsnlalm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zdhffstq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ucmibrph.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hldfrqdf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2belacgku.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wwadmhim.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrobcj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2osenkjmv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2iyemvmbl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wjgnshdg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2acxvxiba.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2bwaghmpu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rtghuqlo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugilphbd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lstpocjn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tckhmgtn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pttqgtbe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svtsxrbd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fbljpala.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fbaaxyub.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sdoyhxkt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2echdhyjh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mbglpxqs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cpvfuvve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hragovtc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyikjwlq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2byudbuff.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgfuluos.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sspqtyaf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2sdzhongp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yexmbpsb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zfduvhxa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ticlmukw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hnqzqcqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxfoulug.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fbyhvghg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxblcpqw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qicltlwc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ykpmtzgr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ahhpgcdc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pzekegxk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2udweboex.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iocuhvci.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bcqsjopn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2gzbejnoy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lhoktiqx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2woryxmje.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkshqc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lsbtdnss.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2awggcler.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kmxdsfeg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tigxzzhh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tiwsfmhm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2letdlduw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dlhahkwk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2uwlrqtpm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qtzobbel.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mlsdzrco.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jeewjiyq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tocghvge.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ayuspzoa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qydpsozz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oukirbcl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mptgzwfp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2edhhtrdo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fnkghamp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2swyypbkc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jdkpqqhi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kxbtvnmr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ogiwofck.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cgwynmpk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2dkqubidr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jxyevbll.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qihmquih.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2acvehdnm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xgjnmqok.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bpshwvkg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lypzpzfn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxiaze.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qhcabpnb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2azloktvx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2otfqntqr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ojyoadla.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ywecfybf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kcyvvivn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uznarzgk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eawpihii.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjujcod.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxdxjgi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vdwxjbxt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oaazhgkc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqzdqgqi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zllwvsca.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nxotcpaj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2sibtslso.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zcaeihcy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bsecidta.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kixsshso.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2njzqqeax.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fappqboc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ibdclbut.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ushgjhdn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2agyoniql.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ejjglrkh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2jdbirpmm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hwlxadqf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kescyhfu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yvbkxmun.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hyorqizd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zzlomxkh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ipfimhnv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ulvospir.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tqxzhjie.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcyknjqz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvsdfrti.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wyvbbwxs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zukczyvq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwzyvdke.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wiyhlrsl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zwpwqqdz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gnptjupk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzcnhkid.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdhqxlbu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gietuvyx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2weffhpis.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2npnbvgbq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2sckwtlzh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2qmtxksqf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kfubsfjp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aisxuprl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fezsleaw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sztwqowg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pikgpvdj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tzgoctyl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pchvvwzx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jkzlpeuu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2apubqidb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2sdatyrbt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ddwjblom.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qejuyxdo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kdkffqcn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rckbwzux.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jpousums.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bjixhvtl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wwbbatrh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2xeuptybx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bsdwilxf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ckvkrmma.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bvipwfpx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqtxkmkf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hrlbkmrb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mvcabtqd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2beuyfhxs.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rymsilfh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sxfgbdib.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vqyoabjp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2usdvdcza.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yokasyhn.html


<!-- 参考信息 -->