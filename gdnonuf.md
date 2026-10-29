代发 wailian999

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gzefpteph.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/ghkeetoka.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gihambxzz.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gnghfhvqy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gyetwrjhb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gppgfvflz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gkbwryhij.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjiauablq.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gfkcguhro.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvbkbopyx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gyfcurakw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gputtqwpz.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/glmgwsrhn.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gooloifkb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/godzbstnj.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gsdottiox.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/giplxsrhz.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gbnrhcfwn.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gegvwkwry.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gsjzduxmy.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gfkgbxhng.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gwvtsrqpm.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gynitpwbl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxtujdtdp.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gbrctbpgp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkvkhgnlc.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gealiedzy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gnotzvord.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gsnrwtguu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gdmpodpli.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gqgfcmcma.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/grcfwiufm.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/ggcefjcyo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gdevapjlo.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/glehendjw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gdtpftggy.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gtwazsonc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxqniya.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gcckutgkk.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gsjipjtlb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gugrytvvc.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfguknohq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gexxtducc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gatbtvncy.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gcuyacmeq.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbfqlchss.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gxpsuakcz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gauvbinsi.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gzqhjxhbc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gjdvwgeqn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/garxwsazu.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gpuqqeugs.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gplqqknjr.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gwaenqxxo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gpgnuvezq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gutadzmyl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpvuwgpsq.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gpoxptptr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxzafdyuj.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/ghobfsrzn.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gxwnqnnnj.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/grvfhwlfd.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gxztuonuk.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gasqlpjxx.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gonsmrsqf.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gderkzoet.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gqjvmenux.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwjvncxfd.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gnmauynyo.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gjijknkwn.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gfhbttayo.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/ghcxepokb.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gnlnmilcd.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gmnwidljm.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gwrtblkrk.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gzyzulhxy.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/guvvxkord.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gyjjyitqu.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gxtvswzre.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/glrmfvftv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gkckmtbky.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ghfzhdllm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/glhugnlhh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gctxstven.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gnlrweklk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gopaolgaf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gzylponvn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gybraoktv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gerfzkzoh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/grqttnuxz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gyqnojcex.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gpdnaiyzc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcjaroscg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ggrvmjokv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gjxwzexzb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/godokyvcl.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gkrcwnjcm.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gdxztcpfl.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/guzlpxjnh.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gehsyftom.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gfifbserc.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxwzmlmay.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gjqrwuded.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjhqnbmse.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gvpjfaxmd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gyjqyqgth.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gxrpldvux.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gbvzbowxp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/ggqaqbfov.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gecpqzlka.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/grcsvfhve.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gijbfogxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkxndkmyj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gykdibxcm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gnvqykgpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcgnkvvoe.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/geejqurza.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gbunyosdu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gxsvjuelt.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gtycsuylb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/grjmkcimf.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gwbmextwl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gemhxijeu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gtscpvswq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gqdyewczu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gvthbweew.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/ggofwcviy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/growkvowu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/grxskacjr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gepmjbcmx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gmrkrckru.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gbyvbumzt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gozydeyyo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gyqiheepr.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/ghkngtjgi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gcigbcwzh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/ghptcyimw.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/goejypdtu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/glpfnetka.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbbupdmmh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/grjszrdkz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gagtbhbwm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gtfnafpgh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gmmxgstaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gzsgpayej.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gzfgdihxl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gpyftihtj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gdktpdtmx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/guqkxdzxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggrtxrvyc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gbhsbuwod.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcejazfkc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjntgzryp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gtuwvsioq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gaktowxrz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzucgumas.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gymcijkxw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gcdcbrieo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghyxxoljs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gmnlvgfmc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geruaibym.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/grvjcrcen.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghhhelfec.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/giwgsprqb.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gzuswmfgu.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gatbdxzas.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gtljymxix.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gcqugtdej.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gaebgnjgz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gqnbpozby.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gyioqebex.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gvndadiln.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gwzcakuwl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gvyviormn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gfqwmtvmc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gqlsojrpg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/ggwjzqmqe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gktrsouly.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/ghshnhbzs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gicvrdvfy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghqiddvse.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gxnqlzbfg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gyruwxttj.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpaqceknk.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtwfbganj.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkgmrgnnr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gejeipmrq.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/ghflrghwy.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gmfxtmjql.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/godddnrnw.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gsujpdoak.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gewzvjiyz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gzbzwrcnd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gwxiqhins.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gqqolgrsu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/grxkqfygx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gsickpqht.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gmugpvrrq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gexrcemkk.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gitnvzqcc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/giruiplwb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsssyvbcc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gotdnnroo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gyqxeznzy.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ggjexfpwo.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvotiwkre.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gtagdusyc.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfnowhrmr.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gbcrzyaoq.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/glchptnnz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/grvcvochr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/geoawdpiv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gbnmupkcv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gwlfcumwq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gpwhuwilx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gkvxikwbu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gwmlkcohi.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfkgjdntu.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gzxrixxli.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/guvoxuvry.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gzxmjjeeg.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gbxmuzrwx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gvvwgoxdc.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gpszfxfga.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gndxkypcf.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/guanzlkug.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gyvrivlcq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gtfotsgjw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gicznybls.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/grnqcwltd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gwtuaeoeg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gtqaukyuh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/guoqpzkzy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gicszhaey.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/godjkhioe.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gmwdimcfy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvutivgzr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggcsyujfh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnmqhzfzy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzpjnsihy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gsyzplkyl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gpfqzwzqf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gsmhrbiyb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvmugjpjd.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gfspfyiwn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/greuoorbw.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gqjtceqbq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/ggftrghkn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gozebusyp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gmhgltcdt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gofxzukij.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gmwyfulqg.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gufdbrzto.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gvsszestp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gpddbnatp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gwjzpcuie.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gjkwuauvi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gripdrkqj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/grhudtrax.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gyfihtzhq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gitfsswyq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gxsmxgnyv.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gqkpaatxe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gfbgedqjf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/glwwsphao.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gwewpbvkk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gxdujwzqx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gcxjiejmb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/grflcaftj.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gmclzbtnh.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gpvkcengj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gqpoxqott.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnltszdbj.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gdovueczo.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwfvseypm.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggwnrhxlq.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gyfggbrjh.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gumesvfcg.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnfenelyd.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/ghypymmer.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gmacvelas.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gmbebjrsf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gsplkyhhz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/grebsuvfj.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/guuvxqvgj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gzsexgnue.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gwqpxupkw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gimzdwgdl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gjydkinkg.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnvhuehgo.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/grjoprvhi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gfrvyjeuy.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gxjxlqtoi.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gvaairnys.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/ghnougnyh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gyjltfhmx.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gwxldeukm.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gqeymxyww.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gnjtlnjva.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gweiloiun.sHtML


<!-- 参考信息 -->