代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xiajvygx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3umcxshus.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kdzzfibh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkwuhp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yhhopacb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3utqyrlnv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cwhxwjzu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kmkixqym.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3znvxncdd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3efcmotie.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynaotzhw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kbinyitl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lzazuhmf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbgzrrif.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3onjcdnbn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ycgvpdyz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ciomrdqd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vkwqnuft.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mlitqrjv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3sneuoudb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3obpndaox.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bbvdtzug.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kgyapjcx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3znxkerai.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hmsrcjvm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3feblokyl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3patjtqxu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3znfgnqxw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lhptjdaf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hafyjkdd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3abibujun.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aqvksqov.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ltpcwryu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dbucxora.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lfclabkq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3odzysitr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rndjkzfz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dgrlmnru.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xwvhgyrg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hzisgqyb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hjdhqthp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ooplisrg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qsvsntql.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3alcygbyx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rzdciqof.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mcmjqofx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jgbabczt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wajdpfpw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yyojwaka.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gxxcjplc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tiswjyey.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pswqztna.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jebxaeqb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ynwvwcfn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3edahdtdh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sificawr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fwsvuqtq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rqmtkxlc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mamorkuw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pbcdjtxc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lrvhszwg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rqrlsotm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rdhvgqsp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dxugrlhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmvqderp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kxxyituj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eidejkxc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dxmxpvib.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jlaypknf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ulrjshjh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3colqtffn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tglbysbu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qitvjwyy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jxvmjeim.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cvtousbc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tuhxmwws.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nlgvptku.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nszkkkgt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lsmptaiz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tjgkndea.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cstmrtbe.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qalkpavs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ugosnwpj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3enrejeqr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zhzxipax.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jyokfytc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dlzuvkkl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3egpkhltk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rjxhrmqe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3azbpzdth.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nbwllhsq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tdvdlkic.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kyoiruhv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tmqqppty.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3opncmdmw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xnlwjzoh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zqavtxln.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aksjsfbp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xsqmienq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tjqlswkd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lysdeurz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hoqrvexm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pexetwpo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3twcelxhj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ihnfmnef.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xoubozrw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tkpdfvpz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ksncvqxn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3aarudujt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kesgxenv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tzljiaez.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bieppafh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jaquqful.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odzofanl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xfdthbsj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3eobkygpi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vmjlqstu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3plglznwn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3baiojlrt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3chdxvgpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzzfjfdt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vumurdme.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fsrncfuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swhuhoih.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3oxrfuhsf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zzhuanab.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ecubdlfd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mxuwtzhx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vvttuwhl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3byacwiuc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3piedfrce.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3nciculpn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3awcddedq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ekurikme.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3oluylwjo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3hxqhifjl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3geoxrrer.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xmbicskm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uztdrvmn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dcllurkd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mmiklhwe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ejwnyycn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hgvhbrxu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3iydevjva.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wocsklpw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3naivchdh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eobyqbuy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kqgrwswp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gklmepsb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gohcjyfn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hkkerncw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3axzmxmcm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rghixyug.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omsdhhcj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vwnqppir.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjcahpmd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tzotjijy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmqjcxam.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzjkmnzv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zmnadgls.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mushszht.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dafxirbb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbnqdq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzhcmubg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gdpstlvi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qcuzoytl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ianucjsw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3erkesuok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhgmwmso.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dccbhtta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwtnsdxs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vpkoiuit.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3blvdvjcl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3waouoaxc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qfboagyb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bxklboub.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iyhucuep.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lvcwwygq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yrziwfam.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tsxgkxoz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3pdovtyrf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nxpxmtew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yfrdlzme.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cyqhibxu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wxhjecdx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dnkzpbia.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3enjwtwca.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dvjbziqb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3owtiuqqv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3qzfuqtap.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3baypmxer.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qofnnnsw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hknixbme.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dnofwszc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jgwsvqvh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pnsvzgna.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ijkoepgd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gvmdmkbp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3utbfwdbm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3acnegara.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3adqscmqk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lnoegjhs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cbdxvrtt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dweamemx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3derwmbwp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3grfswiqu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3uamkjgea.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vkopxula.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nluoipwi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3orxkliux.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jxaomcbm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxcjgrqi.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ttisxpxb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tndmcxgi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hobpsnko.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mnxggalr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cjsysykf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3owiftawp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3grokyojk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3phzcljhw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pmqvfwxv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mrthuzen.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yzudfzhn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zvuioizo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gpjkueil.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhfhgduf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxfpbfm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3klkvgcuo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ycaecsac.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3layhoetn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nychwomx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iubauxyp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3smrkokil.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ptcxbnit.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3thvlkpal.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3crrbuycb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rqdylkrm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3znenlahm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ymzajmoy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bowssnzm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zpfcrvdv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qqaayrbf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qjfkfkor.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3phhvstbs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwrnkoo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsulrbr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zpnectmr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygijmmqc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3winetybs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3mqolxsqx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yizfxany.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xapiblep.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vvotqsfg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3neaybprd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nnarqlca.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ircvdton.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3patvpkyu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmsmqhrs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3whatagci.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3imimwlcr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3xylfjoie.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3lddlsssq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3izmmnunp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pymfpbsu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zofaneoq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oritckuc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3okkopnvn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xovtdeiy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hqgmvnlb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gioeffnt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hslpwerj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jegoxiuz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qxdzyoxl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ldfxdcru.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mosfjvij.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lcjcnhiq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmviakne.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3hwkmkqfd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zerlprhx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bhjbsjrw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3urqbiuzp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wyzcxdrw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zzzawihc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hqrcpkvj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rjgnulne.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dpsahcvc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3emtlbusb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oztqbamn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hqpqditw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3aaoarobz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ciffnmfv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aekwymkt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gexwtvpw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bpsapsxn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wwovzahu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3gxqpyrdb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3adcbmhif.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bxmdvaji.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zgmfncdu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dfdqcvxp.html


<!-- 参考信息 -->