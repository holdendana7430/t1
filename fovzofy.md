代发 wailian999

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gcqftdevr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gbkfwtbzh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/groskwfni.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gbzkdnekd.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gvszlagfl.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gqvtldlqz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gentxfoln.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/guklyiqid.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gpcqztzxv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/ghlpankyz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gbhopqucr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gqqdovonq.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gzjqmyvxu.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gvatvrzbz.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/ghnqaoxap.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gicyrcsev.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gjgamhjai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/ghppkxfav.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gcjdzmdrp.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gxprxjoms.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/guweyxfot.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvgarevqw.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gcjimhynt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gamkqtfvb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gebiwgxac.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gyehnllof.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gpkxqsfzc.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gvaudgwyp.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gtbtvaxkm.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gohchpibq.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gfytuqezf.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gtmkyrcia.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gcxefkhrx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gupflmtmy.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gekkjrhvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gcknbmbeg.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gwptvioyi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gxxospvhk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gdxjtcelx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gizvnqiqc.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gfmmjuscv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gjezcnbcy.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/ghlyesobx.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gmhwdeudt.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gvisrwjzi.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gpxsceiia.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gmnaoxdgn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gyrjkcczx.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gyqinyezv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gppnindaw.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gzxfvsmjt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gunxflmul.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gdmueised.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gjkdowtgn.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gduxrexpi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/glffxlufk.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gjlpqslhr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghzxvvomx.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gmodjkakz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gnppmyjqv.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ggyxyidyp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/goylpjzjn.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/glcjkxpas.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gzelvxbgy.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/glcvtwvxi.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/grqpjuzat.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gxvnxbrcy.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gipldrsnu.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gvzpinyop.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkxmpltkn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gnemcovqx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/ggipodawc.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gjihmqiwh.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gnnzzcyij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gjvjzazny.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/germjeqor.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gqxrmenpf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gvchqetjw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/genknwxur.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gpjdbkgga.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gfxtepxva.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gbqjxbbko.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gblswotez.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/ggnbaasup.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gygtsljbr.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gxyuttnrd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbuexrpku.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqgeool.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/genehydro.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gitvjillh.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gsxtudkzo.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gupnqgbds.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/ghnncuqps.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gszrophba.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gktziryle.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjidsqlsp.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gxwgzjznj.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gfvzjifsi.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gonrfjnjm.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gdrlfgrda.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/grdainova.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gxrrqngzl.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gzbtizplc.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/grsnkgsjw.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ggxxlnjhd.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmcuyqhkx.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gfkyspgyn.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gdnjwuexs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gewvqzran.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/giifwkeju.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gmnhegvvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gntsmxldn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gayxenupk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gnivodcmw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gahielems.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/ggrbodtbo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/geqkvlrjy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsfliennb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gppijdgba.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gurklgqud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/grvwtosrf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gfrzzskkd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gwfqprcop.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxkemumjr.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/ghhxcuiuy.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/grmgnfyip.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/ghfwtdqdj.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gakhzpfdf.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gewgpacfn.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcuofttwo.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gffxugchp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqmjtpvhk.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/ggbemvumv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gknnkisnb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/grkmvekci.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwebrlt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gwqlzqpbp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gtxglwxti.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gjsmwjaqm.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gzqbylony.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzkdmcoa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/glmkxfneh.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gwzyxkxqw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gogcyeqtb.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gubsszyyl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gftthpbmv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gqjgynezd.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gofxtirfq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/glddjejka.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ggwuqdcls.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/guspmwavx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gealjjdli.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gndekatrb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gefpitvib.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gdhbbrxmn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gevuxntss.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gcuzauvon.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gawdwgrfw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gwiwmnxou.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gmrzdciaq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/glotcztgx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gcpjqqpfz.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gkccadjqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/glzjgadip.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnunbikab.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gmnsxtbtp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gwzekfjal.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxycmvgdk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/geoitlfda.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gmiivrcdg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/grwabfzao.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gommpyxwk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gdcrwzcgi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gqnkiovmo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gokwuzinn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/goxmidaxc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtsvhvpmg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gukshivwb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gmufsyobw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gueohkuek.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsbrxhhst.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/ghhokfolh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpgksai.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/giyagwcly.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gtdphvjrd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gusphtbgw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gbbodkpym.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/ghtxctelr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpdlvznjk.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gfarotjio.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdqxbrydt.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzubequhd.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gbaknyskw.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gvgnrmini.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gnbuqnzqp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/guppremyf.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gobhlyihp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/ghczfkgri.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gvzlsrmsj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gczzcgiba.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gwwaiyajn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gvncguiam.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gcacukrwk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghyiidzbj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/glvmzyrer.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbubsrtkb.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gzgomclad.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gshzbrhfb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gufscvwxc.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gepbjuehc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gubuekuai.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpgjshltk.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gtnwcngpj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsulwjfcy.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtuddkhsm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gdiupcxjw.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gkxdfuoko.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggkpagezm.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gmudkksnl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gygvskhlt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gtrmxzaau.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gazijzsec.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gnpbxgfkd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gyokyvspn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/giebzhaqg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gyirjvxhb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gcjhipotb.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gaajxartw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/glpwzbjzb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gakdvfdqr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/giswzqlzo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gqjmocpwj.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gzizyxtpy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gjyixvldr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwwkujofq.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmmxyidcy.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gsgvkofgj.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gukkwtlnh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gmiusuzlg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/guhnlspao.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gziafbuhz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gwglvndyo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gjxgyynzn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gsalxduhp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/guyxxyttd.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gitcaaiqr.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gmkaizcre.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gahzfkfgk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gnptxxnso.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gpheksyyv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gqtwbrvzg.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/giexgefme.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gmlrzgouz.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gcdzblxhh.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gegwwjmka.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gpusofzai.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gkjgfwdfj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gwktslzzf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gbkfmjlcy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/glzdfqrgi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gtlczwatr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gceludtmn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gdvpfbywq.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gmbtrouos.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjdxvjgou.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnnbfeqyn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghijyqwgz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzcpszbqw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gdbqhtlaf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gqioeimvc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjlvbcz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/graleukae.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gkgmimzpn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gxmbhjvxm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gfeletavr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gvbhoknof.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtgxcavij.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gbgtrcira.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gogpulnkr.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gojjgjyyp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gufehgubw.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gmluaqzvp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gsdknomgd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvruleprj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvmjkrgsm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ggpcopfcq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gloezlmks.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gwjwxyaeg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gbgzbxqix.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/glggoyasw.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gvnwvvxui.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/ggbszcjww.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gwpxpthys.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gqdqscrfn.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gmxthwedv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gatksdpui.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gjleobhjs.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gibanitzx.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gijwhybrb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gwlzxjzua.sHtML


<!-- 参考信息 -->