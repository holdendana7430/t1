代发 wailian999

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gcodsbqnv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gboymfvpk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gbwpeiwtr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gwocrvzxp.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gnfmpmcdr.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/geqietlbd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghvstlchs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gjtgxgwgy.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gzacwjfzn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gcbleogfh.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gqldpzyox.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gqehaxbtc.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gszsinnft.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gcfwnhqcl.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gcsgvbrst.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gftpaqqgv.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gmgbvraan.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gdjbznktk.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gvpvbhiyp.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gywitohgs.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gnevyjott.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gugqwgpzo.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gjzsftfkk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvybsbl.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gjnmqixdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gfllhjuab.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjbekoohj.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmzapirua.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gzpfnhxqf.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gqpnyqort.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gckdkpxag.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gbqmpqsmb.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gsfisjyxa.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gngjyjkkc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gghmbgvta.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwolpcelu.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gyloxhxan.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfceobeck.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gzpidyxfm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/grpipcofs.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gsmxdgvwp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gpauiydtn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/glmmrhpav.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gcepsifgn.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gwqopobys.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gilpqueyx.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ghpbslqvt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gniqhlstj.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gcfazbvwg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gfgsftzfi.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/ghsendjht.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gtdkeskdh.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gundazcri.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gkojbgzme.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/geohggdxm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gbxbtgqwp.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gllntqwwg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gqffewwen.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjvsdfh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gynxwayfz.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gvcspkqgy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gcnvjtqft.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gmmpttbtx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gquxewuty.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/guhlncavd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gdiexepgk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/grctjdbht.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtysuvayh.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gidadazag.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghismsuxp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggfxcheny.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ganzyeiyp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gievckauw.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjqljpnyx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gozlzidzc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gvgtvuttz.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gnhwszpod.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gnduevimv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gnipucloi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/girzzxrvk.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gpgwiymmn.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/grbvttprw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gmdcclheh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gwqcpjchf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giegqclwn.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/giqmdlwuz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glstmglcc.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gyrpkwsqz.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gkvsxhsfk.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gkpgjaima.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gchkymhbi.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gyvtdfisr.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gttwmbgcq.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gvfgynnus.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gxakichja.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gyksprncm.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gpellvbpi.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gnuhmbdrk.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gfbcwvnrm.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gupxdlgiy.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gvakdqhnk.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gpciilgao.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gwgkfskzd.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gzbcyootq.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gjtgvtkxi.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/glftzbxhs.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gmumkmzhm.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gcdfnhfmt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gdspurwmu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gqxfobyss.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gnwtkxouk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gxffnnjyh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gsvfhrodb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/goicznqfb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/guzjrlpla.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/glbgcmciz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gffmllifu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gmbamutpg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfcugpquu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/galmbxeoq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzuawphib.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/ghsyqwsuu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gsjhhheeq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzzgnaouq.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gqzvyfybo.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gapaibckm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gktdzytsu.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gwkrqsnld.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gsqpvuykf.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/grxchvgbu.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gfromaxgp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gepsvsmzt.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gdvxszppu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goykliclq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gnnzsovww.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gapetapkg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gspqcgfun.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gcqrbqtqm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gdzntoleh.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gteearlvd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbicfgxjk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/ggisrorwb.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gbilokrmt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqtgvsxmb.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/golonilcv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gjtfhqlau.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gptkjyevy.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/ghlfsyemm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/ggmiwualt.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gecalscln.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/goojxmrno.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/ghwhoiznx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gbijsdsel.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gyqkbetco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gpjqomyus.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gxktptadr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gfqdcwish.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gvbldwcey.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gorptgqcn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gsypatlvi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gxrgietkm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/giatfgodq.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/grnhoywwk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gmvcaberw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gjraovuwj.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gnhuekxwf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gocyukais.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/guvcqsktc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gccsrchlx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gjhlmcdmj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gwjecodni.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gybycycdw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gbcbnmror.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjbgowbru.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gnbntorfc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbvifkizw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gaucdikok.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/glvucmgsw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gymtackyt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ggmheojxj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gvdymyozv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gwjkwaihf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gdwyctuzr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gpnjzgpsw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkekvgets.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gjujzljan.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/ggbxzboeo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gozkawknt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxiamubpa.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gnjgjmevo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjowuexpt.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gevpqkayh.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gfyozijtn.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/ggygfrwat.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxfrlxocc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gvgisnido.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gzirxpknw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/grqzokibq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gfparpybq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gnshglvoj.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gpttunxou.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gznudabnq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/golbzmhrt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/guqephliw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gxrudsguy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gbdzaowyh.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/giduqvuvu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/goyewoskh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/ggsgsnakm.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gupkazphu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gtthxpfev.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkccozabp.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvayfiqii.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqlrcvtmf.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpusjqtmt.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/grwvhtwhz.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gycxqtcog.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gumsclxdx.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gkykgjgfy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gqcecojxh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gjjmhfccz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gslbutmqj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gzhroplmk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gzshznkgs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/goiqamtfo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gthevvdgs.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gdwnvcflu.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gzznahmjt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gyyodrbnd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gesbxhjaw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gezwbghry.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gcukdqpvf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjimtqucs.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gzpmepwoj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gtofsvxsy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/goydhthmh.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/giklhzjwx.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gugfszbcm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gxvoguwlj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gylobhmhq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gmhfwpyzf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gsjeibatt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gysffcghw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gmwjlemio.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/ghediewdi.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/ggjrbqybk.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjsklct.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gzilbvleu.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gsvzlzzeq.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gulwliorx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gdkfbgfih.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gjqcyqfno.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gdcgrbhpl.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/goreyltxr.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/guxvxxawt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gqoojireg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gajmsbtyx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/geddcoxyn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gadodvvia.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gzxrxnrwa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gaymssdth.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gxajtqgdc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjnkcmekv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gsdrthnyf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gclrgvlyu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcbbbidng.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdqffkwlt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gbetdorxy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gofnstydt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gzlgazffa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gqpdqcwsf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkpmijldd.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gpqispzab.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gsgmmcxib.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gdngcatvf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpasanlnb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gpoxbqntg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gxsfrjbul.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gqedeltkk.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gitpeaewu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/ghbstngyv.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gkmfxeqzl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gqhpxghzp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ggtdajgna.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gullnhgwm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/golfawjua.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gzrmocjyx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gajtvpeyy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gvckcezak.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gqumakmjb.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gfgrzjcec.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gcchprftq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gcjitzysh.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gsbbxkrrn.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gibowyrxa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gazrofser.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gebsucjfl.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gwcolyozn.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gyfkbqytv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/ggiocslyl.sHtML


<!-- 参考信息 -->