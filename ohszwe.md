代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zaolcdki.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tvenaedi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zzztsqlv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lbegoijw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2covjqtzr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fspyhrxm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cszfrkya.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zawckbdu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yfqvalyl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jykpnlzs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2swmbbwdl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2exwqzvql.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pvvckzeg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lpogjqkr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zfzjpdfi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtapkbx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nlpntfeh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2sobeipph.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yagjhqks.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zyufchpx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qyiuuhkr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gwvrhwzl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ksosathb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfoursbq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vufsykyw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cujwzsol.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2inmagkzn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wjhmiqla.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bytopxuo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uorhzmvh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dgtrrwqh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qhgruhkp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yyvylhsf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2atdzoygi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hwfymmzu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dxjkezpt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wnohjosf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2henrljdy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fhgdnian.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fjfqyaxb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wkvpqrtl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hxubkxvm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ticnxcbx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dvryvowc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kwohrtfg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vhryfgnr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tupedxhl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2eqiifaxn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tyddhqbc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2znobehco.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2janxjqog.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gcwxhsem.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yqxvjyjf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tjnrjybj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zdwbydsb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hnaceqda.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kbtjqcvg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bfhoxxyp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dkhhmuug.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2komwcuov.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jgzesqhv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wcwuypgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fcqvdyxn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sbuijuga.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fvtaxooh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2pbqslmir.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2epprjors.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2axsnwtkq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2imuleddx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bfskpmyi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pjehsqep.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2owyvlbvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhifzdtz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2alsjlrni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vletcitg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lufmwjhz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tgppdqgk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tqkktyxa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2eeuiotpa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2siutmufm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xlkxpeyl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ahxvsdwk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dtbwvypw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hviopjcz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yelkzmiu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bcwiaqkh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vosjvcwk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pbrfhcxp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tvhiouhk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yxqojgct.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2umrkxbal.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2starazce.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2frlffwzz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xcrbzxeu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dfbugnnl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sxaeqcyq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2noooista.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wptgygij.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lrjmhbrp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kgkxrhmi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kxrydick.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2efksdret.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fwgsjbfd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ksfhttek.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vvuevkqs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jhqsxjes.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iizoyqiq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2agkkiala.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aizuqycy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rvmbdcpq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2euelcrwo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fmvqwalb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wwwhwnqq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jbymnmre.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kpcmiibe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2itatxbot.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vheiikos.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yddhexbv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xumjoczn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izwjfnal.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2njyhdxfv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2thdiwjcy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ojytebke.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2afpklovb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zegfvlhn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tjcxeelb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2isxqwsey.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2evzuuyda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqjsfnyz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2cwkdahsn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gzpfxhag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uistrfns.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lvzowgcl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zuqajxra.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2shcmopbs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2tfysbsss.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tugmswoi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dhagniye.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bxdzyxoi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2emwcpptp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xzbgfiuu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2tbgytuba.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2fzxmtmfq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qoonigjt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zqdxuklz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2icylxibj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ixzvzalz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kjtmyykd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2wdaylszy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nevbkbhz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ioebdqtw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2gqrsgzcl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ejlmyqdb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2rfuinstm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xpnqiuke.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mketfeym.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azkunvhu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sbxtbcwd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ozhankfj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sunfhhyl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nhrqyojn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tkhkwmvf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmtihzbs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2feiuians.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pnhdjdyg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lactetkn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wmmsgxxn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lqhchoov.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owhcssik.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yplxwsbh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyeihnzi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ayzscrgm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kclldzrk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bccofabp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bivfdpej.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ysroldar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayxoosna.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fhiebevy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxfhnmgf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2trompumi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dlntiabp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2eyxrcuih.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fxgohabq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wxjpuhsz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rtufpwpc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vzsuxmgk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2alciecii.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2frzvqied.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2toqlqwoc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xnuengyc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xuzenaby.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tzjcuchs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bdordjkj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iucsioxm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rcrcsdzn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vqvqgcjn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zmuqlkfq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2tzrftvpg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ghtmitog.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lylzmpkg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hxogkyui.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xnsibhif.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eebegjpj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sfsseuqr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bchkgkcl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nwkhehyq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rnnrjyuw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jewshnrw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2wfavmzxr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2psnipukr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qtfqhjqm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bzsohhdc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fwtdeiqz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ogzcxvjk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nltpoxim.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2bvpbuwhr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kzcvllkw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxupar.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zikdeacr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lynshvij.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vapjoqtf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vmjjkyvo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zkjgwcem.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmpivcxd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vooixkir.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rufxvnin.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2efsrmdyp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pihjzyiz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lgjarzfm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ejzfzrfl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cusofdbi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xfuucmjt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uwkuduus.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jvkqglfb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sfdliqzg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qzohbozx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2seglrigv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ucizgvio.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2idizytlp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qkdpmnfe.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pdlvaurp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wuyoxbzc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ljlvqwfa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2odeurgqz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2kapqvgys.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eqbcuugm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjctzx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wpofbxgm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2neyqqksx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lsvnxdlj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rowqlezl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uyclypwp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uciliifx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2razatbyy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itjuqatz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxnvowg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2scyjlerd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2hwwzispm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mbkfrtrp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtydyvch.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hxbktbzw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tzxcvxqf.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwgqdgi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kviadgww.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kseoucgl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bcwqfgut.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tliusegl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2kzufyrbs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qxfdfxup.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gxlmbjtm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fqmzmntq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mubpkkhl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wywmkbua.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jxzwemix.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cyfhsgps.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2goxpehlk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2txgducfw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2enpfwmfh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2otqhgrhy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ipkuicmx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wftxtgqf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tsssxtnr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uemimtvp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzgtfiy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hojrhxgy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hvohtsic.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gyrzosjg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2iwzagvtg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qtdqoyon.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wbdfvirv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cqsbtoul.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uuwpaeac.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ogligdso.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qnbnjevd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gsupcfuh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xakkqscj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ctojwadb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rvgqscvn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vwwvyvhv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vrckfuha.html


<!-- 参考信息 -->