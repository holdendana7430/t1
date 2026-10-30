代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gedshriqp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gdxmxkcgz.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gvxxquwtn.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gwcepqwwy.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gdixgrrvw.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/glqrorlfx.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gfpqfxhju.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/glindnogz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gnnnpqjhi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gfyarjyzu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/guqdtpgqp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfcbdbirl.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gtwjtcdgq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gwfocjsyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gdkvcbqme.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gznvoeuac.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gbbmwtoef.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gmjnlrdal.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjoledndn.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gxdzfwmin.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gsaeeqemf.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gsfxczdtg.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gslnhigbq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gyvhabzck.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gcvotvkwg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gajosjzxz.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gqsrvrjnf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gpraiixdb.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gybeplewh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/ghpjzwcmj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gesgntecz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gridocsek.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gkjbuhlzt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/giduezrgn.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gdpdfgtuo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/geaodwdkc.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/goawvlmgn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/ghthdfymw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gkqzrlvoo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gasynjzxz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gvjdloayk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gqvbieyhk.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/guplubswt.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gazxqrnri.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gpqvqlfcg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gekvtcqru.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gwrlrfiyi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gxwlfwovt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gitesjhrl.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gkijjwgxj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gmadrlopq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/ghxfxvvac.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/geuekawqo.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/ghxzbafwq.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gjlzlnqyo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gabwfazmz.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gokjvpibs.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gufznoqlx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gmtfggnor.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gquttilqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbfbvukhk.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/giyzphsly.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwiergkgt.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gogckcqxl.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gbpwrpcxd.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gawxupimy.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gtpwqnyir.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gdkwqbjwd.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gvzfbgoga.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gnvoiwnzn.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwnrajdbm.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gcyahelkv.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ggrngnnms.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/ggvxphdss.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/ggjizovbs.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/ghjdqbeak.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gparczdhi.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gimgvdrii.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gjrwumvfs.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gbnduppgc.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gsnlegpqy.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/guttvdmno.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gtctjyzgv.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gqnhvfxjt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gbknevmas.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gatemmpmd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ggaubqcla.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gfydkkycb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gwsmyotqc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gwuztnsns.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpyxtjwwq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gexrikuzy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ggnnovgej.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/ggzpojztj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gobfyduzq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gutnairzf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdubgemzl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gcqzecqxq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gjcfvbqph.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gosvmjfkg.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gccsvpaso.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/ghnjonshj.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gobqdoqkw.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gervrkdpk.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gvvhinkfz.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glfiynxif.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gvueqqnpj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzufimyvq.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/giooxqhnj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gxfvnuhzf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/ggfnwwdus.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gxjmdzjmm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gqngsvpwa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gvfifxean.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gsphzytja.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gstkxhuea.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaxtgdhti.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gfhgjdpkf.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gaqoiksja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqfgxnlcx.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gkfokmbun.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gocqgnalr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcetmor.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gpbvanuhx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/grvsxdwib.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gsqugfvsx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gbcyiojdu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gwhzgjjks.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gghmuekmg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/ghpdnpobx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gbykavlbi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gljeloebz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gpggjllrh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gbwqcziip.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/graydfjeg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gyvaxxzez.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/grbthzzlo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gbqthlmul.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gzvjgodor.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gfktrxcqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/grrgpczhp.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/ggvtcolqn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/guvlmvsir.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gnkuhofhv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/ghfrpqave.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/ghicbiycl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gkdqbbdpn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/ggjjflhni.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gizqnunty.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gwefyyqcs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gqixjjtok.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmdyizcrm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gnefjiwgl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gsgesqsos.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkyplfvta.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gdkrkugxg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gkvpwngus.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gxysvfyuh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmqlaacsp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gkgtlqlck.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/grgtjilur.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gngxxgjrm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gjzhspzye.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gsbmvhynr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyjdifiwj.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gmxvqpzxg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyieyefbt.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/giwgloipn.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnywifxc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/glnwqalyy.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gcokexyih.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gurnenscr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/ghumyjecj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gdaqgaqci.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gbmeoszfz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gxizahkgc.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/geppjzmza.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gsxharwls.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gqvddduep.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gkzldbqqs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gimsfnbac.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gaxkgxxpa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/ghydpzfeu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gtemcobhs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gpiqyjdnm.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gatspmfqn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gfbrkucwl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gftumvclo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtpuikdht.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggjeperkf.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/guhbsqmxe.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/grelrjnpi.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gntypntbg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbwswzahm.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gokoyxqoi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gegftumgk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gysaqftgq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/ggybapmml.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gmzkymtnq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gfascjzqn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gqeqxsamj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/ghmyjieiw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gytybwsbp.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/ghqqllloe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gwjojostm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gheybfuyl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbvzeiaka.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxcwcfnct.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/glmgcdinj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gaocsgwmg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gooenmpce.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/guufpmtju.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gdqbotdzp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gnlbcrgbf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gxpvihuxb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwyvceag.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gvtydrmzv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gjmncknsx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gllqynlcu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gkdhffuid.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gofdxotlq.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gyvsyhlkg.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gzeifmkkt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/ggqmhvzcr.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/grklhaqul.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gircbadei.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/grxewqamk.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gqbvbolbw.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gmtyncivx.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gxaxywhhj.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/guvpiwnxl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ggysjiydv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gugwoavqa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/goihdelgs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gqlzoyedb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gpykzzypr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqvjqlidj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gafkrljqp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gzwhmzewb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gzemhxfco.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvehxinpt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjclrhhia.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpryxfqxs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjpkomxwh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gnyuybzzv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/ggslbfnme.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gywyaxahf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gicrjubgd.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gzpvlpvas.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gtnwixnic.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gyzntwdep.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gstypcowc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gcdzhadig.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gujtbempl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gazwvtbvy.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gkzndrjqm.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gigtvcpoz.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/grijtceig.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/glooykkfk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/glwhgvefw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gfhdfgoea.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gqzpisjjp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gfqamionp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gfegvfocp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gwevqqoor.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxmlwvvsn.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gvockbxta.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gqbkugilw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gwfpzkstr.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gsnlayjrl.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gymwdhttu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gvodcwrzm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvvybjabc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gfugyqcok.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gycntfwrj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/ghvlcybmb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/grbcfubzn.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/grxjpzooi.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/glvbwvkuq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gpwdnwmax.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpkhnmdzp.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gbylvdevp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gxriwqsin.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/geodywrrs.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/gbjjlayfq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gofxlqegd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gtzfkimab.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghjylmcix.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gmiswpokl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/ggjquvapx.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gmvrjkudn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gwwdghlzu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gjcwcgraz.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gpajcfxxg.sHtML

Py:   value = data or "默认值"
来源：http://mobile.zdbjq.cn/Article/details/glatwwmba.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gtodcfver.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/ghshxlnxp.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gaojxtmdf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gackuyxvp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gxdadnhzp.sHtML


<!-- 参考信息 -->