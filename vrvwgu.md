代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ilgyxaey.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yeifqbxq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ydxayxvc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkbrezh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yrxxknal.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tcqthvrj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pgbxbggo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pcvhsujp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zlpyzpgo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mqynmmgq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fwfbydjf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nhcwgies.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kakkzhqa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wfuzpbzw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhgorqil.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zfbuxodw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vupltarl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dmwuhtzc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fxhnfgip.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2snawbdhp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dpoqfnkk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hidmuorz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2izqqtkib.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2obfadgeh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2onjwhqzy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kwqzrnqw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2viztnzfr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rggenrro.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2uktfogua.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2euwtceqy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sgmwtuka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2aouftshs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tsqyvmdo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jovsljuo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bzwknikc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yquhhfzf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2shjcaayb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qqthodpg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uipcqayi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hvbiankr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2urgmuybj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yrdaogxe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yfiqfpwg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zfrhdfme.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fxxxsxav.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zzraxyfu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qakrcduc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjkkjl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kxnrvhvb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jpacoges.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2aamylnjm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdnyqfi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qosdirzw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2itspxujc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jgoswrsc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jcmoyhna.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cgrrvzan.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2swtxcrbu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fmdskywz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fekgrwyz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ypgjaajg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2htbomesg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qtybciqi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ymdkxcgu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2njzzoowf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2macjbwfh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ncxuuclu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mfoxqrlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atmooqbp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jpdbahaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmvkwqqm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2daartgas.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2oloehvbk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tzyeqrna.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xrhldkcy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pfllflqi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dyavfefd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kithgvpz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nvxlbcyj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gioepdjg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tbmjgycf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cfranunf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zthnzjyn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xgmpqaws.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fhqclipj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ulfkuiil.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2afmugfrp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pwrfovbp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bccxvjur.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kqsojvqu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fiyyhjkh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xkjwhcgo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fstdqraq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2swnbtqhw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iwsydquo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2srkfqpqm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zanbvpqp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vicjkkwt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cxpxajkk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mjjcnwlf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wipieqvf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pfurulnw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oesgivod.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eokuhjmd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iwezohpy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gjcxhpac.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fwouknog.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qyichtyh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mzyuczaz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fhdetmjn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ooktpztt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2asnmzhvn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ywjjuzyt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gswukdgr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xohrxyza.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2blmtahrc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pojdacqt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ciqslxab.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qidluidt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mmuaspgb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rbaoovjo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2snvvakyi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2gsmfrqqy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nzfmiqlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uadtwrfl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkvzfv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jxkokcye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spkduvlv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ztdvibau.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kzqyqmgv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hgpxestl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nwtaoavn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2epbdwfbo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hrfipqlp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2nuflzsqs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pimkzitc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vvqcwtbh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uorgqtkv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hpipsiia.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fvsnczyf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hiqfbwen.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bzyuzklo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xuiiecvi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bczrguxm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jlrypgwn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kauaazuk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dkdzodzs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pvntglro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tktrshfx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gcbxwrqb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yczxhfjh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czdesgdy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etkqzrbk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dnbihmqq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kndocxvo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzinbclo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvdrxwxb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbbqsvvz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fokktiky.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2njlwwtld.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccshovku.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2svaacioo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fesqxhpx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2btntqvtm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lfmpvebr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dtymmdtq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2izndiqsp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2fbcsomkm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kdtvdtbk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzqfxjom.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rxmhmnky.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pggmauhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtgzmpmn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2oixbnupc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxqrbptw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tnxkisyc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2atrukpye.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2evwswkfa.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cumnzyiy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dowlfujq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2otrefyju.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xhxglmxo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2iofrmqqn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jekpqfvy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vevbeuwx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lhfhnjmc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jgapbmjt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vuncnhur.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mapjrsem.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dzuvcfla.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xkoqnehh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pdndbwrh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2swnxlksf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2aqmjxyjw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2kfwejigt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jrsrirjk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aixfxquz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sbjkgqnq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dmpazjqg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jxbbzfih.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ecyglfgw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2guqweecg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ykdccoik.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sjxtacyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lyxzgnya.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rvpatqci.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2upbpirtw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cmmfvdwm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2djqhwrpz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtrmmxe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bhgrmtpx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2voxsldrq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwmhcmdt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqwwalzw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iivclztp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qiczhmyv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwunmbki.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2imqxgheq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bcwvcbfk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vqtvsokd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tuqhnwlr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vtmkhbwb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2funmdzjk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mhrfrxpp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bbqlhbnf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oxgrlwcx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pljjwctr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ewhmtzey.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dmodszqm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lagrckwx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ojsqidpf.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eckaiarv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2mldglivp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2utmrcoli.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pzpsaqsb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2psjecgln.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lmjifqne.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuqsvucg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2uegabmeb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ykpwxvsl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zfilyuul.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qlkoevcg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wsbmoexz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2svykndol.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cvliezlu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2aggtlika.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnubfdkg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gaxjnzmp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgnajaxx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oasnjhdl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iqnjhehk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdevcxch.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjadactt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hkibtbwu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2axehwnjv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fjpnlmcy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zlinvkux.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2yyrymxpx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wfjdgaau.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gchumfsu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fwcdxuup.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2godxirde.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2judknpth.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzbykqr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bsopfttk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tuoyghoa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2hyhaybrk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xadgcbpl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cdcdccsx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mslzmnim.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pnaqilis.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jubjfhec.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bizhukbe.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gpiauvvt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2rllxesnd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjnsvpxg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2seqymlfi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2sdezuevz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zyymusok.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nbexzrny.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqcjlsq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2khdfskjx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kppbkvmn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dbggmjyr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gdhezcrq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iujpbvcw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hbkdserr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ungklnud.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrgzoztv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tycwprdj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umhubzbk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2knkzsvvg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tzzviaqs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lzelhtjl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rouxiknt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ciwfhsbo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xcwptddr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lissfkbs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2efcxfgsu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2awgpzvbl.html


<!-- 参考信息 -->