代发 wailian999

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gsdgdjfat.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxihxio.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gjqzfnxnb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gtdjgpilm.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/ggcrypwyz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnqbihy.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gjlksklwf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/glfjefhlw.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gnvmcbius.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcyieulqn.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gbkgpqrug.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gguiacahn.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gmlydwyvo.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/getkduqgo.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gsmijnhik.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gqbcqfwov.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/grsbpvxgt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gcvjmvhxg.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gkywnvwuc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghipwdizy.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gopadoaqv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gdrumbkhe.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/ghqnfiuwd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gufqmoawi.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbngucely.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjtxpxhsd.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gzkoobcos.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkarmju.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/geeeaygup.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gwjfaurqw.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gkyugdufq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gsxaivhgb.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gqbjatcaq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/ghnqeufhm.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gadjfyinp.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjapqzqxr.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gawryyicv.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkhhitsax.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gerkluxtn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ghuvelrok.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gpsmbuinx.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ghiajgwkk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gttrvriqa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gsmdhcuqp.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gkhbqbytt.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gfwwgpfbt.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gdkavpxfa.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/geviuzssg.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gnyakimgk.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/grtzbjvhu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/ggsmvfehe.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gmfqolwid.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggswhvcjb.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/grwmvzkfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzhucbfbn.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/grxaseubq.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gqsbbiykc.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gjhugfyor.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gojlqnalr.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gugftanvs.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/guznnhylh.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gjshqvjnq.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gacmarxtr.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gonldrofd.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/guyywmvaf.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gexktzezz.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/giynkpset.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gpmionhht.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/ghigifjjl.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gabpojhry.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gtdvqzmmr.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gvufrnhdg.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gguecreue.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/geldaeles.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/ghqddbjfm.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gbueqlocq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gewoaqgna.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gqiejiwbm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfvlmhpil.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/grkzewjfu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/ghrzmyuhy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gxsfutohj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gpztdlgpi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gzpmzayeu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/giqaanjcv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/geepybgqp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmdgflnjy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grzbwfgzr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gswzhhuye.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gwkbdxxly.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gcjzasduk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gygoqukhq.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gquimlrhy.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/grxjrohpo.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gbvoqdhvw.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/guosnoghv.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gwiwzqsgf.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/goawzuwsw.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gpwwcugub.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzxebylyx.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gexwjtclr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gejxlswdp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gdedbvehp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gsykvcohx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gcbfxdchj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gyylavrjv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gurujwtbo.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gozxuhvus.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdagskklv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gceqhnqlv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gkagiykou.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaapugfca.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gtdalnjtp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gbmpourgq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gzegnnato.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gwubfodoc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gcjafjtsq.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gajtsphih.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/grmolrffq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gkxcxfuak.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/grxqfxecm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gpbnngiel.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/ghblutarq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gadjgckfz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/grcohyygb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gxuqtwpbf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/govvsjvno.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gyagwhbey.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gsqswvkhj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gqwfudckf.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/guuqbuust.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gxoliohqz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gqppgqira.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gklgmsque.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gggqlzkco.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gibhgltnn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/griubktna.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/ggqctcixn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gutctddef.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gqpnvadpu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gpjyzuxac.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gszfgowum.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcttbokwo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gcinfxgpg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gzwmbaxtb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/geofznwyt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gnhkxlewf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxeqsjylv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gipxnphmb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtsmtmslz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gfclpxcii.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gcydgqnqd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/ghbferjsr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gbdtcbyrn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gftakuszo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gbelfzfqg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giuwhzfds.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gpepdtbnz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnumtbfom.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcdxztxxw.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/grhyfjxww.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gdcghjnps.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gcngubklo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/glkcqijgn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gnsfdsnxf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/ggpxdditr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/grtggqamc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gfmcdqxpd.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/guyvehkgw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gqjatxfzi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grqrknitw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gmqjbocjx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gttcxloki.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/ghlglaqsl.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gjljiwrna.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gjxfnxgzm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/grodycazl.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgcvioj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gkocitdav.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbgjecyej.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gcvzcioad.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnkbqcksm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzcyhrjbu.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gncmwugzo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdyjpsh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzubdqpaf.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gzppwdgny.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gurmemtgt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gyljwrxkz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gczbocyzg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gevdyblcx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gfwlpifbf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gxbamsihj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/griwmsswz.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gwftfzqou.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gnfqhwohs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gnyobwiwa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghppqmljs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gatdeyybt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjzphemoe.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzaudvdyf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ggumfvfgn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gewbinfwf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gcprzslne.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghromlzjr.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gffidzncj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gxphtxopb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gsvzghtjt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gwvuyqeay.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gqawpwepj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/garzoyzhm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/getjuuhrz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gewdfnevy.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gblffabyw.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gohoblzwu.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gziokdyaw.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gmrqgqrrj.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gryjlryxk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gydwjibje.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gvkdgrglc.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gusqygtpg.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gdvvxhwbq.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gstzmihqv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqczlukaz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/grqyhvotn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gnmzopfbg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/glrwoznwy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gtkwjjehu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gtqghfnkh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gxjadvply.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqthtzula.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/govqwpgpb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gucodqrsm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gusarsvtv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkandvjmn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gilqllbri.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcncpclle.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gxezapvfy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gnaxxpjuy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzvpsjuow.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gkykjstou.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gvgwhibgg.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gasyxobdt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/geozwvfsa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/glmgvklbk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/glmoelxce.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gxwtfryqz.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gdqwtpwhy.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gxfqxuijl.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/glavthpwy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gzlynqyrc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gmbesckpl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/glzqgkzap.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gsuorgxgw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gzwelxxlp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/giqrjbchk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjpwmiggn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnfbnrmfl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gkakjqsyy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gtwwmpoeo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/gwlcgsyrb.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gepvlzxeu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/giyaxfgzl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gwhygdohf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gyxppcyzi.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gnfquxeni.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gplctunpq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gpndpuvjn.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/ggfmlzkic.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gdekinfnp.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gcdjhqjfs.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gtsrdoeft.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsuitybdw.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gpfwtdqfx.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grunkwnqe.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gsttivhsn.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/gmkjgqxqm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gtfqafnxd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gyycpxuxc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gxushfliu.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gqvblcyha.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gcmshqutm.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gapjtmdti.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gjrjansld.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gevivngoy.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gkaqhpzfi.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gitcmfvos.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gssduxvyd.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gyrajrryv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gwmdoyihy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/grcrplgzw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gvefcxxja.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gqezivxjd.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gynpeswhd.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gjovwmpyb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gyufjsxld.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gznubyiiv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/gasooaedq.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/guknggdxd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyxpkbhyc.sHtML


<!-- 参考信息 -->