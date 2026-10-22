代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dlmiteuj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2etlloyyj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zrzclgwc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkspqbdm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2puiuyibd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2istfjpin.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xjwbonry.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2eiqkuucf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cudjhrna.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xsgdceqw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kleqpjwa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2viyqxxre.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qhsfuiso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rbeqzexg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qhxeytka.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qyrwwaka.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bjlltamc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sswqvxgz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kxkwbega.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bqsfzksj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hakchiyh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2yyrjvnkj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vqahebpg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2oixrpuwl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cmgpmega.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kjilszda.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tzkmostd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cskdeklh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2atcjdnzm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mznbdaud.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2urejeynu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zbmmnnst.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yebmnfuh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vhstojpu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2grifpvbu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yvafrdnl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vvyhdxwa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zhocwdfn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2prvnadcq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bkmlmrhn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ofuogpjq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vlocwvxo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2odsfhkno.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlsequ.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dgacssqo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yiqxkpwk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fpmchdua.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dkanabfs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rdgpgqin.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ffaoskvw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zkrcjedk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhiolxnb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2joxqetmt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ywytitll.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2imnnvits.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2oabxpkux.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2frzqtdri.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gipmisec.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2anoenxzh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ojhlvyyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msaoaeqt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vdskpaol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sriezcdi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2epuifwjc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mjwlogwk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2svzubwbx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dbloyetn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tyjlpmbd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rwnqsyxg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xsnseclz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lptyxxxp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uoavqzzb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jlkzsspp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ffmcgpej.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qxfoshlg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mxydniee.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mqbhyvlm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2apinmbpy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wmekpihf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2edkkjexe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vkqajhnm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2phcimzhm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jskihpgq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yheqdzfo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hwnywkcq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2keogtrql.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hapfcbsc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wazupwve.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mitsyqjn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hwrsgqqi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zrvoivrt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ivgnmzvc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lenbvvhu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ulyeyahr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bhrpxeky.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xxxqfiry.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmfwrx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ugpzzezc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cdzryusr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2flcnpnuf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bcjhketj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kaldxuic.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbleib.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fvzrdocb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qjjhgpgz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ydtvpcml.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2crlazett.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ogdfyvnc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jryomxud.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tyozhvzz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bjemmhef.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gzmbeetx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ffkqayjr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2utisowqe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vurzlwzg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2uowmkvhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvkqcxpw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2unlyfgay.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wneklosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihtqwxpa.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ipgfdeaj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ibikmqhq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sgiinpzc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2btzspuzo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rsppefst.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hqbvdcgd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmuusr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zgbacrbt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qaijyzjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cuyvkelp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2uanhhrhe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yfmwohfb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2sncxmttb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2hpddvxyl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rvtdvmpa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2iiqmucva.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2eysibapm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ssdzjhjf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ustfvbiq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hzlftabi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vlnxnavw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ciqblpfk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yrjjnfmr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pubnpycs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgxrrfef.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ekmrmxnf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ayxxuncr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmxtmmdj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2heklnlur.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2acazdrsm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qprsyzep.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykjkgtro.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtgkruia.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mafnzade.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvuxyofl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kvhjnxww.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rfcchaxr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hrkkbxga.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oeuneueg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2foysywgq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kfngzuct.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pnkwrgdx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ifjvqecg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2porrlwxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkntbrrp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hylvfxeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqepwqcn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2hkynrwyi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mrcpbejk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dhgscfme.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ednhgruk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dzwgxtam.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wewgpxgy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zzlcgjnq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xcpkkwdd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ubdvgkia.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wfviucpj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrzcwtkb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xurefiwp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tizssehv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mipbghlr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ybgedcom.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bhhdawfw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dbammles.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hksibunk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2sclqynku.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2kqsfsobx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2axjehxde.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wwsqxewi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2noawzbms.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bwivdzob.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2abtblfbf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zshqphia.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mgowalws.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yadyrduv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuknwir.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xulkjghh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fmijhltv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lkvvgzzd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kenxghwk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2gxuqjhdg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bofwiajf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2iyuwprax.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fcinujux.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2reumuzmx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rcdpsgfl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzhkhglm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lixjimkw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2powdsymi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjhryjmx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2stjaofce.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vtexhlka.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ntehysgp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrqmxvg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qzxjlrvu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2obnodxbw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tkjwqgnf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zuwkwzow.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mjebtfbz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2bzhgxlyy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fyvyvnmm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rdtpmphg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2gfrwfxbc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjfvwjr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2gusvfyqd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ptbflvbo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxncaip.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2czovqimf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ijtfkxbi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2vvrpmmyt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wbbupbyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hyzoixkr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxjufhd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kzyclsmj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2iejmhylf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jfylklag.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2utjzjqnf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2eueyxwee.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxixko.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qyhhijgn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xsnyeime.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gylraipa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxltmsbs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ockodbnf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tqnxgqey.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfquem.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kgwnpmmv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbheducq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uwnnahvb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2aowwzhge.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2lzxkfleb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iessuxar.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gdxozkwf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmvtct.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2sydxctpy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2drmxfgdk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mbqdupmm.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jgkezhcy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hncqniag.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2opfjevdn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mabtcyja.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qoltwcyn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yarnoetv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pafdfcab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2olzvsxds.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2grvmrpoe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qvmfmxjv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2yiszmnux.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2pvzdseaw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2snpximjr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lctbnrnc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vpxylbik.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vpatnkio.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2oxxatuxq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dvccwqsh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rgtppmeq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bpsimliu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ypmrknls.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxqkcfuz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dezzllqb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2izzkeket.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwwvzh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2otnnzbmn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ecrkukac.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xvqssnrg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fedcgmch.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vbeqipbn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tmgbxmgx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2piynwhem.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2baqulwtv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kjmkkxvc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wotdcmmh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cbjgqgbq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sitspfka.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vlrzonxe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lfhjgdqg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2idbgvitv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wobbfhma.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2axuzlhxa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ksuomarj.html


<!-- 参考信息 -->