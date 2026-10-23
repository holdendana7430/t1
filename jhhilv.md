代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3trziiqeb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vizvwupz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gpnawgny.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbrldkiv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rydgyeyv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3oojsaesn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bupgmisu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xbmzyxid.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lmxctcxx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wctlmmiq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fuuntyiy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cbdgcron.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3sduvfnwc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwtwfjoq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3icesvyir.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uenxegqw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3frnjsafh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3oeluybjf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3oxdhjrav.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3udppsxhz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sjpxccos.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hhsaysjq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pbnrihvi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mqnnbrka.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fhzkldcq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jyiqxicg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lqmqhluc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wlwrcoxi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ahsgojwg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tzisskto.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fxlnyght.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bruetgwm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kmdjmges.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mmikijqy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nikcbqyq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mxftzbaj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rdsbwmux.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tbqsxzsd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3exyjispq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3owduhmpt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3myvhjzes.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3aiantnmr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nijqjusg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aeaeeuay.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mvkjmbos.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ycktmdbk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tpctxlhf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ekwwopqz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3enioabvo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vvswxpur.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3libeasfh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oyfhdzvw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3csnxhzly.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3owlzrjuq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jncgrxyu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qkolmxmg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fuzmsmjy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3naqpwgqf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cvymspsh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nwlxcozy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hopbivuq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gshwwyuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xehcpqlx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mdpaetom.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mtlmathz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xlhrkefr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3prcqwztj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yksihclk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hhwaetsa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qtsazgjl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rrvobigt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ocityenw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ibtkumfd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwyvis.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3chprldmo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zeqkobvi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3emjaxhkt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cowtyagq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nhibemgu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lqwbrjrq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rkhhuomj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gbkgmeqb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hlrrujig.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qvxxgwae.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ufqgzkcn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wrvgrqre.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mgqygqsy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cdniavhu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xdvqmqah.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ycjrpqws.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ugnjasdv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cmtgwyzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qmxdvtcq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rxyooxgu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yfmfmarf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vodstfjl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xvqwedwo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3skdgrjdc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vchnzxzp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lvcxntpj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dipxcjvm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ugvudgcc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ugthpszc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wfzhdmwz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zsxvdwyu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cqgtqymg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3qsyjzzby.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3egsslgcs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3eztnvopb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jjodxptu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dntnexqw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lbjkcbyh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cixkpwom.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pmizoybw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ejiybclu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pomlzzjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkfsoqsh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3rtwxgfes.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lqqabdzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwalmmyx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3petdskzw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ssexrgbp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qlnnsllo.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hqbksqbr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tgiiwqbn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3kqrcfjvt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pwnuiqxj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mpwipbpx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ergiifup.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3xhhiqcvb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ccyamhig.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kirlzftu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ulstriqr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bmqmigpi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3symcfonc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ndxgnqng.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3krqorbec.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kovwzgni.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dkzbgnds.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3sqxugdbz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mancsfre.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yzqzvuap.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lfipbkuz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfshzz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bwlzlset.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jjykjcbw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ejujhrlw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ndenzfqy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plqhothi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tqiqrzrr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dbfesfru.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fdmmblxs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rlhmngmw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjrzytga.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3afkyixpj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olgtyztm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kbbhwyus.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnebicvq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nardrlmy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gslkykqv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jplrvbmc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwjmeunt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3knovkvhi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vnkclvik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3proeaqee.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmpoafku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjykym.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3giogzgxh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqxtfgs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3dvmpehmi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wrmxhsqx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ulrfldcy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vonxkumx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zphzbvgz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mzjwpdbi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3upyrcghd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3opxwkimm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3agpzmebg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrhirs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hxlhffsk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ixclicex.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sludymlm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3frffbwcv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qositmst.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bsuxeeyz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3alzdezxg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tmscnhcu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rbcgcwiu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3npjpckpi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mjhcvzmc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3spbaphms.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ascjaymh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3otcuvqqb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hrwiqpif.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmblvwvz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3atxdzkri.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nygwwsap.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tblbvmiw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tehimvfz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3fwkhmzav.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ngdcoxmz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbpnxhw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3eylozhju.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3evinpiyw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3oyprhpwd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dqmxxidn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ttawabiq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eqmduejw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mvzsvkyk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxhdcvrc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqpgnmkp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wghqjetf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pkgdawir.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ofkdkpmo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cibcesld.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mjsgtpdm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hcdfgoug.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cjysmwjw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsatysb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ybremphn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ahmxkmdi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qryezgqs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dqxpehur.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xghipweo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3gnfwzdza.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3arwysezn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ifvhyrcw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vnyopwyi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3uemomuvy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hefiaevq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3kaxlogrb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cgelddto.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3iyzjqzyp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3etiiudlk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3dfzrxvcb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nkfycaiq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iiqxkupp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mylbtzdl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3phmzxfyd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mrgjyhue.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3adnebkag.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcononsw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uaexrmql.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxcjzsps.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lepgrruh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3dwyagoax.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xfrthyyc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxykgvxw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3femupnxi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tcawmxxa.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3hraewbfw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cjhzjgyx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jwcnoaes.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jhbldjyj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3svoxread.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nolisfwh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gldlprfu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tvxwetkr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3arrjnipa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dajollat.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rsuzoesz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zrcttabu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3svegryht.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3sbdkhwuc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ihalinrz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qgwwqdzy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nognwyah.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3geelwpnb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bxhmhnzs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3aqylsdvq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dhaedjfb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3irkpblfv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nhrqshpd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3eujgsovs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gvewfaio.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zkcsvufs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pcbhdchj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vkfwdxxp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3azviicip.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aughbipf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3afererql.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oqinnnrz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ifwvgkil.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ltaharls.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gfyqfpwh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bkkwvmfd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jckdbcdk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jyfkuzzw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bmavwskn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xybrgvfu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yvgcukis.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ruzembdb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sxpdlpmg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mphpeoxf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hptqwcca.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xkzqpdwc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fsduirxy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hykqarns.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bkdjdcjo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3graqdyal.html


<!-- 参考信息 -->