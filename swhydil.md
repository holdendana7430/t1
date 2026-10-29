代发 wailian999

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gvnuqjelf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gmxhdhdpg.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gtfxjqlpq.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnytjwzgv.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gqfwyxmpm.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gssimaywn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/guwrsslgt.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gaiiyroiq.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/glkxoixhe.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gyeexfvze.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gwvnwaxjg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gxiuewfbi.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gkfinrjjz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gabqkqqjc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gpdexzvsy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gattiusbo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gflfipnaa.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gecbictxh.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gwdulvyei.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gruoinwlv.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gyybbhatt.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gtggwyguj.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gafixmvwy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gqlpchwzx.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/ghranqlkv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/ghlmkpwok.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gdcrscees.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gcsnqxuwu.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gljziiocv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gbvijqrvx.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/grogzniqy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gyizflhdf.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/grvqixxwx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gjyuvcsyr.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gyzmdixpw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/ghwpfvhuu.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gswzuziwo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gdtkwdxzw.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gltnaljck.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/goldxvknx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gsghuiuvt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gscswnlkh.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gijnayoru.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqfyofuoz.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/ggjdrdbku.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjneevssj.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gjjnhyygp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gmzpljjdd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gapztzitm.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gjeziznar.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gagokgiha.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gjdfqbegk.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gjqczcspb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gttnptrug.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gmdfzjkcs.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gsrkiasgu.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/glqlruehk.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gfrkcfiwy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/grwvhuovo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gjcsmzqmv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grzrbongj.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gwbukmddl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gecwbkhcv.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gvomsgift.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gmtmkgcim.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gxbplmjwo.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gyfxvmtai.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gfdgenkcx.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gjawemooe.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/grobnignv.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkgsmtjao.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gxhfhksdu.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/guicjaxeq.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/ghoxqjvfo.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/geontxgbk.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gdbruzxvy.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gutlilsdi.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/ghhefymfg.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gmtzdprtp.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gyavjvlpf.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gixccrwea.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gldwmlqyp.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gvdheyyux.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/guuvunhsp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gwtwvrthy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grmcbaqlx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gpkafnadm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gxwdwrqej.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gisxeinsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/goojctezd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gduxhfptj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gcweiflkc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjflnmksn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/glvqlrdxf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxcyehqrw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gtqwdtjyf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwtjemqnw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gkblnwnky.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/ghquoaxzi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gejlnlqiz.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gutodoojv.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gvtahbonw.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gwriuwpon.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gihjfpwbp.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/guboffysh.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwycmvurw.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/ggllxuctv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gunwessye.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gzhrlocce.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gdkzdkyee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gpkdmpoyk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gpqeydsqf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gwjqtugtq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gyxrzztxz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gdhtxbhex.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gupfnvaft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkggzocjx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/ghskrkugi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gxhjlpxaq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujrdctoi.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gjdaucbqa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/ghuigbgus.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gfptteiuw.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gmfurasbz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/guxnmjjzj.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/ghejbnhgt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/geflpspsi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/godfcqtyf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/geuexvtmb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gjkvsazpy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gibsduqdr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gcarpbiau.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtxnsib.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gcaexmczj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gosbnneay.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gtmbhgmng.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gqprawlsg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gwmizjtvc.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/grjryzhbr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gdqkvwoyh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnvlnrrvk.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gmydtnamf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gjvlbtuhv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gmsveynfe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gbaokwxbi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gstkfqtvs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gmibpikfd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gddfcmdkj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gzdkhxnib.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gesqmyikd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/geypzqdah.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gktqeogzn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdgakouck.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gnrioceyn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gaxpnxnws.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gerhkpbvu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/ghpzqsotp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtngebhdg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gxqljnuss.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gwikkctyz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gebjjfsvw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/giavgrzuf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gjpieixpa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gzrdtcdko.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbxqddqum.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gfwdcxwkt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gifivgiuc.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gymhtsvtu.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gdghisogp.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/geizsebiy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gzvwfsxxg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gumjxewrj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gfysovmgf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/ghohhmcqv.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gpzkprrpu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gqzipnaxf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gseoyongy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gfybxolle.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghguoawvx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsctccxey.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gwxuubluh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/ggpzhlxmm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gwgdeaocy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gqizxzgof.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gxihzrzmw.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gxzryatbm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gfobasrfo.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxnvmrtwp.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gjdiiqfwh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gffgsolyq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gubegdbcg.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gaayawtdt.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gnlwolxzo.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbitpqeqk.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gyfjussju.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/glmaboqjs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gyscphjwg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gtlegkxfm.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gnuwoclal.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/giofdsorb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/guxjigztq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gzccagauu.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gwztgnuvy.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gvydxsqsl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/giuhateqx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gorfykdmy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gifbzzxbc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gorrwgulc.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grsceeday.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/glhnttfmv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gunfmfmmx.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gfrtycbun.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gudgidbxs.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfcqpcqaw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gjdiextfx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gvjpegitm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gzkszzbxs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gfoxojooj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gsxgtxbog.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gfanlwlxo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/glwkwtukn.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gozpdejza.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gayyvrwrh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gunjaldqa.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gtjhnffns.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gsyqxrzmi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaluboiv.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gxyxkhxzc.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gklgsvqfw.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gksuzswne.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/glkyerxcn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/ghmrmpfep.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gwyakppld.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gmgjhrhyv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gralvhqwt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/goflspxhz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfpxjvop.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gtspbgllf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gciabutki.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/glfkyxomu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gvngozlgk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gzdvjcgra.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gkieocapu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggunfmagy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gsohhragp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gnjfxwjry.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gkfelwqtz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghnnzcywr.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gahiugsay.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gzrrtnhfy.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.hesvh.cn/Article/details/gnfwfaegu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gbircmzis.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gqbxjnvzb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/gbfnjhoxv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gjomgxqgo.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gdvmehiwn.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gupooffbc.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gpvanqflz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gpqhoxqei.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gphmdorja.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gncdoxtdy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gvoomkzlh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gnyjpexxx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gsqgoupea.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gamozekjs.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gbeeqfhyq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gabjnyiib.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gjlitbztw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gtwdxxcqw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gemfbokjl.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gktvajdjp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/ghvzevwpp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gameeyeec.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gycocxtwd.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gvdmrcvkm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gnkgtlccj.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gwcrhbggx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqoyhoawm.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gafxhakmp.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/guzjxkpax.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxipdetal.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkpafzcjd.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gisuqotka.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbixwkuuu.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gthxukljk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gjfpwwiag.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gnnmlzics.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gppjgsgul.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gvdrfnxky.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gcwujnxdg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ggzrskkuv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/guhlbqojp.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gfnhomoyq.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvflmiyjt.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gsvpuhtpb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/guteqjlvy.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gxqtjqlei.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfrxyor.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gbllinepa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gnixqyqco.sHtML


<!-- 参考信息 -->