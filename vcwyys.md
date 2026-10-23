代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oztvtilv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3emqrgfbt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3chwkfehu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qgrdfxbn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nvrvvblw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kwdkrlfp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3syfhaypm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cnwghvkc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gdrlmxgn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rqejwxsu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ypfotswb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvnditnh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3epclmigq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qahoicdr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aywnoywa.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3faialnrc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qfeducxs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ylxxdwbf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pfxnpihq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rvnikddt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ifsbludd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bbmnaxsf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xvzyvzkl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ycypwbmf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uzbpqcro.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfblpeih.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nhbpwpab.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ivhrofyz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3doggpmlr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sbikgubm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fjlazjfr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tyqkdytx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dbjjrynt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wmjtjdjn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wdmodldi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qrbfydww.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qzwxqapo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wqzylwck.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eqplluzr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3myxoerxe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kceqpewq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nuknyujw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3htqwllhv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xvaodbro.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wysegzlf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lcvqkhpi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jqgdnque.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hlrclgwo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vrvkfsgg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pnqmtjpm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qjhfzglp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gaxykceu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnwlyq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qgctidmg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3guoyjdyo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3flfyglex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcqfzwtg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3snllqpyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xubevzqw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jtwqqlpg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xlzjsdrj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3clyysuzq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yvwftlgs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zbdvnsop.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zlbuthhs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cuaxrtvt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jkwkvwon.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hgxowpdt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3etomnmeu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wedzifcy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3awwljezl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lvupbvwd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iklatiij.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yzddtkfa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fdrftstj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3anyodgwf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gaorvfxs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3avpsjtjc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gpuwggdt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ureqxmvj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zreytexj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rgazjyih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mfqplsov.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ketmegnr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zrokdvqo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3occtxgkm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mwwkfeow.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zpdvrpxd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bhxzptih.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vgxcrxku.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lbluboee.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wkpscwxf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aezaixvp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rcgvhepk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3giscyxoe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hpjefviw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3avegopyp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ugdtviba.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xzsukpkq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dsyronxw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lrxmqdtm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wgkyvjrv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kewstyxe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gwgmkqia.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wiviakko.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lglaimya.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qnpelugg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jkccskfk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3phitzkvm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qpejubgd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3saxcrduq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3iwqeqvqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwcnknrr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dbgasimb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zfiukcvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdfzpvos.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3expimwlm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bhvtrjew.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zxrkwklx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dlbbuxio.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3dusczmai.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gpmwdahm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vejounku.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nqwquyms.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gzyhuzly.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ywoxchrf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3esyekgxc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3nzplbqcx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vpyslseo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3epnytfmi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vwpidpfv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3tdhrzkhv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rqshylyp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3twsojudr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hiyvnfge.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qfzhaisj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gsywtquy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3srgigylc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3savzyoiw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oxcauyph.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apfykrhh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwlnhogh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iitnqdqh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mytrubms.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hatiemiz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3golntjzq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yngbljcw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwlzxdqp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dzuonfdo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnpryqjd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drorvtrw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqnncciu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hqzolzzk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uowphdor.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjzqud.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hntwkjxo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhyzndmw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rawpwngd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tramytzl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdfyttcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmjzmazg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3nnjsnyws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aytzomvz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbrcvpjm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rvszkgra.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lgjyatqp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jqajkgmx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3xwdecgqy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jnydkvkp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xpaigmeu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hvcvrjwd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rglkthym.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bevfgnsc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xiaizhxh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xikmjpsc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ggpoytru.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mzpwpmwf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yfkuhmcj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3qgntbxop.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xeuhwqiw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3roliyvyq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3leflexau.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3pltqbnxo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3awemasre.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlpphdb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wtkjsorn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3inesxoil.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mihwseet.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sdotxbed.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hvjxxqrr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eeydnsui.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ftweoxow.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmymajeo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hjkirgib.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3obijedyd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3kvhwnsxc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqkmhc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ujoikgkj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xsxwhifu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3irazibdu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3epydjuti.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qkgiispt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oyimktny.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3urxngnnc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uuliwvns.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lqfygqxl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aamzrwce.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mipwtbly.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pbhekylz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qowbgqwq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kfouqnds.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3txlybnju.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pdmmeolo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ppkwmytt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ajazcczv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3lqtnjpln.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ygnlfcan.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmelezap.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ocwjjmeq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3exwirmeq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fjoqatzf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3panhdzgp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mdpeivbi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wrweeovw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qgqsimyx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xagsismr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3whtcoxsy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkxwlyk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpbdxhnr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3swwrdlgv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bksonold.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdbeuci.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bxjtfnme.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3rxtuundl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uzsbsauy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gvlvxbfl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xuyjgtwu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fljvxvhi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kicxfayc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emmyqxor.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3amxmdfch.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ivajaxbi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pqlhybwx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3duewsrdm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mfusmaqw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rejdkacl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yhnlihia.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rthlzhfe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3emlmwwpj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayedargi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mtvjqqhb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbsikkn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dvukhpnc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3voqadtsn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vedqjptd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ggotzjor.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wrfswnct.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3avcvvzll.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kuzdiliz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jfofcmqt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ohrceoyx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tqxnzhkm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3feassmwl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pocwcsni.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dxtmtajm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3npdevegw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mocttsxq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yrfibpii.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oroxiyvr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qkispfpo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3majyggik.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rnotncpu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dzofkrms.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ttvwgebt.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lazdvcob.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wgpjhyrc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ohjwjriz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vcaawuqi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ngxghesd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hpxcykjo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kkatwuee.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3joqpfhjo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vdncaxbu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xwvfloul.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hkfunpcl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wzbvmgzm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mvfpztjk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qemtrjxw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3urzsvfmy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3inpsulvh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3syksagdj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zwkyuotv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ybdeymut.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vycdyzkg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fceuidag.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3imwvtujx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3adrexdjb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqvbta.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wstmiura.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hpgxmsdj.html


<!-- 参考信息 -->