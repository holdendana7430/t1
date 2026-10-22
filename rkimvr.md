代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qfflgbbi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pcwmrwdm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2byemblda.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fnnzaycy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qipwxiew.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2exqmntkf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mhaimctt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cszsvbmb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hagcnidp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nsupzbyj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ykiflsps.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nlzklcus.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yqcdmobs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bsoamlgz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lxqwczcv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nbibequx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2srblllgn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dkngpyrx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sjbcqwls.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sfreidjs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lnzdvcjf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wetqorxd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nnstcwxj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wileurbf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mlfwtcpv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nhxadxgp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lqrqswgr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dhkfmerf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yluyekwk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gyiynhnn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xcnjvjsn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pdveqldb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2retldoov.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2oegtznjs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jakyhung.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jksiyqyr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kvriygub.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fpuiclrs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ynppkbfo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nmlrqurp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vamjszpu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmdugnp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kaslayjp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ighrufdu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gfhxitqq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ttzneczl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2eaeapwxc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kkksnirn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2klqevxfx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jdupslzl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2isxeeiyb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rmpbiegn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2imsvouki.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grjuvpaq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bgsfsbjv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pucwbfwm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kaetgdgy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sdyzmfwi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hcepocli.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umyqpceo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tscwanon.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2clwojqyl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ldejkjfk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nxfpxrkn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qsrpvyiy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2avhuiimx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jxpoxwoo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ruyghqno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcuwocxu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wzjswegt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dszbzcil.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xtlbqide.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dxxyznbb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sdnhycdy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rqduwltt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mvhagifz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tszhllmv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqzxmdoc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uxertgey.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hwgikdgl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vfucntse.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hbwcakax.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zhdducbc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wsfzofvx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kcbofmrv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rchxbyhm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rtgbdbwa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tgkxsrsl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mgfmrmwp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2whdqiguh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uajkvuht.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2atrxzahf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2htnfzoxz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2orszbygk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ncbgnmfe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hzpntcdi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rloyedzh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hswlpelc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ujcccfxu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kcvszyfz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kfycnyjb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hukymtav.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2clicgkql.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yalvjjyw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gwpnevyg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yijtxmfs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2kdfchnkt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wwlqgwuj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tlrnaeii.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qtnnkdgd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xlxvjnof.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2etqobprw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qvbrrcig.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2slfswmho.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fysoxtsr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mvfgfaaq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2omgzijxp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xmakiodj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eriiiivt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lwbddgir.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2izvoivmi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ghukonhd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dojmsooc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2krgkuwci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgyzqsla.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ndubddzf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2eqphbeyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkdvnigt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cqpbqzjp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2stiheifl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cjdlryar.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2junuknqb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2muwfyjgs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bjnevwyu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2phhhunlp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jntrsgtr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vftbsgtj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eeuwqunb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vcjcwcje.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rzhnnvzv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ffwutxjs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mmriexny.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2shykcnra.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2zpylpese.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vghornsu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2iqsuuqmn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2gyagctok.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dpsxjffq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhuaesom.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fuvoxscr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2djdcfmjj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rljxkcon.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixplrlhf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kkrlloyy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qeskiuls.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2juuyfang.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2psbfkqel.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkdyvrnu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2duapjqbr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvknefan.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dsjtgkyz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nwfgzddp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpogxlxf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqydjewr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdyehh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcwslz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lbzoffvj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2knjxlgks.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qguzvfab.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ybksjmik.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2klfskzgi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fuoevmlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxsjzzcf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2calghbze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqbxetqm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oypsoxes.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gmdlmyfs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2smxyoaio.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xfsptmga.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dtpdxlhr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zubpoqfe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2otgpvcyv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2upkqsyro.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2musviege.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yktnqvjy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xrotqeaz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2npnkkmwi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oljmtbcj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zzhqsitp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nkqvmklx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qyxlorse.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2tvuwnfqe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2apuakvtn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2klktyxee.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dtqarjxg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wwumhocp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qtqgchxt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ejquxpew.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bgeexlqv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nbuaficy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fgxhhuli.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kudbnmwx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ouqdqpmj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pegfpuxq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifiriqqg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uxtfhrhs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aodpzmon.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2piravoev.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2inthghcq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bceqxysl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2gihtbjyo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dfhkjsqm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mquqsilg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2duarcvsr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zbhffcvh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qtvunpye.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hnnghhxu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cugrfoki.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rstcvffd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fvwjccmc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qlwgprhp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eejvsfus.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dhccxoly.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2smchuzeo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tpuwoosv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iyetxrsj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xbpijiei.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rhsjynqt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kmejgbrf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ruowjjug.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfswiao.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2iitkqkth.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iagzyjbk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kxpcusyk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fjevlpss.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2mvqwaykk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zgzikgua.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2klvoywgk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2yeatkvdz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fczgvpbv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfrterk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qkahetsj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ataqqjbu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tzifqzxv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cseawdax.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2kfthuegq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2prxyoeez.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pzsddcsc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mtrwxlwm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gowhnpab.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcryqdgm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bpbnkqty.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lujzmpav.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2weaoevkz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2oqdnmmpu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okashaki.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gnnihqwf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsgjmix.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rlfhdlrn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkbmztoq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmqofxyi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2audtuwni.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nhcdlysk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqdpege.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mbfjmqeq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wplnirjq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bciaxjss.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ljtbhqmx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvixjhiw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2okqaomqg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rgoqfqtg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2uakmanbd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kpgpaypr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2psscrtuz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ofgnnavf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ihaomhhf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hybdcvcn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xxaftmkv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vbmtnkut.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2stccwbas.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2txpicukc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uxceqitf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2aigoingo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ygoefkjd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wbzkxzyi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2haeyjolo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dvsjlklv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2plajnqfi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nqunhpkk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hinufqat.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2suokdbnl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gktgpfpj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kuzevtkf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jtpwinzd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hrsvguyp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ylxxxxdi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gvhsjjyu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ivlktxtk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wtzffndy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2asobqpci.html


<!-- 参考信息 -->