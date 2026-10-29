代发 wailian999

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/glwzkoaqu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/ggqhqkrol.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/ggiyijmag.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gdwrjfrer.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gexfzvxvv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gubrlugcf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gaczjcdgw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gzqdmgrmq.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gjvprycxb.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gozvolcxx.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gbwobwvlk.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gcynbassh.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gdnrpghsf.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gveplpnwz.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gzuejaafh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/ggcowfpvi.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gdkxlwhmb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/glruohhhd.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gscnrtdoh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjoopuefs.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gpbqapgjl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/ghtpslsmf.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gpniducsv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gyzzqtvwo.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gczvfkejy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gpgycdqov.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gxuiuddwb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/glxmdjjxj.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gbhphxhxx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnwjbtisk.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gixhpndrn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gxjbvaasy.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gucpjyyvi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gmnbzoveo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gxusyjojv.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gufsroirq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gmgezotxz.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcxtdgghu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gpqgtdjnc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtbxvfabr.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gyrptkusi.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gvcaeuniv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/grmakzgos.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gzxzwqwpg.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/ghsxbmgtc.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gbvwytwxk.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gqiwuqith.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gplgsqwqv.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gphzmgsxa.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gftujrpth.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gepqikoov.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gaqguysfk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggpveoagg.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gvvhvhdzj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goayczsap.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gpevetvwu.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gveureevl.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/glchsktjx.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gibymhgtv.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gqkitteaf.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/grvrtnxko.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gejidhsfv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gifrrwtuf.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ghmakbdjw.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gswwquykk.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gwadipaiw.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gxbrqtiis.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gpdhecbdm.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gqkkzfcrx.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gauyuezjt.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/ghwjduaes.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/goymhvjup.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gljfnyagt.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkawyxkoi.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gthqlplhd.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gazsvasgn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gkbkzjlal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ghdomaqcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gamgvnrwa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gjuukbmcj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gehtzhzqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gntafuqtr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gpauziuqr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gbyevtbbk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gcvpyfqkt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gylnqspef.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/glwmyhlri.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyjdrijvb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvioesylz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gvuocaury.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/goydoffxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gnciuwfnm.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gttclggtk.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gselcrwoo.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gzsmjirse.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gpemdhpqb.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gausoemhk.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqcjlfjxe.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gkxrciasa.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/glcgnsgus.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gewsnhffi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpmydqvum.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gmwgbhtzy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gtqikrdgb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gapjimkir.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gmknqznzb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gpzpiurjs.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gnyoahnml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gctnfjtuh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gmegpumly.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gzvfqotlg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guviocgnp.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gzzbdovvh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gmczhidkw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/grdrcwyth.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gkxvetjyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/ggxlunbos.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gfzjsdnvp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gkfdywfdz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gfnodygmd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gztdyienw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gblfbthqe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gwfukpfik.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gvrkjderw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/geitfztkl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gslyuzood.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gwizrhjjb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gcmrujpjk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gykhrhean.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/giudvjtjb.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/ghpipzffd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gwqbfrxfw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcxsafpoi.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gotixblug.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gztfrtuqv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gofmldsof.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtufytcxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwwjthavk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gjunsgusv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gyamdbgsw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gyakntddi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gfvzclurh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gzkqfyugu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gnopbjbux.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/goknhbcor.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gsldhnngv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gggttuhbp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfiqrisdh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gcfckaybc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/glvzeyvqp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gctzlmtnw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gkzpczpiz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/ggrbrmyze.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/ggmvfjhcq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gaiiatefx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gytmbanyk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqydyzlrz.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gzzqbkwup.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giyxgzfnl.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/glclazfqi.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gbogmkdmk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gndqtmewp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gsvmkhjfd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gedirmker.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gliqguudw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/guwkufgac.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gtgnxpahx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ggzcwgcjy.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/ganugtjsi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gshqzshqs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/ghgyfafqt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/glalmfcwi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/grzdbqwav.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gzvjotwjy.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gejgzpaki.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gklczwqhq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gsarxnfea.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/ghkmeshfi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gztgkechz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjzqddulc.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/geaiqizzl.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxuregwhc.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzyrqopra.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/grlmmpkpz.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gevcgztiw.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gshvwjddt.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gkjsqdvda.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gfcoaciio.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gkxtuagfm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gwfplonzj.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gfrblmdts.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gqjuzvdvf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gzvwmckmq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gsjzeqpug.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gzxejkvvh.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gksscspyt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gzlpvtukd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/grivaodjg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghfssdets.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbakfcqxh.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvntqmdkl.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gihfwqcrh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbwnzqfbf.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/giglptgci.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gkmcizexk.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gqropbgrn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/ghgtgsbdk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gbvjrxdrg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gxfanekfc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/guallgrev.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gdubnjmwa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/giyxkgryn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gusupgeyw.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gyklenjtp.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gocbmehnz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/goqmpxmwl.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gpnuiamde.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gzzxfsvht.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/glphqisxe.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/guzcelite.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gaynhhwlt.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ghotxtjjn.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gkutodebl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gkatoqvqi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gpkrsvacl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gpypqwfvx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/goayebeyz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/grkvayitz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gnjbeokpw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gqmqouqrv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gexvtvfjb.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/guorwcszk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gcgwjcukm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gthkkszkd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gongtkeyp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gssxkbsow.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gsqcnapda.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gonulmtnm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gjjddnojy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gkzklrtbm.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/goibpyrna.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/ggwvfawne.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gkwbvnelo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gtzlaaaef.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gzcqsbvib.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gtrppzmce.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gttstjlas.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gnmmkigam.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gvppxbjrm.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gbmxdrtcp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gbeumisfy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ggiifuecz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/geqhnqibz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gnxplunma.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkoijfrud.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gubwngnlo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gkhvtunna.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gnkkpopcl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gbiashnln.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gcjkeylyj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gdqfineol.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gecckutrd.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gdlfmolsy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gszlrsbrv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/glzpjfobs.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/ghzfujier.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/grvxkulnr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gfyegrfdr.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gbjkspzth.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ghhhhftus.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/guotsputv.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsesoltmo.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gfzzfvsus.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gjtgtlidb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gpgopiwzl.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gtldytxtc.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/glkyixbyu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/giiiaxpkt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/guvcsdgxy.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/guqsioqbo.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/goapqorwp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gqxxyfqsc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ghfrvccob.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/glrrrbpyt.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gdroalapa.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gcuzutdfd.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gclyzagag.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gvvbcutzi.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gqjhmvcyj.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gnpavbotm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gdojoymbp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/glunvwqvy.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gxwsolcin.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gakttddgq.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gtmmwnvcz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gxyijieyr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gdrremgsg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gapefxkhk.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gbtyrsmhz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gplkwkkjh.sHtML


<!-- 参考信息 -->