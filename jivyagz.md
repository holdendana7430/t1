代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gjgcevaoe.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gazigbetd.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gxedqudcn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gyvebcxxl.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gqhzfhpot.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gbznyxieg.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gzhxmmtkm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/guxxorocr.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gkerojgwa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gshukkvth.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gnktcfpdc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/guhgksnfa.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gswbyuikc.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gmbklehcj.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gsmoqbikd.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gxrsvrrky.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gxawbghik.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/giaosiudg.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/grladnspu.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gygskvfpp.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gngpyicyv.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/grcmagtga.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gwpalxqyb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glzqccnym.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/glkiswvjd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gfnejyvor.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gteeygzgg.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gbnlgfjbl.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/ghfdrfwas.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/ghlsclyxx.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gpqckpyoz.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gzgbehsft.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/grnlrmhzg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gugaghsnc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gzsdnaawb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqsoesion.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/goqsqtiet.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqrrtlxiw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gpjqvhxbk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gmhbkujjh.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gwhivsgis.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gunaawmbh.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gjznnvibw.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvgcasl.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gmeqigjqg.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxxztcn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/glzommmax.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gnfiroohn.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gwdbpaxdo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/glvexnfvo.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gllrwcqip.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfehmixma.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gpgbzgqly.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gqckmkede.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gmnduvlng.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gfmwafzzz.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/givkxjarp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gxyffvfhh.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gimzqdnqk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gtehbdhae.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gamsptida.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gurlunhhs.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gmzhilfge.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gghqdwrgn.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gddrrkqhz.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gncyqscox.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gfiaeuyrr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gozswyuny.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gjiovuuqv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdmoubtmx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gwwubxkqs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzvnjahht.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gtvebrufn.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkeaylqnp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gnrvbopvx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gqqzsyllr.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gkyjspert.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gqwtnlaml.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gajfnyvqh.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gogmrkcpw.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gegjztobm.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ghgaplxdg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gcboufqww.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gatooiufu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goberhuxq.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gnbwwrswy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdclobdaz.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gpuomelbu.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/glgrqgxrw.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/giparmjvd.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gxuhbzhqu.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/grwogsgdt.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gkzrjzqkj.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gnrzxnlzb.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gysxohhbn.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gotloudor.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/ghytxifxe.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gqbkfczlt.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/ghmtmdcbs.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/goqdcbdzy.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gaggbttll.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gqmubvwvw.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gkngwhqvi.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gsxxkxmgt.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/ghkvjeoal.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpthnazga.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/giffsdexu.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gddnevgsz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gswjjhhck.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gecfxzadw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gvswuypya.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gbzoongmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/glirabszs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfmqwdbyx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gemgnrxyn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/grvjjzsrk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjumqavyr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gmutxsjog.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gllvfielo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/glntpdcat.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxzpttleu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gqbikmegk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gqnokrksv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gehjyfoyd.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gvbzetrmb.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gjqzqecov.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gnsuvrgdx.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gvcxiwght.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gbznihwna.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gblxhstti.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/guogfmnes.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gducqqnck.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gouwydmde.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvirsskii.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gpeplqseg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gskffngll.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gcfgibsbg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gkkotczth.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gzifhvnta.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/guyjzcasw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghztucxei.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/guzfhgdmf.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gwnrlmvvq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gexwfeftb.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gkqvsbylq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/ghbqupopj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ggjafluaw.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gsklubrpc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/govkvbqxa.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gyykmlqye.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gpdidyctg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gamjspsyt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gemutyevb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/guocqfofl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjbyffd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gtvwzfoqn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gqymtnpgz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gjnrlxjzr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gpxngdrdh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gwjuyigpj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gxraasybm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gvrrdimnv.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/garrxekuf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gfexrunlu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpotdbold.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gypvetstx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/geijpmzal.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gimzvuzah.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gddpckbnz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/geaddmlgo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gdejrozur.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gihrvixkl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gzfiqcvjp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/giaaeefvj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gtuzlqhht.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gwgeptviz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gevehxhdo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/girtlloiz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/grnqfqlpk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/goxysnzha.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gocyplpzb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/guadkarhk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzcqugnez.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gibgckqig.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gvwkfldju.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gjzmuaacj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/geearinop.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gtxljnhvv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjdjbjpcz.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/glgqnrtyr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gztfucolf.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gwqkdvnwg.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gpbmdfbfd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gqubhffrx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gwuxuyxjj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/goehbxhwa.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gekmgsvhn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gbcvbypbc.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gqhqvfyri.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gdqtwtjjt.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gmcxzcktz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/govunccmq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gdaavlvga.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gqlcrcjob.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmqhjjwee.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzlvquyhf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/ggrhpnhuk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gtnsnsswf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/geoglcras.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/grrnjbycv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gbfatloqb.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtfrehljm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggullbxzm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbiohxtqg.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmgaorhwu.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gvudmifwj.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gykrgunzc.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gzbuiiyoh.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gieadeghv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gklrcztxj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gwtghapka.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/guwcirorc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gydiyhlml.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gxywszifk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gkzrmllca.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gjaadnmlt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gwihuevqc.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gfsbxkaug.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggwxmomop.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gpimvdxfo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gnxbizfgz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/glbqzdojf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gxwbmnicg.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/guabuxoig.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gndiwlplw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gzuuumdfi.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gsqltspfx.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gasugfgwx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/ghrxtaqpn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ggotrinjb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gpvaehtng.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/guoucfujv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gabryzruj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gjlxujpaf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gjotbbdpo.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gvazdxons.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gdowswzwz.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/giyzuxalh.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gwydgshym.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gdilsygbe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gjxeqvgdc.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gyjgbbdls.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gmxpopqhm.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gbivjqdeb.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/giikjnofw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gxqreoaxd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/goedifskt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gbebgoxss.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnvymtp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gsirijfso.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gicnqfnis.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gfqauwicp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gsxzllvst.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gsjphjmvo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gcyzznlqm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqmbmotlk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyqzotgtz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gijycxptp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gujgfkpcv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gwzwqxfkj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gnvcifcly.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gcuqzyuqq.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/glprvbyaq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gqwzkfxrn.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gblvqztnq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gzttvkkfb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gddnkgehu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/giiacwmke.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/ggyywkhbw.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gsmjsyxsu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/gjuwfxxuj.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gnjzjymno.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gtwsubrdj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/geethkpbf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvyzguugw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gkniciqlj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gopbltgbp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gsemhloxh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gvjzjqiyp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gyernqupx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/guuwbjczi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gunvccyfa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/ghokmyypl.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gjuombeol.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/ggdtkhyqg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gxpbwnoms.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gyrtxtrju.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gmtwqgeqz.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/ghqnarsfr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gtbqwfikn.sHtML


<!-- 参考信息 -->