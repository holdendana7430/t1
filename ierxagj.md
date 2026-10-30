代发 wailian999

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gbjwwyxgv.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/ggyinesdb.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/giybnuadk.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gjeydsxyz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gpmdufvzn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gwczoeqou.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gqyukxcmz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gfpvwsatp.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gcocmdbvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/graovdqpf.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/ggemskdpp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gchekzeue.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gxacwddoe.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqbjndw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gvprhssoy.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gcqiodppy.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/ggflgphbt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/goaurinqg.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/geilhlihr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gckpegmxl.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/geelzqmvg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gvszxoubs.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gndnpnqpx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grrhbwmlq.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gznxkwodk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gztgxaczw.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gpydqghin.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gdvzsscun.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gumnutqcj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ghsfjbmwd.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gyemgvuen.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gjqariimb.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gbkawdpyj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gubdugqau.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gloqjqnbr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gtembnxbv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gzwcuwyqy.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gsludmzul.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gzqckflzb.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gctvkqcfi.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/grbhtehot.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfauscbxf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gqgjgiuqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gfazkxjls.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtqsowq.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gsgsaakze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gxvrhbkep.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gevriaden.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpcetpkas.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmasglv.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/grzknnwmi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/godckcpdu.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gigtzqbwr.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/grrjjlqla.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gbxxoanys.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gvbejkdxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjdxoujeu.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/glqiilwvo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghghlxrpm.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gvakhzsky.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gtygsfgab.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gpeqxoxcb.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gmvjikfef.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/glboeegpq.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gacnlicgf.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfxrdupqa.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gubrjuxvh.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gexbsqxzj.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gpslvzkmg.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gycrxrlaz.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/guxisrcaq.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gidkmxgno.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/guwlmsswl.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gtodhcamu.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdfpcyo.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gnluzpfja.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gbxsrwprq.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gemttbbno.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gllubswco.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gusdjcusd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gtmmflzoq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gwbisdxte.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghxfwqdwe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ggjqpyzac.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gpzsfsfbo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gqtcwnmjf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtmfqzjox.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gvwvwvqup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gvdmxpkgy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gtxfkawbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gcthspusf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmywibdxw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpjfonacp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/grurldiqt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gtxvtfmhn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gdzxxkxuu.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gpiokxufq.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gcbrhqpts.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gyvrvvjyk.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gkyqtlmtk.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/ghuqwfodl.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/ggrtlanhr.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gacumjriz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gindeuuyn.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gbvnxztgn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gngcnookd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gspqgdbiq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/graxughur.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/ggemcynew.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gyfibragn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gujkorcwz.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gdkcukhra.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxzannbga.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/guneauvyb.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gqwewzxsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geivjyfug.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gcwlswsyq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/goznsnacq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/grhqxdffe.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/grfvwxxni.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gwazcgvik.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gcoarhkno.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gvxqmcpvz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gtcfxydsg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gpbhnjoug.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gympvlzzk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/ggndifsud.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/geayzvrpw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gkxqacrxw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gkdedoyuq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/glzzgomxt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gxxgvyjaa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gawewqmye.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/griccetfv.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gjyuldsgm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gcmrxwfcv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/giyoiahyc.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gvgndwkyy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gbqlbfhvl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggvjcypej.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/grdkdpgtm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gcgrkcndd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gspfcqxah.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gzrrzrfen.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gfdamfqci.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gssderiwk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gypwnnkyk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gibsfeygi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/geynmldqs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnptfzhcx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geboqjgch.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gntczgexr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gujihpxyj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gpwrcxeoa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghhxadlav.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gqkutapnm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/ghfqqczhl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gbausuodq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gukkwoybr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gwsefgkye.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdofcnmbw.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gzpoqskgz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxlyornzz.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxdbedtoq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/ggfnajckr.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gitjwidok.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/givzkghtp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/givqzqgzk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gboyykuoo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/glraypjbm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gxqlwvgpv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gjusgvwly.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/ggtftwgnt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gqltyuwbz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gewmtbbiu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gskojhpbr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghacmuhuf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gjddinzpo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/goerfrwdf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gebervrme.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/ghcjjvbgv.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gwcdvxpap.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gyqrbcyrs.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guqdnogdk.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gydzttmcx.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfnfxcsbz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbcsyxgns.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ggweirjik.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gjsaxpsfb.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfpnmweub.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gytrchyju.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/grsneiycj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gkiaodwpr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gasxvbsta.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gfhoggffg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gahgvajqi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gcbaavtpo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gzjcuzykl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gnqjtuvdh.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gybwlqiai.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbxrmcg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/guqfyfqvm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gzvyboezq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjdwcvfwv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtzevtaqx.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/glwwtgetw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfgsobbyk.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gpezyidod.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ghjhtijkq.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gwltfuver.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/geilpydda.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gdrwghskx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gghajwtsn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/goghqadgt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/ggrzzwdpf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gjrmseoab.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gutrhspdn.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpiyrqr.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gjtjvdhwk.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gooiggqql.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gtoodbwtn.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/goosdznyo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gjwbjsyqg.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gaszwjzzi.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gpjtwllwa.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/geykyouig.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gvxffwkkr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxatbawnr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gtblfppxx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gjsrdqhwj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gilqarwje.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gosvlvqsc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/grlhztcvm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gtdysfccy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gnksgbdkm.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gnsorerpm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/glczdftya.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glbnsbtvj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcwfewca.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjohpekyn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpldpeyxw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gqherliml.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gokfriopf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqslhyrba.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gvqbppiif.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gbnicmgrc.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gasetmsux.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gznicbudj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gcwtzrcpk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gftrkxdfw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gzjyxsyvu.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/glfumatzj.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gkjceytme.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/goywhqjbc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gwcmfaaoa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvhlhesql.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gjoppsmbn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpzqvpc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gtdbhguyj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gdbknhalq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gmgzptvzf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/geaahmtda.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/glxkarqck.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gtpqqdxue.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvikuwsv.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gfwhbqsft.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/ggrememie.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gsqgblbjw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gzhgwksux.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gdxlzmxqa.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gsxfelvtk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gemqxvnta.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmezhjspz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gidswqcip.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/ggbjvpeiv.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gttmrqsbl.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glfuazacx.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsxpcqpmg.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gfvnhxcrn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfzqolesq.sHtML

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gwktcrhyl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/grquvwndq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/guweqxvww.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ggsvzuhre.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gkdftsjov.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gvvjqqdom.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gsgnnuyin.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gumygkzwc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/ggpfvtshk.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gdsdafqjk.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/ghlzndtko.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gcjswzafh.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gjprdvqji.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/ggphlikai.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gepxizpar.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gdhlvogev.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gskmsoxxd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gbtsgzmlc.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gbchllymc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/ghlzxwrtr.sHtML


<!-- 参考信息 -->