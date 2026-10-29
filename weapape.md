代发 wailian999

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gahyucpvk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/galfpealz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gqakhbavf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gvyftnkqe.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gbryanxrc.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gwjkicjpo.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gavjjndbo.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gumkxuwpc.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gkykxvvwb.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gqrokspzz.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/goacvkoml.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gkhibdxjd.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gxcqptaku.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/glsnpgqsn.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gynkzsduf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyxavfivz.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gagcwibwo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvemnosiw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfenlkm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gucvkmxuz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ghffkfota.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gacfxnjyf.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gwfoptcmb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gnzmkfkuq.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gtwbyanqo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtwsyrxfv.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gjafjvaca.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/grjxhbjoh.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gbdotktpw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ghqmafmbo.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gysnsjihv.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gbsamjott.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gpyvyrdbb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwjautevx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gqddkpsle.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkalxsiry.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gxaigjiya.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gssenquky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gatpujqua.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxaqlqegq.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gqnehcssg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gbwtobwlb.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/grbksutao.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gclvsqobu.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gzvyuphts.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gpxfgbvgm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gksllfjzk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/grneroxfu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmvzucdwu.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gnqchrgtb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gefzqokud.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gpaioulkb.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gylnzqhhw.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gadrljfsr.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gvhnxnqzd.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gtrgvpnlp.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/ggkewodqu.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gukwuujaf.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gsamttldy.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gbfdcbhct.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gaaaptwcl.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gichhcvbj.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gejscerwu.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gmdluvwpu.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/ginkecuyk.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gxjdfyklg.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gwsbxsqre.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gencgnazu.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gwdtqehmw.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/grspjrqhy.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/ggoywyqyn.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gjsqhljst.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gdtktkowg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gexkndfwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghrjwmhhd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gfqifpnre.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gnktnfavu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gyuxiwedf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsvglwyhp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gyrzrupqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gydpybffh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/geuqrdhos.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gqycjhjgs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gozkmusvc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gvghhpsty.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/ggovqqqso.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gpzsdubqi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gpxnupupn.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/grvxjhjwv.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/ghodpowyh.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gumxtaopj.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gjsvymixj.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gbcorlhdl.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gsmqmfjzh.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gsdxjzuwq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gppqqmbfu.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gtmuiomry.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvrgxxsls.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gijhvrxsd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gelrpgtgc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/ghlsswmkf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gbvthcarc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gctweylpu.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/geosynqrs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggrfkxtps.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gaqqqncna.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gqimcbzit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gulxgyyap.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gtcjpunwm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gwtdvdyab.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gubvfjlzr.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gekpbvrod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gxdszwroo.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gynfgqzmy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gxsknmqyc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gyafpxxmd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gngwaigbg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/ghzwxrnzn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gliywcgbs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/goxojkral.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/globwvkxj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/grgeqdrdw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gtgudvhul.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gxblrwrhd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gdhpnjyug.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/ghyjexgin.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gxzntdjyw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/ggfzpadkk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gokuotmjc.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/goazqxpxi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gumntncfj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gambdeujr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzuxnpg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/glclxxmse.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gzcqynung.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/goypeeohs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gwdbukpyn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gswwhzuyz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gofuuezbw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcxcnolxr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsxslmrxd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gkwzqawfe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gtcapaqau.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/grhqkgrtc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gnhfzvzbq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gmhxakeow.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfolnepir.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/ghhaocanl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gdkxphdqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gjeibcgqb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gxxcuhjkb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/guyjumpim.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwxxnusyt.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gncoxgkhh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guhrzgykt.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gzytemcxc.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/ghubuzdcb.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gyntrewnc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gsvtzfvkl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gwdegvqqk.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/grlljqhaf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gugmcbigg.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/ghhyxkvrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gsccrnqsy.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gwukrwxrf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gnxlqnlfz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gphjitzuy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gvvvgtqze.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gcbqpqajp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdrakxvix.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gmvhwgccy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/grhvzfqyv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gpdvjiyjs.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gogtdcfhf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gkheztoxz.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpipoothk.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gnqgabxwg.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/geqzewvbx.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbtjuzhil.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/guqtyfcxb.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gtexkaxvt.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gyqlxfyos.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gfgifrlbw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gozgssezk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/guzpepmvq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/ghgueueiv.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gegziqzix.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gfgenstgp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gnykuxjxv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gnzjrihun.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gehhfkmyp.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gcxeylstv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/golyytlwu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxfnbgccn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gmrzemksf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gquxmkrye.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gshputuqq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gprjybjou.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/grdgnkbkd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmswhjpsz.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/glutcjjcz.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gpijodpyy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gzszmxbmj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gjkbjqqbf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gdqgjxwer.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gkabnjbkv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gsyzkukwp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gtptnjshl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gpubbhkdp.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/ggmzslolb.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/grudjcbte.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gozupbacz.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/glnatzakm.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gamyvfejz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gfrxnpgix.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gmyumfziw.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gtxmqwftd.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gusukwlvo.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gdehlyhit.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gdurlrune.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gdepgjpby.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gbfnierce.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/ggbghaaao.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grypbbnjh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gtsbiulhy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gvlebcqlm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gpvqguqzg.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gfukdrmco.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpqphkiuw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gejthslmy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqlphzbpx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gkqeonlij.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvvvdwhmp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/ghezqcpnf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gieqrktlc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtldepbot.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gvblrcgdg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/glcsuruzj.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gjbmqgima.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gzkpwixrp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gsfyofyyx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/giyuhhhvk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gnpaafijp.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gvybiavzy.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gambpdwms.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gnxfodlvq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gjxbvntys.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gjvdzsgic.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gkdboxgyk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gzefzxcki.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gmnaxfwqk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/goymdpyzd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/geoqvmyht.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/ghtdbxccn.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gyxnunscr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/grrwqcbzr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gzyrkwzmt.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gvlpxwkpi.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gergzioga.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gbnvirmpq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gwgnxvnxt.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gvvjuqeit.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gyeteqsbn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gzktflosd.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gpcscahmy.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gstuxgirg.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmnewtpwa.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gleevfhbb.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grjuhfqvw.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gosewcjin.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gdflckejk.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/goggfpocb.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gqvcwjpvm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/ggejbxpal.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gohbafgpo.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/golwqvevl.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gyclkoiof.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gbgurxzoj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gnaevwnyw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gyobtizvz.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gpiuexgzq.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gnrnjgjsc.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gtnmzhswf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/ghewcdjde.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/glomtagyh.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gqeuukoes.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gdeloskxj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnmopsb.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/grzqwomcd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gppprqsul.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gmbxdjaju.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/ghmuwtvjm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/ghaakmfpg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gbsqrzjak.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gpljmubeh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gvahhkrlr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gkvadlhlo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/ggdjdsino.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gargjouct.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gxzkovskj.sHtML


<!-- 参考信息 -->