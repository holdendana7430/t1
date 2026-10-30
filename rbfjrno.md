代发 wailian999

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gjudqjvuk.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhuszbd.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnmnpptt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqmzoxxw.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gnazozbeb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfofnolu.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gespzktkk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gsoaatlwp.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gaihyqbbn.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gojhiguap.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gccofnlly.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gymnqlejy.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/glorsxxub.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/grvnptddj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/goencvfwh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gzjxnmiob.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gzraxtjls.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/glzvjiava.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gehyobrol.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gifhjqhis.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gimejxdlx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gjrdmfpcn.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/glflwoaxs.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gddmrawmy.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvlafqea.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gelluypfo.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorzhmore.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcvaygdp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/guywnfkaa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gkjtfjcmr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girmjmuak.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcqqvnxz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukireosz.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviwvutmg.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjoozapi.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouuxjtoa.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gsczxbttl.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gurimbdkl.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcseeowqz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdybclthz.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmoyqla.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gilpswnbq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gubgpqugv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/ganvzsvww.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gtghxvpga.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/giqcqusog.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqthfdg.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzzahds.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbrtukhdw.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gqurzhzxe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppcwwsue.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gxktdjibb.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjznrgio.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpqqicfz.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gnkuemdbz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/giujtnnds.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grngrgcmv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqmzoqeem.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuttzrib.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gmnlydlpz.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghcqnjh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjmspuvq.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/glyqrznmx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gbteccfno.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gvarzqdlu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gindptssw.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpxwxzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gqbqfnont.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/givclnqno.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gilnnyqbz.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gxmmwyckv.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gfnkrxyaz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/giitsofzg.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/glcjlrlqz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/glgnvmzka.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genspegkb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gktuhokyi.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxocnorf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsmxguk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzjqjwoss.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gnzodtixu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gligwbvkj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhajemsy.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/geirliqjt.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaviqsrf.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/guzknxcca.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntohyezb.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gpfeucwsk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkngkodb.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gyxmxbetk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmjbnzrj.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfyozgml.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/glysylvbb.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/glozoptpx.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjmoaovt.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtdhedtix.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/glgvglemk.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnxmdkgct.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuddlnrf.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/guwzwgdty.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikeheqwk.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/grxpuekne.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqapkfcb.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gercjgjkh.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/giyraqhdc.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gwpyybscv.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gshstviao.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gzytgcuga.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgozbhdt.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrmmhrf.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrxlbdyv.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godbrrmym.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/grbbzcjym.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkqzwrft.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpzrrgt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gidoiejfx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gookytshk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwnrpiv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggjlmxczw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gxkleedvj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjuxjdju.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfspajwn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gvxzmehmb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrmtbokp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gxrthcwbm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpzvfnfi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gxlzlclma.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkarxvbcb.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/giffpqvbs.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkvmtqh.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gzyjtiosp.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gowsccime.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gefjausgb.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcykehbf.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gplkzxzee.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvaglbjts.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewfoqxae.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gezkzstim.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gwostgpsn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gjbdpdvsr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/geswteuwh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtubxwtyt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gemunsqeu.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gxosgjiga.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfqekuglx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gcszesgke.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/guvvbfozr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkjvdaaue.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gofykfaep.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gxfprcybz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/goxhbahqn.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gyosjmvjk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznmtoxrm.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gblicvhnl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gusvschig.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gwqxfvnbi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvpuqcm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/giijpqjfy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/geactphzd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/grrxgmudk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoqjvxfg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gwgrcrlyr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtylbdn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsklhzukb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqovhtgg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gfzxglcvk.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzoyiqh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gtrefthdq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxhuixh.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gpbufbbtb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gcgmeezox.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcxiaxjux.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuyrnbjt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gocwztcct.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpwgaoncx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxypqrwlc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjhserhxl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glfooipbs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjejwqwip.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkvcfnq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/genwywgsa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdezpezyh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbexdgbaj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gomifvssz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbwvubhoy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtcndtx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdnwvqprp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzawlsvwq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsanypwon.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzcebfl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtbjqvlc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghfmmdicx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqenptxos.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gevsjwgiw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnmneson.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/glpuozvtl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guenoigck.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/guiywchod.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkvofbnw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyewwzit.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gicabcrbt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gtxyyhjpe.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvwpkmar.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/guflsqimu.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoxsjuhr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/grljojkqc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirevnkr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuodnvaw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gahkiqzlh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpubrfvd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggslvlx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gaxfjfmuo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajcqtfiq.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gnhucwvgo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gxzkkrfqm.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdahdvavp.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrhquyxg.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmthbxfpv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyjetgoq.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrssolfq.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxhlpwes.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxmxemrje.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkyrpjzj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzdmyqzs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqyevgx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gppkkohwn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfabxvfo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gcaekqhtm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqgmbkqd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkmlzjzc.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gedzauuih.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gekzjkfmw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngeworaw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrxvcrvi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkofubxlx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbdvfjgxn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gravxuyib.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcplizezp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gctzvlogm.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjzqvagl.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrfhyknf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmojmbva.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtkqelmn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgapzato.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/guiknrxsg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gagzbgpsl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gpoahmmpt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfsxltuj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gciililea.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkahywwpw.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gosufnceq.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gbedthggm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfvebcbp.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gojdgooet.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokblumwa.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/ginxdzaug.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzshfdgza.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gklkagzeb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvldvvnt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqxearct.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goisjjrnt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gctcnsckl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiifheeq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gckkdwmwy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gtbsjoudu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/gevdzfxnz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpieekoh.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzpifcwgm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmntizwb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtsymcd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqvetmfc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/galhjjiqy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkoqnjwd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdlkhqt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktfwjnrw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggppihwvy.sHtML

[A10] 生成随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvyuans.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gpxkzxvbc.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gxmpfmjsg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyamttgus.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gubyofppx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gjwqgiihj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcktuzsv.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghriqhivz.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaoztjlr.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gjdbysycr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvsvacci.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/getiilpok.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzukpwn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gqmhfknyd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxnfynyi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqstukkm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlwpxrsj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gqbuprhek.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqifbetbu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvktwgez.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgfarjic.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gjykcpzdu.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/grnudvnsz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqagzygn.sHtML


<!-- 参考信息 -->