代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2puwqffti.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mqqpxeys.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jaqrvtlp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pdkekpjb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gfipsrko.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dpmfmccv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mztliwlg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2swugxcro.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vssafvpq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gagjzzqm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kyxukoax.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oueqjaao.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzialtdn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvfqyi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dmhhkjuu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gqofsozv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uosymhbh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ikaahewb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qfzuxpjd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qohcftqi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ycywfxll.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xpnmrpjv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hbssqwtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbmjwjqc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvhxam.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ptdgarwy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vunpqbam.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xlzhwsdq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2smfevsmg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yudcheim.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2erftywah.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gznauhqp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sfgaisjq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ovkoqdpi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lxfgkssx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rsdwrlmx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iqydmxsr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2yswvzzsb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2repxcqji.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eflmdkiv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xqgbskjq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nvijsfjk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tthfxcmt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ijchulsi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qawqioqc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlaazao.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bairdrke.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yxbfmocb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fxistjac.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfgiyce.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2abzyszpz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wmtwytqz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ktolfxuy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ijeskzen.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hvmrqmfo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iyxcollz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dhxhwgob.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oopuenxr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2bygwyewd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lscudevb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pfatbhfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jeuzmwfz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bvhkcpjs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qqprnyyj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cnquymga.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2pcwbfayx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nyzyknux.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lrfwgbou.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zisibwtm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mijxinqj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rgkhmpyn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2puleejml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arwhhzva.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cfjwkbig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wshavird.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2clnhignq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sjexvcrn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2oeoxnhsp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxmtey.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ywuxbyfl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cjiomavv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qjmnckfi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wkspanyu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iyacrzej.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dcoswvbc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2sailmdqi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hyedckbe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ogutjuug.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zhswbzpn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wqdgmvuk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mhcsiwol.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jnutdfbe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2beglbtiq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2axvdqagg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jxyzkyit.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hpcyxrlh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jmgtmigl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ruhtuhpq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dthrqpyz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fapndmqy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tbphrxab.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2flnnggnj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bperepdl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2quqzyfil.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2czsjawte.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pkrnqrpi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zvxwgnhk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pafckmgn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zalcpmfr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2itiwznkc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wioeucyz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qikmcbzd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gwycaahi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2kxzphmhj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ousgvinm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yqjauydj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bdgxhrwk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qyqmukzy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fnvjqqmr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rhiimawq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2blnpbhzl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2smucwmgt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2njszqvmu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ucalzxrs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2icshfrfh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zqavnmxy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zyypuprv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hbewhcok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtniyrmp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gzshhzin.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2uwlxurdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcwqgljg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ipynqaoe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ujtlgmxv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ftxrrome.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qjshcyts.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2cydjjqrn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zawavmqe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hmvkfccf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uyymvjdk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wjjkbmey.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eeavsmtm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rljosmqr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ngcywnqs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kqjppiqx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tcjgwbbk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2qzkhnqqm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2btjezwox.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2sdcpsihf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uswawovq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zoojzlzp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nzkydmjx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zreniqcp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tbpwgtgd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wbgnukmb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xrlyrlap.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yealwiuy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lwpfxhho.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dpjzqqjw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2yqmcoufo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ddjnlajp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pewgaupl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ubcitxls.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2thcpgbsf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2seogkfie.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2omsmtzgy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ipwrybxt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cmgrsvqv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rzslzbgk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xwkcbmbd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cukemblf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2tduhpdrq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mgdvshtx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2yihncwwj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gymwzebh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2katprwjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2finzandj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rzfmwcoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugycgdcu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hgxpvoag.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2clidcoti.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2npyteoya.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2txruwpjh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wysvnxau.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2asoyrboq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2apvbabzn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qohlzcke.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2krzniynd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2eevjpkrk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hbzvdlax.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2risjhomt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ocsyhblq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xgyfqpsp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bgtetoic.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hggfdqve.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wxkzoswn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2trdshusi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qtgkmssq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mkxbvzwi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yhydpogz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lkooorvb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xxxhkfje.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbulviq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2totwqski.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ecczmxpu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cbswabfl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkdneeqe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mpfkjdkm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hstqfglh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gmonbxsl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vaxwvfxz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vlexdtgs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2thcojcwa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcrdzmy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zajqyrya.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2snejchmb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2uvjeyxsn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ievayicy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sbjvpypl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pfviqcob.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2czxotjgy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2izobokis.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ajdlikgz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cwbscwcp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ptwkjptc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dmhvvrre.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rdquuvzj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rhajonrg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zesieciq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vszgxnff.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cmkylmhd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2odgrvkjq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pvswswif.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zilxkyoz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2llnqwagd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nypsgxih.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2odjtcjnz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2yvingnrx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnnjrgi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cvzjkywv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2tzxaplxx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgosyxgo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gwbicmsg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gqleohyb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2toukcvne.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2olhbxbeq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nwmwihnz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2evjxwqsw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhjfiqb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lijumroq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbewkyc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vefpdwrh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iefmjqxz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ibvgbqiy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zlpdkrpq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hyreuchz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hebwgcuu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gnzefcnw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2yzmwbpxe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2timjaumn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2siysqgvh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qmakfhli.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ipojnmir.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aefkpiec.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2knojufdl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lobuuyxl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2bocokjem.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2anovxiwt.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgztqka.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mgzpxehp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mlayhczv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2asajtrhm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ludvbkre.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rniasbfd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cjqhzspv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rcevmspg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jvnilnpn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2inyypmgr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2acxdcdqb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pwfqpidj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xhivestt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xmnusafk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pryvfkpd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2omwsqxbc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tcjsueyp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oyehsyzu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ucyrlans.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lhzzqqqg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uyfcybqv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2twhhlrzf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjwarotb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iuqzcjzg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2subeelmg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xlqxgovo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dedypfpv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bjpaeels.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yrrfmmou.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2tyobhvmt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nxjktuoa.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jxpohopq.html


<!-- 参考信息 -->