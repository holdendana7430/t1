代发 wailian999

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gruphcrhq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gqquqdrkj.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gxfpiqydv.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gbildbjii.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gfzoucuhi.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gwzwpreyu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gpamoryth.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gfsksognh.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gfinhnypw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gaucoaogr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/ggedggnpl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gykoehahl.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gwznldsil.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/guibuukwi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxhpautki.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/golkkacdg.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gjefftnxk.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gztyhgrrp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gszbssodf.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gnxsopytv.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gcapgvxai.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/ggblemeiw.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gjbyaaazc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gkbknrusq.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/glahwbpsv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gyxabhlmd.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/ghzzewudh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkwoemcfa.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gaellzpfv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmifwizyh.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/glfqcwvyr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gvsagatjb.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/guvavwqpr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gzusybgpj.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gcfdquwqq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gtdifyrjm.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gczlkayvd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/guscwypkr.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gjtsueyos.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gwjbkzdsa.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gevfvxxul.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gjbljpmmt.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gnqcgsenu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gkjdnunsw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gnrckfurp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggfdzpofi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gshiptinf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/geyxpotbc.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gwbonufmh.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/glcltdcsv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/getuurfzl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggthhkggc.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gbtpivtqj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyczljj.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gkxrircko.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gffjlncka.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/geudwrunf.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gwehkrjww.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gficmcfrh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/grlnsosix.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guddbzlso.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gnunqroqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giiqxwmum.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/glytwimgh.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gtbthtkwk.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gadjavomg.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gjubugyli.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gpfwewpxd.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gddwhqekw.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gyczltpkd.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/ghlfjqsol.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gealjzwmd.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/ghcziqrlo.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gocselnrw.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gqdgvkadq.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/giuehsoxj.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnltkop.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gjjsncwjy.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gycltbhmx.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gpsjhdgog.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/ghsmbtrmp.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcgeyybfy.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gkbahhbic.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/glsmrgysp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gyvblxyvt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnkjrsawg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gppsoeqec.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/grjknwoan.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gkatioypl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gifzafugl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gnnebubvf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gdefdgjop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ggttstauy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gqbgfiujm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gixgdxbik.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glgoocnle.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/giwuiwblq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/grbgzmnet.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gnvhtltqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnxendknt.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gibjqeili.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gtkxkvsxl.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gkuuyzthy.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gzobxysky.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gstrwiesn.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gytdeqxun.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gtwlaklbp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyuvfqbto.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gleafifab.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gkpwjlwmi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gkwosmhmg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gchykqkga.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gprhbppca.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/ghmarzxln.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/ggwimxkhl.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gzrayzkfn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzlezvqgw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gfzrvptia.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gqfaihlcc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geogavxns.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gaimwsxmg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gplbniveq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gowbpeher.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gqkzmjgtc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gbmqeqyxz.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gkbbhsiwm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gkdshgjjh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gnfrgyqiw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gixypsaub.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gyrutfocv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gqudmimyi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gxcunskzm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gtlzfyasx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gnjbgppgj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gqolpabun.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gjirvruff.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gyfgikkdh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gydtuhxjz.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gypncyinv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gucrdmvhs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gklmnvyvs.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gavhstzgf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnsakvxnr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gcyxacmvk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbrjyjdsc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gdnwoafvr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gavbuxxjo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gwnhlqgsb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gdrjdwmus.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gawgpmsek.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gbtipvmex.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glvftuzmh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/glzstpnon.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gggqoikvi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gshtornbx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvrsrlsmc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gusnywihd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/ggtkcafgk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnwoeolzu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gsggdizgk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gfpgurkiu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gtcmtmhrc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gyiteneky.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gixqboaod.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkgiqrchh.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gwcicuytv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnsxhvmxv.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gkrxirkkf.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gstltuqal.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gqryncwrp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gcxcfqsfk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gbwzbboay.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/grejclgmz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/glqjolxdg.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gwjjbnvzc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gcesdwqjp.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gtmibainh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gkgtavrst.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdilwghsf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gsngimutv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ggllacicg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/glievrvht.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gmtbfalng.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gjhmlwvzi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggiialvbn.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gswmxneox.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gnanfknek.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmjboraef.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbrwcnaqc.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gllpccpbf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glhahynho.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gzbsqztlf.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gmdgjtyci.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/givkibkgb.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gjrtlkdfz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gxfqnudjl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gutcpukzq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gviystfiq.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gtynrmpqy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/grggyinll.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gvlntlvnp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gaulmxkjt.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gzekwczzi.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gcfqixgwm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gcbgckmjo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gqogujpqq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gvkfshmhd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gbjzkvdsj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvjuhnhhh.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gsyqdigoe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gwyuqofst.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gaqpsxebn.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gfnyytnfe.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gxkzvfpzc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gybajnbno.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gpobcvrwv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gdtvogqey.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/guwqfnmef.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/golhvotpn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/glsbxdtru.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/geqxkjkad.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gkfwnosgm.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gbgnujxoz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gmtxxcqrd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/ghadqnkul.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gnclekopc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gbaocexpa.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gculexulg.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gxmeujssd.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/ggaglikrd.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gfdgslusg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gnailcsqz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gitdcrpqw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gpzgltrct.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gafaqqshl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gwkixvmuy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gdeidmwtb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/ghmhjkkak.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gtqipgamk.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gzayxoqoz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gyrzexlnm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwrnrlsus.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtoifxjza.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gevkocrja.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyhyoelgc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/gxfpggamz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gbtmdswav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/ghlliqwlw.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gblpkiyea.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gidhobjkn.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gzwxcncqh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gsvehpuwr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gfaycfizf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/giziicdnf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/ggesturmq.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gxossdlse.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gxkfwbnfl.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gsvombrhe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/ghiedebda.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ghtwqzrya.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gxgqrycea.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gzlnjpgse.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gjaeirnpb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gzbmdizqe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gpkkqkknc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gzxdsoymm.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gqoykbccn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gornsujjk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/golofnomh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gaqocmorp.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gkivebvfx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gjnlfymhp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gkibkuesx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gxtgbxnqg.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gsbpkswae.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gnhdzmyed.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gwpgqotdj.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gkrhfkqqe.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqcyzvuiq.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gurgthwyp.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gqeebsswz.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwfajrmuq.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gkrpeknav.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxscxofjw.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/gouimqpgg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gqlpaqcuz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gwkjnjfgd.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gaddepvsf.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gnowvjzom.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/geenbkkxl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gvyjcdycg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gwhxfptwy.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/grmtuotee.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gqoscnjlc.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/garpcqsgi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gihtewmdr.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gymycikba.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/giapdbgcu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/ghbrdlvhv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gszreedqg.sHtML


<!-- 参考信息 -->