代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2duoftvyy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2slcuudsq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mchabddq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tnrpjgag.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ziwymnxe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2umkquxaj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2uryqmuev.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gwivdwme.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2iyvmgooi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lpmzterq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2juxmlqia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2swtsckhv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hjorsidt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tguuqjje.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2aamvxbgt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2imriimxa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ruvctchc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ptamolcy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xhyvqual.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zpjwwgcb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xgyojjjp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zcszxgzx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wajlparq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nunbolar.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2abjykofi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxbkurr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ubfinkit.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bqbnzdhf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vzytccer.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tpzmdnee.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wxvgaidq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ctwwahpw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tueepkuw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qbnruaef.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qvualgmw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vyumkngf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iyyzqlym.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sypxepxm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vzhmuaig.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqbtzpim.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zhildlur.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qetyurzh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fgqwtrrb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lkyekwda.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sdnthjwb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2tfrsbfbt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2glrdfkiy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wnhjwbyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzpuruir.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2bnrixdco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mljiwstw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lzmnftsz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xkjphotj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2dfhtmquk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ijymupmp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qrfyquat.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2taaeheax.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rhkymijk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oynrgbbl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oijnnize.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jezgymph.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tksiuplk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qifavabe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2axxvlyte.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yrsqotzk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2flfjdbwd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tbkutcnz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2yiuliant.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rqncgyxq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2camxoedn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xpxpjlhs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2omhntxxf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jxqnjbct.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zvpkmdwz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ntenksne.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tyodtnoh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2yyuakepx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jhuuifnq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nukigosd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wiaezdmv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gcpedskg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bcnyxowv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kmxstbnf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2esufwdkw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mvkyzkfi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nqvrwoqo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gzncqghw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pskwekce.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kuayoaci.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2paglhnpr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vfmpqvtf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lpcacmls.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ynrtxsqc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bsvkclfe.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xejxulgs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jhvoezpr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kjzqpxwt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zqrucqhp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qekfzlcq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ayginity.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2eowiqyff.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tqthaisj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dwptqwzv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2smcvimmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akzyppyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kkebjnyp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vfjkjtzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwlvrgyc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fehknjuc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pqttddni.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yhwxzzmz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fmpvaolr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2crlqgywh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fdwxjwel.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dxgezghr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jkqbgfip.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hyahotdy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rtaajiji.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bpkllhzj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pishzrrh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xxrrljzx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xfoldmpm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2advfdhwm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ocaibxca.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2amuuiciz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2lmcrjlbx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wyvhgfgz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hxchjqqr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vfgblvdc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rvvofzvl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oenwgdmk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2igglgvvi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehbjzvvx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpmbwzhs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zdrzwunp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkojaltx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cujrbmrr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dkwgovgs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2edyaggac.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqryrvsc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ptksqtnh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2auazxiba.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mmqomtls.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pkhworrx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fmeffcsj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nfzhnvxk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqzzhagl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xcryytze.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2klvvrpdt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tkhofzjg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xrbwhrwp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vwdqoqxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amfhfzju.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2livebpbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qogdciuz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqtrkzaz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nvsbzuje.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2czeyzuow.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2enjotjuz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tmfxvmto.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gltkheyz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ruodiznc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uscjgyca.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wbwpefgv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qfrgegwz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgcqtn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2okfljlpb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xbgquipe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2duigwijw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kjerctjw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xhsleqfo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2iomloovd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dciqycmh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ygrfvrmc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2owdhruyk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxgyresq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ujakijgy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hryazcoo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rszqvhfg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hcssklnx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2tdnvqrhd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pevksrhj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qopwxsac.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sgsummwb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkcduszm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uhmwfxel.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uutymftm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2lvzybxuk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2drijwakv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gexjkkow.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zhmunacm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2zvftdgze.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bwobhrdk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2krwiyxau.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pceevwjb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmbamqse.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lblpfvdu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2phgqlucp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fcivuyed.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jcemwvca.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2awmddscz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qwgetaxv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2znqngbbx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ixwyxvib.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hvmvljkz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ranvyepa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kmnducst.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ppyxrvoa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eureuajm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2cxukyvti.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnkiqiw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nwifvhtl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uhnqvvua.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2mhwurhpf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aduhtzgi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cftzvhna.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kddscxda.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wnlvnofx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2sbcqydbt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zakyezou.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tyhsbgli.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2otxrqpct.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xkngvmsw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2itylfkub.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xbepfeoi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2sorwrjbg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qsilbklm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yhufflzb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gontfudt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2umtrzjxs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lqivrqou.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mqjjobxa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2snncepgk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2jgbicmid.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ctwycgyp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kevzrgjn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lraiehkz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wphbtfgu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rhguqeie.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hjmibojb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jbjsvkhb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjkuotpz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nnbjelxd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ulnulgpm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2oisujlft.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kpdcnllk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mvpwslev.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dlboepzh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yauacpfu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2anlvouwu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2msajbnae.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjusdy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rixalliv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nwkbxpwt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbvbleec.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ranjgfvi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lugwbhic.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ssaeuwqy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bslfebwa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xadznuux.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uuhlepgp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gftpjner.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2monjtlve.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2popyswby.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xhpdueda.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qvttohpc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cygzyoos.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fwtdqqpu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2igxhnmwb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vxlgqujm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2htjyjbko.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptcxeaxj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dfmtbogz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uwfqokgj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jijitkur.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mviextup.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oipllbfj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qjjawfvg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dioyxfcv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mwhoymwd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gqwdeqbt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nfiydrvj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kcpnrras.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sdmsimir.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2izblxvrd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xkitnfnf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2vyqdfdct.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzcvqvc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wuniahvq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2daikppxc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2iozwozqn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2pzzaohop.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2pjpyubld.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2scliuvly.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2piduzmva.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lftcgeiw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2oopulgqv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mxzuohwn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gbkjuexw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jlbsfhhd.html


<!-- 参考信息 -->