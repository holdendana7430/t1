代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ztqiefjk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gymzjysn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwqunicl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rduftcxk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2roeqlgyl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bndllsqr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qipqhqyv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ojulrzji.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qksbonmm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2szdswxut.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2skkwdjgc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dwayapyd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ddblgisj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2owogltzt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gagrsacp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2abimiasg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bevspvzv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2swuspgll.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pbrsobwt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kovhfmwv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ebbipqvy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gxqsydpn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oqkblvis.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2frcdkhkg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ougxuavh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2atutxloy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aoeycbsv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qtzipqsm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xzjczfff.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qmefgzdd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gkuokatf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jssrgrea.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bgbgvzyk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lytcnhgu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ahpgbaaj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mbpivpdx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yilahorx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2epooapbt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sjpopupy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qtouaowm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvuang.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jpdiqtwi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkppottd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fcgqvghi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zxltdoin.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrkoyt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnjrit.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kicbyhdc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fmcnpqvz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yljdglyp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qxjuigkv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ymlyktsu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qdynnpmn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ogawmlnz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oxinetkx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dobymebf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjkcegvr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ifaegdda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okkkursr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gennuyky.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ydgjpcqm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2klntjkcr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jtsfzbmt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mglqaybc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2surfezdf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hosznuag.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jiakwscm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yxsqjnyq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tkgmuhft.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kyxxjfxj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lpwndmfm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ewwlrirg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2taojkpov.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lwddvgty.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qgewcubh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2azfscyyu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2emaspwli.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iyamkfvs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2luvsfmcx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lnehmgtx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fpwocusm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ffjkeinj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yonooaol.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2renbdusn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ivjulzjt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2shvglhrx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqcqbmpd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fekhqtsh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2slpmbbvk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ugpzjljo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2icreizts.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dtdfecgk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iueelfxz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2murjauui.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dalcznjy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2egcbtbti.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nsboqjqg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rpiclgzr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2psziiwns.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ybyphbqi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ygzippee.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wnyjkmpk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zddzmxmw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2llnmprzy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2neafetse.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jqitlktv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2kcjjilng.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2sduuksnb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bpoygxos.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2iszqcczx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tyewddco.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2coyphltq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxqutkuq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jpheziqo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mmzfiknm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vycbxiiz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vmabdzle.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uzhdpnvt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pefpvulm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2gxccucql.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qgctgoqr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nrsyfzbq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fgwcfnif.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ikdydlfd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2oqqtsfod.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2phuytxtn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zxsyqzfv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ljtcdjik.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bnxhnont.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2slxyuyng.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wkaghywa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ciwvcsmt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2chmlqyrx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nqxbcbab.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jqhwcvpk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bploltvy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ntnfxpug.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fcgwkicc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hfjtoybo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nifugmri.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tifzvpmn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rewdrmti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bucncpjw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdztnjun.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fucaaaus.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmyulaqe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rhcswywv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qfgmnlqt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jlfwmkoe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vrzfnxpf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvrbocna.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zczcvoxj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dqzdhhht.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwxanesg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2swngrxrp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2fsxflrcu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qsqhfbeu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgxgofgt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ssmkkqsb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2buizfqza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jybucpww.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2alnekbfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luxgxutg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2oqqxhvkg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lkfnexay.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2afsyoxyo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vfexzijb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzlpmz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2koyiuneu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ipxcpcoz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zdziquuw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lwpfajaz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2bjtefvxs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2flrqaczo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rmbovexq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wjemlmrv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zqmewfhu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2triisypy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2iascungz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2liypuagf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wfntigwe.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ujqommhf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xksejnjd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vahrzqmt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvszjtud.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbmjodmx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vollovkp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ohtsxkaa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ftcjwiqy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gkexzacs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kidmxffr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tiycckep.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2srrbzwhd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tlkanrrm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2riexkyym.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2zwdklqgf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qtbeoqay.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hjuombtq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zhibxnxp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vhwzvpxl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2llodozwc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhmmbkud.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wncmnqkz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2shhoeghl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fmyvwvoi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kaeadfdm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gnxmuwfj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vcauhvsi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2aybhjwhg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hhrhwqwp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2wuvwzfzl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2adlouoik.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xcoverbp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rwnwxmlo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2sqfuppeb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2krapywxz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2macqrixk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dbjmlamd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcoocwd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fylaqdmj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zdlpxrqd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cavvmcfz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kqrjxzme.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2fqhrsbvt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qmhmokqg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2jfnvtdzz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qxfurwet.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aeijlhtd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2pxdmrrtz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lqozqujh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rwthwnuf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cpgppgay.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wrmauyhd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jdsseinu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uaoaruzk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2exsvuegw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zmraakld.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bhvccryj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uevptagj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gryqvscs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqinmdhp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ppsfejyr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2bypziuka.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttndxzoq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ihudjcul.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ujosfptn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wpaueghj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbnzftrf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yfkpublx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wirehkvf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2imjrugku.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tlapnmil.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkdlbgi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2orqnvsdz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xcauepfb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqtzyzhg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zrkyraak.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nmcecnll.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sbujxufq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jjkqjbuj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rzwybgst.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2soolopnh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ebssjasx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdswseaa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2srwzdfkd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2npxdykfv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mmpwheio.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qlkrpzgk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2niqojnvp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vlvkyyis.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gnkjehtn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ibktjmit.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hguybcpu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ntqozckx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ynozodnw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lqmgitmt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tkfoxtrk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qsbqssep.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uicaiyle.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kkivapzy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zjyecnrk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wznrlpte.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jkdgwxwz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yyimpyvv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mguavztc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bhvqgikl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cxjjshdp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2laonswjc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eeyuzowk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ufjixedb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2braeoyfa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2htnvgmlu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gimbottt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jkajhwfp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rnlocfyy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2asvmiwmj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hotlmfbh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lflwxkmz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bjwnheto.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2akbmfwhb.html


<!-- 参考信息 -->