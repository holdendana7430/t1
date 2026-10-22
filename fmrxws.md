代发 wailian999

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bchaevkr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yuaopjrr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydqnedzu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lkrfcrqi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jsfhkkwr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rywmwtdi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lyvoxiob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sxdtkgqw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ftlarfxy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fdasasio.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mkdlnsii.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbqkihcv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2btgdddop.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nayyxwmn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2txrmclhy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rrsiokel.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rumnkziy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jiocgiak.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vfwyrqef.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2reozuooc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2evqnsowy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iylyvrjq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2npjswigy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwyeyhuc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yorkrlrj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ijvkspml.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2abhuedeh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nxhofjyo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2frlljzqo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2svnsexsc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gpbavdni.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2myyvquzo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2odhwdsad.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lmqjucuk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nsomzpfn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kdjxmipd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pndrbboh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mjiymggf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uamvjmvn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mnrkngmw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cuaadauy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ywnnfgfp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lijjllwk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmihdln.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vymtfesq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ehqyuqvv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2yhyejylr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydszhmuf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2voizyqwc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jprpnkgo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wtqikfwg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nyrhskdq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ruubczau.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2enxypbcv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ltuugsgx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yjgihivr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spgtdmsh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nowsntsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdkhginn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2arvhqmct.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2utgypjpn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2aorpoazq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rwpijxev.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qxkexsmv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vlukyxfv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ssbenbtf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oturjien.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zvxmooft.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2izgsiazh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ejwusaei.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dxyxmrhn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2toizseqw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bkjkhpgp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rxkgelhf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2kzvrscvl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nzfydlpx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bcffwhjz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uowmavev.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ddchrray.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gqwrbrhd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bucbjvdr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtzets.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xpxacotb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aawjonbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2meqdlpdl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ukuhkkgk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mjuhvodf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tcaeutiy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aayfkxks.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2itnatsbv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2krgbvwyu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aeulodsa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lmhpjpyp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kfxtjask.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2eijhovou.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sntrhssn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2njvjnkzx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jopdwazz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2naarumyb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hmetrhad.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ifoumivj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bjwuwqbw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2oxnyiwnh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hfrabahx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2iefznghf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2avqeswhi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2krhywbrx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2poxkpidm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rzmbojam.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2oxqozfrr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wzmjivqw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2cmfuyiqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpmxqpxj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qumzwufy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2emcoelaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkupcezw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qkqzurzx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2sxvfjssl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2aiempipk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kbltpftv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2htlkdlki.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fxbfnkle.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bvevdlaf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ehjtzyny.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kocgqdng.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2cxhgbzpp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ojazjqow.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mzplkals.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qcbnasyn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2asmbkeok.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nqyoivop.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rbiyhugf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2argbqmhn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2oeaawrtp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2trbdlcme.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zfwiwhhj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xknxfstg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2yvcwaeqo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yzkzexgl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilizjtow.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cksxpwhn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cvktbkrh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wfetedpd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfwzupsh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gumqitbp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2plzexwlh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mopyqlte.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2isbtiioh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2spjeaidg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2txwogims.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cpjfyofr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qorlwfxi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gmntzrup.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2vjrzjlfi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mpjjfsvy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yhebajdw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edkrhmuv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2hrefmcpz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sbsbuiqo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2huejvxeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpokctgb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sabtoocs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmuwrpog.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbtuneop.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zsyudajj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2btmrcxgl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2erzyvjla.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mzaocqqn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lyofvtza.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uqskcmyi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2udnxmdun.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tomgcvps.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ahbrqdje.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wkpuywpz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tmokpteq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hhvbbkfe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eikbcevf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sphumttl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nnfxoiuy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ebzbarpa.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jfvygddq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uogjkuac.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2erkmfwyb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yohojlng.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eztostea.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ojhjnwle.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2viglvmkd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2frimzaun.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nivhcfvl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lvkrqips.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kugayqef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mlrxcftg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkknqlpu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2skeurzcz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qdvntnkk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2koxpawip.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2afbekosh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rfvjsqnb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vvqxkfvf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kxzufarh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2adlkxjpl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hxiktdtm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2udsfmtwc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqgyjldt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqzvkylj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2izwfnayz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlfnntpr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2benlsgcu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2igbzjmfw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vyaeptia.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cwosxlry.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ehjzjksg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zybjlxyn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2keollhhw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnthwwqr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yxezgmjc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dkoglhpm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckrwvgom.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jbbgetea.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzdumtb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxemkn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gjjyiknv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzugzkc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ipaxnopi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2crvviekl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2guvmthcx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nxuzjouu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ouigtvlq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2scmnkcsr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jdoidnnb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fcehpibr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kosymtrs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lhzmdjgq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2nndvnuhn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2njzqrbsf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ufcxzyeb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkiarkig.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfksuhvv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iscnwive.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wuyulheg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptasghji.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sxlmshqm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hxnxqmdq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pprjeysr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yzrgucdx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2iswfqemi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mjofefno.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxfgjxuw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aigfyfmo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpfnpgrl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fstntrqr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2acdaugzl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvreecp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ghobrssm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2bixtypqk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uhaccamd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2imvvpyne.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xhyepapp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2awgfqnfp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bnxdoskv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rfejijdf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vfhkybns.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2niaahwuy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ndsyidcu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsprssx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ybuvztse.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ofwjtyqu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2oonzpzbh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzuofgp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bannrvtu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qrozboxl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2eluvrgdp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nvtyxlzx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzdkqkyr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xsnzlwpu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uxhpczwa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lvieedmm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gwuotdvk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2grphizlu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ttackyhn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2scmcdkou.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2acnsmmfi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sefuovdr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ndmxjfdp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hfvertdw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2oqdxkvti.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hcpipgxo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kabclkdu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gabnlwds.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2dxzgixkt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sjunntzw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fhbbmdkv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pwsiomtp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2psmtzvpl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2brdaezoz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwqxves.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tvbzxycb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ffxndden.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2trpyrwzb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2najxcqug.html


<!-- 参考信息 -->