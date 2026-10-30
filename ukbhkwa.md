代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbvmrwbeq.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gdolhkpej.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gvxwhgovf.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/grqpmssjz.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gtoqzrmkx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gpzqkvcww.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gdbjsviaz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxvmydgpl.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/guccexpvj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gihbmzcsb.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gbylvodfd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/giiifhehf.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gnxxrmcpl.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gtooaaeof.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gpnxijjua.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/ggidjgxyf.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/ggguqmvci.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gpatkajql.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gnixeeqac.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gedgpoero.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gixkadswm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gbntglkgd.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gyeqlhulb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/glmaxbjlj.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gnbdficbn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gpqbnyzwt.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/geiiyhciu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gpmysozwq.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gakknyzvk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gxtpnezru.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/giqlrurto.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gwvorcghf.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/grbqdmhhg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxbmlrxxr.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gsgbmpvae.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gybmvbxvj.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gkdwmlfpa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/glrtdhucj.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gijgvollt.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gczlfnyzo.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gzvwojupj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqlnrsbod.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gijldfkkp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwxynxggh.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsiwpqpmb.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwgikshlr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/ggldvrdhl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/godbfvayw.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gsyvzjvqe.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gqzglcvst.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/grtkyfrmy.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gmvznorra.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/ghquitigz.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gplnttbne.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gzrkehzaj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gxxheyath.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhavewmu.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gkamobebp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gosaldzax.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gwvttztkz.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gueoxrgbs.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/ggpvnjflt.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gighdpitr.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gsujafvjg.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gzwwcjzfi.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gbtizfokn.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gpviokjuz.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gncoulmqj.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gqqgjxwao.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gsaksrikh.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gwomyqmmy.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gwrxfuypi.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gbumxfctu.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gazhvsqcv.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/grxpqtgmz.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ggswbyghe.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/grkhhrgpb.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtugaslpr.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gxeroqcgj.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gqsrfhrtx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gdyebapwv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gzsvmamtb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmdyrkwed.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gxofamteu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gjxwirwsj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gogwyipbo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwknjvtgw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gispxvibi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gzvmyqnnb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gkqszvkvb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gpieksbvd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gneffjevv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdfiehcra.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gcnehrdtv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gyrlxtgml.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ghksvsqgy.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gcmkpchkw.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/ggkumierd.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gpasnbqkn.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gtnsmgvhz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gsjgwtrim.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gywksddkm.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gxooowkde.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gedpveoma.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gzpvczhqw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/glagrsigx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/goekkyzwl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gpbbfhbtl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/giznbbuog.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gobrlmsiw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gwzwpjvui.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gtqctpazh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdkpvpmst.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gafypumzp.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gypluvwzl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbkkbyglh.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gcfzhrpac.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gjohixomo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/ghdkldzls.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gclnkhuaz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gzerozpld.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/grpnjkysp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gvluyzmvo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gjwinztsd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gjlqngvep.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gumolurjk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gwhmouxkd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gxnbmgoli.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gsatdelyx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/grakgtqdz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gpkoeeeoj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gozoiatzb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gwxesiycv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/ghgdbbomd.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gjnrvbxsp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gnwtbibil.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/goqsfixdc.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/ggofnixzn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjaxxrixf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gbytpcaio.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/grbnrkkqx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gxvjjaime.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/ggeenvtbg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/ghgqkrbne.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gkpxjdkfq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwpwlmsbe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gphpeqhwf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxdvoanmk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/ghzwjpkpz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/glnbktczm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/giazkdvof.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gjiukvfko.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gmwzqshht.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gusjwufkz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gyebkvmwc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gfqogccpr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gveuxrdzt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/grogmcryg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/guoqzjebd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gosdtntnf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvyhbodza.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gqceqtcyk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkvuztqqj.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gzzoajbjc.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gkxyeglof.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gxmmyxclq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gsvhinbua.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkrqhmp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ggvgxzhsu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/glfkaeept.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/glfkyzpqx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gqbfnwdpf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/ggvlafqqg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gdldxwpqz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gcojtonvg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gjgtgplhu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/ggxknjujo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gdloyivso.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gcjbvmhdt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gsckbeeae.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gzpvqpibc.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/ghswkhgtd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gsfllxhdv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxupvyutu.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gltaqccic.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnlcjegcv.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggdanvvbe.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gknlhuybw.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gyxzzzlnk.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjkicajnu.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gptwqaqgs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gplhcjqxs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gvbkzxmuu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gppkddjvz.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gvwenndxb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gvratdbhm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gchariacv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gikaolwji.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gfinifqdd.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/grejzioqe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gdixuaepq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghmxyrbuu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/glwkcnwha.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/guoykefok.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gzzcsxyph.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwtntyriu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gutuouewk.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ggaddkxqt.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gpxieaxnl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsbpzou.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gvvozzxtw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gzswwcnru.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gmspevlrc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gbjlmhghr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gcrgvwzrg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gltephulv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gzkxhvham.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gjrtujnnw.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gjimfmbyh.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gydzzoepg.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gnvvtmirh.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gapjpivhx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gqazipihr.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gqjgmbwnz.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gskppgfdz.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gjxazofpm.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gqfkgkryk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gcobseeto.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gebqlesks.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gdolwfwxy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gfdkxssyl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gbucvkwsc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gcsgyvjnb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gkbekzyak.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gjbfjkiqg.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gqvwkyhbo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvgkckqoq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxqzrhvdn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjuwwlugg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gagqfhxhi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbqixhayc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/ggqijmwtv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gasewxrzf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gatrffcsi.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gnyxlnjlr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gsqtsckec.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gxamhuzla.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/ghocorzdu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gmkalkjad.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gypjbvqov.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gjiekahbg.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gqrjhwlmr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/grtsripsl.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gtajdmmhv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gvqloskit.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gzzamoxcg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gfeakntew.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gclyvzpco.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/grngrriym.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gytosypdq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqkviqpgp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gfzutmdos.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gjtlhfead.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gujollcnt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gwedlawcb.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gyrwdmtdp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gkisztnve.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfecmcshk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gptrkycua.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/ghxdturjc.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/guwkucdpl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gwouzsfgn.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqupmmgjv.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gcvbpzayh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gjlsgwwkq.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gwidmlsnv.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gypfpshet.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gzkcjmmpw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/geozynqsw.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghsorlomh.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gzihlujqt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gzcvwveud.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gzpityewd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdcpolfto.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gqpwpzdrk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gfjtcwezs.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzvhrtu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gtpivvhbr.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gadfaqpbw.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/ggbgxafzh.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gwtegspop.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gjbyamilz.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/grvvhulus.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gunivzjuu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gszianpap.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gdjeagenz.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/goiqietfz.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gmkxhmutq.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gqabtorpt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gzzkrpvyl.sHtML


<!-- 参考信息 -->