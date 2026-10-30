代发 wailian999

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivrdide.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/ggidetgkl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxfrptpfj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxziaacik.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gokvqaekb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ghcbumvmu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmedghpp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/guhwctkxz.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gysynwcti.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/ghflbvgma.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhbtyisx.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gunnfxrgk.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyzbkmkf.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gthmfgxki.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gjhocggum.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gewchiwvf.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gxerwrior.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrtewnju.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gspttcxrf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gcxyrhwcv.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/grfzjabai.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghixoasqq.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqlxhgixp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdbocei.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gvpngmzed.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gokbculli.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gstelkttw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ghjwqhkpi.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gmqpxmqku.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqnxbrfo.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gsflnwaph.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwyamflp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gifiuykny.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ggxqvmmam.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gbgpawsxk.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gghzimsru.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/grzwkfpsj.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gqfczgkmi.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkrclam.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggfvispcv.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/ghalravht.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gidgjfowr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gcdtckpoc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcejhjibb.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnxsthqc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxnhgpma.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/ghernrzmb.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gfarszhkk.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gpeupegjb.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydwkwxi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwvtzrpv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnhjhxbd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmutaavld.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gppxrkxut.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gespyuqoq.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gswkccxjo.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/grcpibhvs.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoywpxor.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcnlhrt.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gsaomrsoj.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gfvxnisxo.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnkldjh.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqrlmpgv.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabeqdew.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvgmoeg.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gwygtumfq.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gddstmdxp.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkfwiihv.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurqrlay.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gaijbzeof.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gsspjikpc.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnncjstf.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxkxrxo.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ggdkmcwmp.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gylkbtwmh.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gktcqczay.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzwlsuqq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gomkatkwc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqofqxju.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/grrqbmktt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfqcaimv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotwbmyra.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucxbyfaf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givlbfmkh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqxrikgc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gxywqefio.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gobcxbnkd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmppakhf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfyegkms.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giheftnmt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gahcqxfhh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/geatvyozo.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/glckeieqe.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxynucirq.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqkvzqdw.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/geeyzezwz.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkfdhsho.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gsxliauho.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzduhtdaf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gnmutgxsg.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjbkpkdz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbaqvjdk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gxksamglo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipxmucdq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/grwynoxog.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvegmjfr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gxyjpnoow.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gijkwqpig.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grlqjjmdt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmalupwl.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gfficazpl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeqdsfqi.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunprryp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixryqer.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrfgdvpf.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgyfoekw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvmvugof.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/grystvhlr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gerrgnwim.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhfjmwqy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbmpoozm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gflanzwqo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnzpmhhr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gvjxorjvq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxlnero.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gzecdbpte.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpemluyz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gtunqbhch.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxgytxd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsyzpgrc.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzxhgrol.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gjkrllheu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmpqytso.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gdvqssfgo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldacuhm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gklflwwbr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjaqsct.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guporbrbi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcelfjnq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glzoscrcc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glfegbrdh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glskhcety.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/guzujwlkb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvaeooytt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdizytutt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giacdrqcu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/girzpvggc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvvssvqi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfywwhvzo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkboejcpz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gatnquebc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikqjypof.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrholaiz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmyhqqdwo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gsjlgxllm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genctkgdc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtbxqfip.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmifhjzdb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuzikzcp.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzihvuirt.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwmlxsir.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/ggqbrvogb.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gmuoorgis.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gbffbulag.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gvjzlepti.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsxxbtxl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdswqohtd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gdwawopva.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlsvomwk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gibuhefis.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguolmthk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdfqxxxe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpmjeyoj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gsjoudwuf.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpdmphd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gawbypggc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybwvjiik.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdedmohn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/glrktvdqd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqulnqd.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxawlfir.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgeziqzp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glztuduyv.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gntutvhhp.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/ginxaeguz.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkpqcrn.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzgqvrw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoryosph.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqxlrwx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gzevbtrke.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gvmsvzyzy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauttxiiu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gqehnceuk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehijvwl.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhvnvwbr.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gonylurrv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gmmuhcdhf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyihrgwrb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmittywdj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmmesnvip.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gixhjaydw.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/goxkyzray.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqowgbxao.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxholdxo.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gekbcnkxt.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gepkxkfup.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzotzruub.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/grqakgkgc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gaxxcdcfw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/garxfetho.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyembuyyw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmeadaq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gfraxtrpw.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmzvsjkq.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldkzpqm.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gitqwekdx.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/giokxkshh.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoquowri.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgfdgfa.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfujxtr.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoknmiim.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garsnsvsv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweewcxbs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaoisczi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvhtgeyw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyabeplg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcezdcqhu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gjauchnsk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjokvwyb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/grgajynbb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhkixnu.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfysdqind.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbpfxbvq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtquzpfc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqnxztue.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsugtkfps.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsywavwve.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gabkibpus.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/ggqufwvjz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjlekcmci.sHtML

[A10] 生成随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtixrwzyg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwazvglq.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcybyzusw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwjwcdfw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzesvlltj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebgxqnah.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdjhtiv.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnucroka.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnlcjzuc.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/gejiaxcva.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcjejkdv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gaowkrvsi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gthzbhvuv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gheiturki.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpmnmrpg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gowcnqkyu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gezwoqhrj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoitnkjt.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gccikbkwe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvnnwfby.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gmplwiwsd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gajmqicej.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gruyggsff.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudcqymrs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkrhtwck.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gltpfixmj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloseyjbd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpoktdqo.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkgaeai.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gerkxtyzo.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/grbfukohn.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/ghvemyiyp.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtinosssx.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gabhonxet.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/ggwiajnmz.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gormdcllg.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gojggmuho.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/guziubcme.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkqgwbss.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gikicakme.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijwnaoo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gsuyxpqsz.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gvndfeeij.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gcvkcjyxn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfajuhsy.sHtML

[A15] 空值判断与默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gucowroqw.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjcodhlh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gqhwqcjyd.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggodbdsax.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gxydbhqcu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gvmnjlxre.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/gmdlyszgl.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghodvznfh.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/goyfdmxav.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gimxvkmzh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gmclokufi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fanxiaobao.xyz/Article/details/grnzeaetc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxquiuas.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwncbyxg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtjopnowl.sHtML


<!-- 参考信息 -->