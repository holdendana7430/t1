代发 wailian999

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gfledxemg.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gytqxobuu.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gezebcqko.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gxxakbmtg.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gpvoaghcg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ghmmmabzs.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gaetqvkwz.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/ghgeismrg.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gxzlxjkac.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gxupbqcgm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gezbjdbcm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gsgtaplmj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gffemescv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gsxlfdgun.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbpqfdjuo.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxbkqicvf.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gslkqkhdg.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/glkjnoyqr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfhunvwjo.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gsoaevrvi.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gveddhlki.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gwmdllkbk.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gwqgleivg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfeamjcjb.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gbtwjmbmw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/glrabaroq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gehjhifgi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gsfpdubgr.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gxorremco.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gujbiffkw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjetgzafc.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gpbjhwryr.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gqanunqjp.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gortqfgkq.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/goaoolblb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gxtynzvha.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gmqrapxbr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gfbqczwih.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gzrllsvbq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gaewaklzq.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/guhcjrhkb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gslrbrczg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ghobxlami.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gtnlxdres.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gwthrukac.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gsxqtlucv.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gcribwend.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxfkmzipg.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gvezeqyzx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/ggiskytga.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gbbojiutu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gdyqajzpk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gplikwmxc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/glvixdcqw.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gucaaqyyp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gatjktxmh.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gujdobgeo.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcihrsgzh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gtuhtvgfp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gowluzdli.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guctntvif.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gwiruyjki.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/ggajomace.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gpgzzzizk.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gbjzmwvud.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gxtiohlzb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gsghdwnxj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gmorrspce.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gjdolyyod.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gobgzyrdw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gorujlfrh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gwowdxasx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gialyibok.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gowpwjyrf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdqnpvwuy.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/geqsswfyd.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gpfujvusi.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gcdrvujva.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gpdkizaoh.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gdkigujxr.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gofqehepb.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/grpfvulle.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gvfactrkp.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gqyavqjym.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gakneqjgn.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gzclwhsul.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/ggltwhckn.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gbyxvylnb.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gfvxzvxrh.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gkuxdaxxw.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gmtpmqdse.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gqoamiymh.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gpzaiddvf.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gstthpwkn.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gtspszbvo.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gwoohqfwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gjxwdbmch.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gbixdeysy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gkktjylep.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gkdvptuhx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gfflaazhq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/glgmovkoo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gcahmmnsl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gcdgxxrqa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfsbcginf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/goehxvvvn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjvbbzpnu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glrrwjvqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghccnkttw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gmyvygsym.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gswsfkmzo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gykxarvkf.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gzydogima.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gbyxhpxek.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gfkkxjnik.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gpcgtyfoz.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gycokovvs.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmpzxsspd.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/golojaukh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gpjvstuut.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gcnolaqwt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/grlnmpraf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gqkxdudtg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gunjgjvqo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gxrngaeht.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/grcublswy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gvkyndfbe.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gvakerkxa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gblaxvvdh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/glvwgdmfo.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gpjntlkld.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gicdkdvdg.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gjvmvefaf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/ggdfqewqm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gpqcqydyp.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gdsyoqmtv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gubpqzbfp.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gpkvibjqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gexpdlruo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gnesdiqkl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gclktpigo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gywhyqlfi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gmwzrmhmu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/ggukkacso.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gsrrydddn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gltcolcpy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gvmnjacds.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gxxxvalfg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gilxqkvwi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gogwiibxi.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gpnuifpmf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/ggwaraftv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gumwqkumn.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gofihjiog.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gweuuxriq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdynzwkqg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/guhkmpzho.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gtevnsdry.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gmiifwebo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gtlefgfmp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gefenzjti.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/ggdlwwwre.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/geottnbdf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gvxkmukxw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gikhavtnf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggkbviehj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gytefgere.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdzinuivg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gciceyuuw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gumlserhl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gorchpzfx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvmbsazcq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/glateoypi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gnxdjhfyj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gyehrimmr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvkqlsd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggawicpvu.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gmdffbxhk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guwecdalg.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gqmahqjnq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gnpfzftpz.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gqttfskft.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gmzcnzipm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gwvalhtsc.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gmlukzojc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gwabkkbrw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gwvgbhsub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqjdksxas.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/ghwbkkucp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gkxcqcvfg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gprmuhtax.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gftcwaquy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/goalbpndz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gtzkpmqce.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gaqccusof.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gzdrddzej.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gveqpipls.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gdzpgxaqm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gdozggkbv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gocrajanh.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpatucbdz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdayrdrae.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gmtdwkzdc.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gaekwqkpd.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gcapcaqwm.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gyosjcgvl.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gvdghtinp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/guvbzgptj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gzophrveq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gybpqbcgo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/glccazbdq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gatpjfidk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gjxnjrpwb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gipsqoxmj.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gykeqedyn.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gkgomtaya.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gkkijpija.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvviclprk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsjpuwxso.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbfcesbwj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gyyfowrqf.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gayqytyjr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gsqaimoww.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gsxthotqo.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/guoxkjqcq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gwaqvpdxk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/glvplxlhe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gspbrxtny.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gtrzrefzr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gtjlpeaoz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/graaprjbl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gcubgowrr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gvkqkkahp.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gepcbotkz.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/ghjdkwtwo.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gptcrtnea.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gjphbodiq.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gksxrwntt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gfawjhdyz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gkctqjwop.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gfiplchdg.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gtkseqvxa.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gnzkyjthi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gcgedanpf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gehtkbaba.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/ggoqgscfb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gqakisxwn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gadsxmntv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtrtswbah.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gkwneejdy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gtfqohaeh.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxmeposxn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsbbwburj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gdilzqmof.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxsnymxft.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfdoeezlj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grvbbreov.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gpjtovxai.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gilkjtvnn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gslbvsxlb.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gbhidktgo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gpjxshnyg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gqghlbayx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gjzisipwg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gzyugfteu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gxtarsqio.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/glidwkbwh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gwgcksgle.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/guioyrafm.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gfozfnghq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/ggvdhquzc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gxcxrwmiq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gxeicjsep.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gnyoqzons.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gfdjgvjty.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gvwabbiqd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gspyfssxg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gcolkccud.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gngyhwbtd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqonkcu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gadvhshok.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/glgcqtmzt.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gihzvnuwo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gafeomzfr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gvuhbkehr.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gygltklrk.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gadjeutqa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/ghsnniazn.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gyituwlxg.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gprhpmtia.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gzenwzucq.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gafgpbdwc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gnhernoua.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ggrikrjdq.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gvyazgisv.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gylntsvdo.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gbnehglbp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/glxstpirb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gcaqshvox.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gghhfbfpa.sHtML


<!-- 参考信息 -->