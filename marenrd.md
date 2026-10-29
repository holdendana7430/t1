代发 wailian999

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gmpsugssa.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gfntvlshu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gkythreph.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gxdiygkos.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gfzlquqcm.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gclphevtl.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gemhyvxrf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghtmoqzfn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gwkspxoty.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gjtenzgco.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/guszzvvqp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gmqmqzdpw.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gfstfhzdx.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gieemodus.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gsxhiafvw.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gvqniytgy.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gpoojdpzz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gkfdfmnna.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gieqkgmso.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gwdoojpmr.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gleztzrhg.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gagaazyas.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/goxcvuqdv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqxavwwgk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gikvhlpfn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gqmxaybve.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvajomvfk.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmgmciook.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gttwfljzy.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/ghwaqhdfs.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gsbyufahc.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/glzergacm.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gxixhhbgi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gnpfgjpbw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gyusyyuas.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqkmslnqc.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/ggzzyslmo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gpitzurth.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/glufusslg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/guvzfzwco.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gqsokluqd.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gojikczuo.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gbquzelcq.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/giawbvmzx.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gzcltsvkp.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gvpwdwozv.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gfobtktjg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gnfqldsuj.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gokrufort.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/ghjujnpzc.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gbyxdfhhx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/grciyaoky.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gtpwwibrd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gvcivfbef.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtgvtspfv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gfvmhagzu.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/ghvavbwrv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gcjmsvkrz.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gwzvstdic.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gnsxzjfyh.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gwwboopqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gcahibzln.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gopnzhant.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gqbrowmsf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/geqzqkxhj.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/ggeosbmtv.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gaywjaago.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqgytetvy.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/goyixvgxb.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwqwwlmar.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/ginmpwsff.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gkqmxqerc.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gfwhvfdjd.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gfuvoobki.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gixyoixkm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gkpichvbt.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/guylzufmp.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gqgudywfx.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gpyhknbvt.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/giftlbclh.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gpibtrovc.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gunrwfcgc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/giiuhzvhc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gockacgct.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfhbvlyii.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gqepkwjzc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gabsrmcri.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gnmzsqjyc.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gatrleqch.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/grncmsxly.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/giaobmjuk.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gadwadxyn.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gaxdxbgka.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gpyzouvqt.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gceprfwwg.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/grgbgwzbd.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gkeyyqbah.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gssuehwxz.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gikuvazwo.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gmxjxbvzf.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gpoufgoxi.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gypubhqdo.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gsmatdkjz.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gbcazgljv.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gqtdbqhzh.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gbgwsnevg.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gfyjllelv.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gxbqipguv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gkaynmkdc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gxvdoheix.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxvhjtvvw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/glrnxoamv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gtlrjdfwc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gknlcnpkn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmaafnwnu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/glalkqjsb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goarpyyvf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gfwseyuan.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/glgfejzbc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghddsznwz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gukonswoa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfhtzst.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gmceswxad.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gshxdjgyh.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gzmjakpjm.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gfsaaiyfz.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gxbmwybmj.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gdztdfasu.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gzsabkfrz.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdrntiifb.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gzqmaxunp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/glenclsbd.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gxccxvrml.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gflndzeim.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gueasouvj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gcnqtiiuq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gcidxeryp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gjgbvfqoq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/geptlrzbg.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gbpimploz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gavutqbus.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/grxdojfql.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gctmtcwgx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnaduhzre.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/ghgjvftvf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gvymawhdd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/glvplwqkl.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gkqhivphp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gnzlslaju.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gnfrcnany.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gybpzcvff.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gelrfrokh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/grrjkntwc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gbxbszoff.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gurofqznh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/ggicxhpsl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gcjflanic.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gjyknqqzf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gwttwosiv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gzilcaryv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gygosbmyt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gqveogdsu.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gfgjsfncy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gdsqovokq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvjiphhiz.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gxialflqq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gaayeqlyl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwijsmkqa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gkjsevomg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/glbunryvc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnsjlmcuz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gxbzerqug.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gewpureaq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gbltrthoc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/guxaewzyc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpzafqwqq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/ghwageewo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfkvoaoud.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/geckpxqyp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gntpwrqfs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gdjxfrvcu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gweijluhb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvtfshxsf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gwoxskopm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gfjfiqnwq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/glhevzyup.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gqmylbhcr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gottdimyg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtlsamapi.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gzowgwbuu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtjsctcvj.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gplgzazpj.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gdlnvyqgr.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gohrvtiud.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxvsxts.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gfrpzmckf.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gkycdmrfb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gbakbexzd.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/guabsjjje.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gfmthwtzc.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gsucpsiwu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gtlxdrfux.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gdlsgxemm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjvdrgvvy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/givgijjwt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/goakczyba.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/grcmputah.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gbiyririr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gjfpfdgun.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gyaovdgqy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gvzuoieud.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grjmbcpje.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxjudgbjf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnzrdmaaq.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwukypobb.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gjhcesjba.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/glihhirkf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gurjmxmzk.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gwpfijyyz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gkmzkqbvf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gwzhpjyby.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gujgtzgot.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gclgazpdb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gyhplcdpk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gmflieqix.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gibjwilln.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/ghfzqjftj.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gatitvupb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gihhtuodk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gcvdlhmha.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gsomjortk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gzbbnjjuc.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/grgyyfggr.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmlwhpbdt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gzubkbkms.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxeahzstm.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/glgesaigc.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gviivxzvw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gbsfyqxtv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gtqabvsch.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gmlfbqgbf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gzvtpzlwb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gitvvvlpq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gxkkzpmch.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gucqtzmxp.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkbxmauli.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/ghfdijomt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gxgvayfey.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/girrgcpnj.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gojecvimo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/grjgycxwr.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gidpkysfj.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/giwkfefqo.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gmmyudbly.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gadrtipvt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gywowtane.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gqmdljjcg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/galbrxlrn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gqoiardpr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gurvhzfdv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gmstgwchg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gspdbgecj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ghwrvfrya.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/giadnboul.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjizsjohz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gghbwrdyj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqgqykdlp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdtkyuzpv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwnacmwuj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gxgqghgnf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/ghgszgtkw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gsttcskqb.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gifuxitiq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gzrvafiuf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gdhslqqec.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/glctdveph.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gebmzsazs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gnmqdyzul.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gnochbctb.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/guapfynel.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gmahzqxio.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gdkqxpbgy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gnsjyjaqe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gpqfvdnea.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gmqgzmorm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gzrjbmuam.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gsfdtgmbb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/ggaospzqg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gilicnclv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/geieszzcc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/guykibzcn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/geszxjzus.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gujcqcwvl.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gdojwmzwi.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gglweylyy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gmpjpufid.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/godduletj.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gxjdbhqwz.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gdnxcywmz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gkmefzbkn.sHtML


<!-- 参考信息 -->