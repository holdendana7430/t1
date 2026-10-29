代发 wailian999

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gnvuukzsz.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gmzcksiln.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/goxstzgje.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gtcmginvh.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gljlpffhw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gektntvye.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gtusvvbnn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gouqjghxz.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gazqdvzuu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/guwksdylz.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gxmhkeyza.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gtogenbdc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/grhrzwuap.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gjroqzgvy.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gklxoveuq.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gdhpfzidv.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/glfcivwoo.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gppuntldu.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gumsdntzu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gbiygsapw.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gqbyhnrpd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gyivfoqjc.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gzhnfdumj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gjueipaar.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gwubbhzvr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmpnybnbd.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmcvfrdia.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gbtigaywc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/giqiyyijc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gmbbyhswu.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gnhmazxei.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gswhhjjua.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/govhrgqsw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gsbofqqzi.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gotzdkate.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gdrctimok.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gapkfgutz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gobfvsnxo.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/grwvohxwd.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvuhejayw.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gvjbfxohw.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcatxqfkq.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gzciwlahp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gbecdpghz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gmlislxoi.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/grygsbajz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/ginwanyct.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gerjqpzzj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gpbaowhah.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gvyllimde.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gkpyftdda.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gqxfsvdin.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gcipkccjq.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gofnjyuhe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gpcoybmfv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gvgishmoo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwiioxuyi.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gduanmpwv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghnacuvlv.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/grugygssh.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/grxpncyyr.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gjechxghj.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gvtgyanpz.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkfgpywsy.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gcawoayro.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/ghxvrxdvm.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gbawqosvt.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gsryuuorx.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gdxeqgswk.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/garzcwnry.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gwmytfmdt.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gvyumxlyc.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gzeefkula.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gxmqvrvdu.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gamucyxsr.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/goybvcbjw.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/guqftccsl.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gezwbryxs.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gydlkkqmu.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gpwmphxui.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gmcfnbgma.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ggmsubrop.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/goqxaiwqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gopqnajvg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gvfjvdizw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/ggqjydour.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/glxskrvyf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gudbstfhd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpclsigjg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/guslhwzvr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmnevpzwe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gsonhllgv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gdjvijknn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gkauutkxi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gldzckfcl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxbpzbgru.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gjzrsqsnn.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gowcmpqsf.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gmfqkfjjs.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gtbnvyfle.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/goyuuqfvh.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gtbxlrzui.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/ghvqnkhol.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gmdsxtnoa.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gaopmribp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gxkburoch.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gztqjpvqf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gbpihbpqq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gxvxglzrr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/grjqicnbn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gwbyzhbez.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/ghzwfpxlw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gktyvxywq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gricydrxr.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gwyojmyzv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbkxkgcr.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gcbtymmbj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/glocdwekp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/grpbbybvw.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gecaeodfa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/glpzyidap.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gdnbyydni.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gxcpemizf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gljeaynge.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gbbkofkpe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gtpfkldlz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gxcufjcop.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gzihnngxe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gjwxovwcb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gqhxsgkma.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gbxorqehp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gpbuwkpms.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/grhwcowaz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gxlipzbew.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gapojkcyd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/ggeshnqdt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gaxgytpjf.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gghulmgub.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gltxlzxow.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzelospbp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gbbtzuhyx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/geceouxzl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/glrbrisrt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gjvxjglmd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/grpblnjmn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gmdghfgcv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gusqdiaka.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/goqiioffi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gkskonoxp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkxlakcrq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/goxiqupht.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxsbuiakk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gsrdrgffv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gexcmflmu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gkkfesewx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/ggohhfnem.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gamrlhrkj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gublavpvz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gpwkvfpzs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gufwlnmoj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzsdughdi.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gndusazbi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnqwgyium.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxeyaawvl.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/grokzeitv.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gveuwlwnm.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gbjczbmik.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gsktrrbfw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/girlyhvzq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gumqzyays.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxsygpxsx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/glgdbshef.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gzjdhacdq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gefgibqae.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gbxedwtdv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gzdpbefve.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gxvroawbs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gmgyipkqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gwggjkoqb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/ghaufnwlu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gjeqklzlm.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gllbqgfiu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gzzonqsxj.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmntrcmkq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdqtgzyzx.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbjjleybe.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gjuybrovz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gwwlfbgba.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gdzobyiwg.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwnmglgfz.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gpmovgart.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gioudilhx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gxasrtrid.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrvywxz.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gslcmynxt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gmngpcadr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gsxcepcdd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gwnxpyzze.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gyjwwewbh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/grygtnctn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/guxzyulum.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ggfhesfbd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/ggfpnugxz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gomkflzqw.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gzpasyzcp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glxvomyeq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gyhsiqcqs.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gjnjhmjam.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gldkyrzeq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gjyxgowvt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/geqdvmvpk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gvponxltp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gxrirwzhy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/giliqduto.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gzaxlbmxp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gjtjiydua.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/grvuszaqm.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwclyqynx.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gjfefoggf.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gqmeshhxc.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glxhrrnmk.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gkxtvzset.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gfhnhcvxf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gswvvlrwq.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gpxbbczin.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gufucbxry.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/goijyyytk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfqysndog.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gkmzlvlhh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gnkvuprbd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gdvgbtddn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/ggvuigezu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gzxnrqudg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gigomxzhc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqwjwmwax.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gnehgdmrd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/givcdxtvm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcniwjvzd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtkmnfvha.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gfetwpgfz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gauvtcozf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/ggznmfihq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gvmbllgak.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gukieunbw.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gcdaifkfb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/glbkbsyqq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gzntifxqp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gazoyxkvu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gdphxruzr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gvybyogyd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gdvjpgxba.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gtzvepioh.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gnvataour.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/ghmukldxh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gxksxrbdo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gmyftsrbc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gghraywts.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gkjrmboht.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gyxxnmjbr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gtobbhqob.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gnwthpvix.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gkqjnyoan.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gruyqdnah.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gyrptqnsv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gtifnwyrh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gjgousfsl.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gbexipmob.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gnzitxzym.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/ghmizuisp.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gwkvxpykt.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/ghzbqzeiw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gczbggmxe.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grhqbxwkv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gjhfxuhcm.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gtsxvlxfz.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gnaofwxtm.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtklxnqqd.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gygtcmqhm.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gvrabqeme.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gajflovsy.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gljuoezmy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gkmzmuqvi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gyxwxznbg.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gongbvtfq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gxhhnduop.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/ghpzltjtq.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gbhynatfh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gdemkqhuf.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gyeexftcu.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/giceoomsm.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gltvlvesz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gtuofzrzq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gtusyuskp.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gisvteeit.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gfmajgxea.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gqrjiivep.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gplicvdfd.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gauvvfntj.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/glqmjtmgq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gnwcwfwho.sHtML


<!-- 参考信息 -->