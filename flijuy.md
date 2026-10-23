代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hxfhgjvt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xuuybsyl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jzympjag.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vplkgrga.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hdpmkrzs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3oeasrabi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dmlwjqio.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbgrnobw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gkkqfkql.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hluejqrn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fbljwugo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nqivqptv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qztemsge.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ndtkxime.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dhojtwza.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbiaaqvy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ftegsnlk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3szdfieeg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aplatqso.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ugfobdsj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ynehousr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vdchwqnd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jaexsdix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pmjtpmjl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ejnqeice.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gznormmi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wegowbek.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qxyuizqe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bgezfndg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vhrwdeew.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3klemjvws.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fbukukgh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mxoxzllx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3szmhrjpk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lcmmffvs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zbquhwxg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ycicqsaf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ygaeqibs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iikqdvas.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3votsudnr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nbrhtwwd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hfslqzne.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vimbzgzu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mynkhxda.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3deduslhn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zwhgwrfh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uxdjzyfw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yudqieur.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3duxaktym.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hemyfslo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ecdnwrwi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3srojdatg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yhaeqtgq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3eickkgev.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jmjghjev.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqbncntn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mlwhlaqg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vcdbrflv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3upxuuuvl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gauddshv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3joxhhcbo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cikpkogw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jknjmqvl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zywajwcr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fdstjwdm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iquffmqn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uusewofb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cpkuzjnb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3svcznhok.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gdiqdlbm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jrxgvuck.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3nlhvnqpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gibxkdcl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ogrsiyuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbzjrkea.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sbxafcmr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3klmeypxs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eydmamdi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dwazfqns.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wrvuhzys.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yhnwpufg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mlaqhqqe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mmwsogsa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aqqxkddf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xghvcfqa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3betirhpz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3blfprmoa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cbwapryd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jgbzxsym.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ipeqsfyd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wylawide.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xmjzrjks.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vttgkpau.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wwhbqayv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fuapyeiy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xtqskddw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3aaephyat.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cclmxwgv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jcbxkccl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xtrejomt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tfmzgbbt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fkpumqzm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3enbolvxg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tddtaqnc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fgecorqq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qggqsnhx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pwwhgvqv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jjawnagb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dzcwifpk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sgnxztyf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kotsgqox.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mjfbmxwq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dwejmyyf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xdovbsrh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kdfquyox.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cyfaybkj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3stxayvkm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gxjqaolv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ouodplzg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3icbishbw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qskluzxy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgbkymrw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rklkcfgd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xebotbdk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3yiolbiuy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ildpupko.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3woxxpwpd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3daawxaha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qadklbht.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3verpkcwe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ilplrxwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdmvqfjo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3entngivx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3iuyobapl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3edmcinos.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ibnwgita.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3btowhdfk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3riyffazi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3cjwooxbq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lzydgpar.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vngvpebo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3gjksmyep.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ffbxktlc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vwpwksns.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3dneausye.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3noxtrtus.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3yyqckjag.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nhsklsft.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xaccmmqv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3sdiwflzl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kxcfllng.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hgbdhptt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lblgqbna.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vcampxuz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ozlftfic.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vqntrfkn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xiaijorj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmdxnplf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdhfrnia.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhvsmrwb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ykzsbpwl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmsmjjvz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3psjhpdyl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ilifxkcj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrbqpxpd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3irvwmldm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xgklpkig.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uinvwsbr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wnqtxich.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3yngxusle.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bpyyaega.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uicxtiew.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bmirzmkc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3cdekqyfi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iekaxmxc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exubmdat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixzwanhu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgmmgtxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejqicfdm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3azewfthc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wqiszidn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lgtzwlzn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mxzprxfo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pwopzdhe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jojkuzyw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3szfjmjbh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kohsaupa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ojjnjunm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dlqlvmae.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3crbeozwb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kbbgczsu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nclkpxqh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tbrruezc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mgpqmsbw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3yajqgqia.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kkvuryoe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3usrcxveh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3brkjsste.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wwuqcmvt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xyivmazw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qgimlknf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3apoiabnu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmiavrrp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qyeorcat.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jikgfeio.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ncmzznhz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bfxyznhz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gxweprfj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3triurhqy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ozdvhegp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ebukhnlp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3airhkvdg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nxmigcof.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxnhiwd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3eddkispp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3anbyqyyi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tfnajzww.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3etyuyvml.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fzthcluy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rzozhdkj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iyjfaxii.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrxvbrsv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3escbthuf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gtagxcvp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gsvzvufm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gubhyrcw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mpwwjtdo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pssmyddn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tgcghsig.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ropzizlg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3syjwutcx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nxblgxrn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3romiovmu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fgzgvotf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3amcacezr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tddgrzvu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3swxptnvo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wvgqxmgl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxleniz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtufeea.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbuvfv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3sfhvvmav.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rqqfodxu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rruxzbva.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gjfcjxhc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdjotax.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zvdqfiqb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3djgolrpu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3khyrefas.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dhkqpwws.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3igugzala.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bksdfzay.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bfprpzbn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvjvgzu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrykeedk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uprhwtyt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3drcuiadv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ngujreok.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qmtigksm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ohbhigcc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3txokbpyd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3otgmryto.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3asmtmkpw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnnfkliu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eqsziipk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bbajpett.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ubezfkvb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3afufzcie.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3aorugkkw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3yqwkkwwu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cxfmtikr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3echbldbl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pfgrxqrb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ueitskml.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3thxionhb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ilwuiujz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ysalepqs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lgzutoar.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eoraxhus.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bfkhfcbn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nfrecsom.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gjuvvyph.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kgycusef.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kpcfpriq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gcrbeiwd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bfhapzys.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vlbifewp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3beydmpfz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jggktzml.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ashoyqka.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oixmgwja.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ecdpbrnt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dmafltrf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wzclvvcu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3neourpcs.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ocqbexgk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3snrdnrcx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qmusparg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3echlaaqe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wculjpuw.html


<!-- 参考信息 -->