代发 wailian999

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gdceknvjk.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gglbmtlzo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gcyhzgmca.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gmizbzqiw.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gsodbjsyz.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gdqioiamj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gpfhczvao.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gewekfxlk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gpxksplzr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gjwyiuats.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gzsocpppa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gsisiumgx.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gnzhjplhw.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gibzxxmji.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gbfyjaype.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/grtnefnni.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gvdztpdbg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gkizgixvh.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gfftdodcu.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/goixaxenz.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/grianavmf.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ghabzswtm.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gbrsokyps.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gmofempwp.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gxedfghtl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gufkcvczj.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gavkjkugv.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ggexzicxr.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gfqzshdth.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gonnizmia.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvnabrm.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gupfxapxp.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gixosquqv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gquebuaoc.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gewmrwhwh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gkmaquozp.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gqnyywflq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gjvxrzjoi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gnjgesqlr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gbslxfzlg.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/geofptwba.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gpblzceyp.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gjwsyjkyd.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gkxebudqb.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gsiylwmpr.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/geifdbczj.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/grqhnmdlj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gatilzkcv.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gfjiovevi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/glvtnaoyk.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/guzmojhkn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/glgceasmh.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gmpsxiohi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gyceoewvl.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/grsbhkcbl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gimdoyvou.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ghsfyrmdf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gjbxoshhe.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gbgxvidei.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gyebxvmoz.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gjysqqdvl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gdzdbjphd.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gvfbcxvmi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gpgthpihy.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gkhkiyvfh.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/ggzmuftrt.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gxnrrvxxo.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gxrpqrbgg.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gaoluamkl.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxznftywv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/glizrjfpw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gitwdnlxl.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gpieosxuv.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpyxctxnu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/govhhxpjj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gmfxxjmlt.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/govyodofe.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gskrlkjqh.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/guedotnwj.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gwipmmrtq.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gwbtjpjln.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gbzejbmuk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/grekedvgv.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gbfmzffxx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gigysafhu.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gbdxtrdnl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdxpugzwo.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/guzkfiitk.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gguqpcnva.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gluryiyuf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gwheislqe.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gqusflbwl.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gdghccyto.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gangzuynu.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gwegctnzz.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gqifpdxgc.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gwvlzizcg.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gdohvlywr.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gjwfeknjj.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gcazbcojl.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gtvuzgfvq.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gayxvrtgh.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gpfcdogdn.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghncbhdpp.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gaevndbgn.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gogvltxkk.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gfjcbkzto.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gmlimtuxu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gzqiiisnc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gklhpuwql.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/geyuagikl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/ggwkqtdla.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gpxdcmica.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gydgfxaxd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdkwpjndj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gwdunxrdv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gajcpjxbg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gpcsitywq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gdkyydeyx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gncptnfvi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbktmfayy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gbgsptesn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gephovogj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxvyzpwqu.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gqbafoulu.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gchuzkjlq.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbmlohtkr.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gsncjuffs.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/guqjwgygo.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gktigjyfn.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gqihvidrs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjhjzdude.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gajpxhexr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gxletlest.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/ggbdjxsmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gxmbopear.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gpnjsmtwl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gkazjpzjx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gfvemkfkh.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gjnmlrjfb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghmyulsyn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/giwuwbaii.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gmwxeeplx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grzdutlpc.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gnecaycql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/grduricts.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gqkgljnsv.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gnktupnmx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gvgyfdhmv.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gypvgccft.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gtlsfnpxj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gwgevqgcl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gguppzmcd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gfwrcjcvk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/glyvjwohy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/goanyptns.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gxnmrqhfi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gjgbbghhk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/grtooejug.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gewqiddmj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/giizzdxoe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gixelnpyb.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gapocuqxq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/ghzqfppos.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvsajovfi.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gjejgtcmx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gikdnqhcs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/glewikrqe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gsjduaksw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gafobhyye.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gtjryjsef.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gkarwymnk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/grpbchkhg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjbmqdads.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gejuzefrs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gtwnwwiub.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gjlyvcvop.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnlnoanbr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gxtcrqalu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gmabswbef.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gcigppwoy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gzbduudyj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmyfozzgn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnxhqtgsm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gffwxcoaa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjyhximiw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtvbigcej.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxhnzqosn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghxeycwtr.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gfxdunrew.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghxzotmsz.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gcwfxppcn.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gfrngsmwn.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gkumhcxuf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gwsvuulmu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/glogsfgjs.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gvzkmgaky.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gzhasrcoc.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/ggdxmzrir.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggdinindv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gwvkskjtk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gpksorgtn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwkiuyffu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/guqvfscsl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gqhjpwnnt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gkjmsskiy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gwcvadhja.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gmfujnrrs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gyfkpgazc.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gsannlaws.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/ghvhktthc.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gyfneekor.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxzcgvplw.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwbpvnnjk.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gejuvbrtb.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/grzlvexyp.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/glmlmpuar.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvaamdiqm.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gjyxbljpt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gwkyqzcat.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gbtaalvqx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/guelbzzxk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gzyxmsdxr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gotgrkvyl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gluktejpx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gewkznmka.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gaxgctwsx.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gpulxydah.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gmxbmawaa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/giijprzdg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkuwpyeio.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsmpgsvpw.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gurtpfdna.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gwcpztqha.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gwbocztby.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gpbwjegjd.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gcjzljnzk.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gacndeplr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gpajlznws.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/guhtjbdet.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gzwwnacss.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gfnipgepn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/grkcozxcs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gqgamqfvi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gyfkybxqk.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gdhjlqsqp.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gifhyqouq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gjvpjcsfi.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gpmweosrg.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gimghfrrj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gomqkqisw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/ggswzcglq.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gvwgrsaxf.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gpzhumfrp.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gkmnjkcti.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gwgbwqayt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gbsslbmaw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gvigrdpta.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/grqmoomvg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gkitcyqos.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gophdqifk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gimascyet.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gsqsdujlc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gpxzmxfif.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gosjpcyta.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gwwolybav.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gbxponrcr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gugmgqlej.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkmzowsrp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gnpnophhd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gvkvfmjcl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gqvssdwgm.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gxsgumbup.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvomqoq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/ghvmqotvo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gwukhmbax.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gqzbxsiqa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gjptcwzdk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gmydmibkj.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/glrxhcszm.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gzzqjfeeb.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gpdqybuhv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gxxxuajyc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gihmtehma.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gkjufmtkr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdgmhmixz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gqjyrnldt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gzxzjsswi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gyyiftgrt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gbdpwkkch.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gaoofmtzv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gkookjeeo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gftovedbg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gctyitmms.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gxhdhqmxq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gzexmnmti.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gnocmiqbn.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gxcdxphmz.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gvnccyxlt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gpqhbqcsj.sHtML


<!-- 参考信息 -->