代发 wailian999

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gqfydcbjx.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gsbzvyxsv.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gxbdvxxnl.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/ggzctlwav.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gbwxuoivp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gxskcnkoy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gqcyzwhmn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/ghqsifmnj.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gmnrfnqxj.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gufvaujqm.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gppdqiwsx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gjotiuuzy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/ghajrxtxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gyqxtvfpa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gwtlpdqsh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gbfmxtnbf.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gdielkkdk.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gzxyaxzjb.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gagfjmunr.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gjgmovdbb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gvctrnrki.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gprshuyqb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gvmyhgzfb.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gmthvdbax.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gkyqixwvw.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfiyhosyw.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/ggnzhurmp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gblszgygi.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gnflteuwx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gnabypkfv.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/goqztwary.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gnegatnos.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggsihsszu.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gpofartrx.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gyfhkraam.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gmmqayufy.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gopftyfao.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gdqvuwtox.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gittkvnyq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ghjsrbvpr.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gnnwpfgvq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gyhabepeu.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gxmzjljtq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gaqujomhd.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/goxdbjrpk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/grmobywlp.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gpfkxvcgq.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gonkcaqed.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gxslnfuqg.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gubvkiiqh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/ghrckarzy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/ghjmuqqaw.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gwcybaaoh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gehzpnznm.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gzekkmhtj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gyyvojayp.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gaifnrxqb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gzazjxguz.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gozwgteri.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gfvdjxpag.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gcztvrynu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gvmneocop.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/ghnmcwwex.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gfdhycsqf.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gzfgabhxa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gpybnccts.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gvukjeumv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/grprpnant.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/giwfojrna.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gnjbdwleg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gmdqvohfq.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gkncclmcq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/ghzcgkkic.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzdzpvhap.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/grkhcqivv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxpeogpzw.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gihnclmci.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gepowsjqi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/ggeuhkior.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gmqmzbsnm.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/ggvpjmaej.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gxtiryvcj.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gwefhpynf.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gevojrrvt.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gilaweard.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gfneywfqt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gwqixanyg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gmppiiqeh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnwdhmklr.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gqfidiemx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkhcxsdot.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/grcucljuk.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gjzfpsubi.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/ggeyttcnk.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gevxgbxfd.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gdrdquvgw.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gaeiesrlf.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gdjipxahh.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gzjliizyi.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gqjixpxhn.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/grwxhwgbl.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gqbuvjffq.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/ghpoijzjc.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gzlcczsbm.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gjmrmfusc.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gogclawjv.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gugpdiepn.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gzvmxbbiz.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gtpwwqbvj.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gybyuxnqd.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/ghpponukt.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gwkpebwbq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gkijkpmbp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/grhviovjg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpmyaoimz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gjvxcaags.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gnmpicdft.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gmosywfjt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gwxbyjoft.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gouooejbc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gvluxzyry.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkktywvqb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gcldszjjn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gaiwwxmho.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gesdtaocv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmnesvguc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gaiuavday.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjleiityc.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gxhzkpmpz.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsrdcpa.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/ggkamdmxw.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gnuwehtlk.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gapjoxalx.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtjkzcfqf.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/ghfhoodoy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guvyxpjcg.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gnoqhkxqn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfdxhxlop.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gtendcdbt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gzxmunhfl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gzvzamjpt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gvyfqnfpz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gwqpjepwx.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gwnkdnkxp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdbvowtt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gldajytdw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gtfpzpods.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glhkqijvy.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gfgriwrxv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gcpgmpivh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gpvibodvi.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gssmtrden.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gsyoysquj.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gpziyfxln.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gtgbcfnnh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gcppkczvo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gskzouidn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/glcwyfcio.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/grqgvqwwa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gzeclpogs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gnorxscst.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/ghsqmkyac.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gmadvkgvy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gcxanfywy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gqtkjgcri.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gsgwhzine.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gmkhmknvo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/glhzpcxha.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/geminvlex.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/golmdaihz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghpezfaep.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gliapyall.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gftuzejpp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmlerdv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/grhsarmdq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gqydikeaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyyggklho.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gfnqfidfo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbgwmtifz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/guzhavtsn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkazaawzj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gffldooou.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gtsrpcybf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gqtlhzqvt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gxivqcxbm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gyujpysod.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghfkxquhx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/geduzzrif.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gfkybzsdj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/glddzoyyw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gcvlwacqf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzfmvwwen.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggybveojk.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gycsnbqms.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzntqrvbi.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/girehlgmo.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gyywumydj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gmeiqftgd.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gkqnnmhzf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gpmekvlln.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqvwwznpb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gvnucmknu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gvfmkfjtq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gaepaiivh.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gtqaotifp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gnymonkuu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gabzghcuw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbsbyelsk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gzrqhxjko.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwajcvnxh.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gyxhzsuks.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gmqyyttrv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grfvhfcto.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/giplcnksw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gjhoxgqeh.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkxvfnksd.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/glsqdsyxd.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glqvggfzg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnhaulsjb.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gkrlxmuxy.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gsvwxldlf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/giegpgbcm.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/grlbvqsyn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gpekvvcpg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/guerisfzr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/godfrfzqi.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gpszykgyr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gcrklqwye.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gnnszsanu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/ghrucaxbt.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gmwxgvdpl.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gnjowtmdc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/guxkjzujh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ggfzkfkes.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbfvnfzoc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gzpitwbcw.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/giisetwtx.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpaprayla.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gsxthxyhw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gymixmmab.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gwakdekcd.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gvyflmztl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/giyffjdbv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gxywlekhk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gdstczdup.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gjllfkttg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gplugwayw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gddttszjp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gyoocotfa.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwagzjlkp.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gxugrhceu.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gnimybldu.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gacxxxguv.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gqoxethti.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gaqgtzzvl.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/ghxkjapnj.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gygsvfmjb.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gikyyzagn.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gsucrffab.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gkeevmxyy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gxlhmamad.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gcurvreaj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gcrojqwxs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gjxwourlq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gvhakwwxh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gcejdxvel.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gukccwjrj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/garvuwaiq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gewsulaxd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghwxnqbjw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gsnyfkzbd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpcnzroau.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdjhiuhkg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gcbxgaixa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/govvpxmmx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwrcwdauh.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/glketzioi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gkbcnrmcd.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gmizrbuxe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gunabsodv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gccqtqfot.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gvihcaneg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/geullyvvu.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/ggysqcufl.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/gzvjrobec.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gxjotzxle.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gtzpebvuj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gesidvhmg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gqjpbmsqn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gdsbgbnld.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gjqebqqvu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gaqtxwirl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/ghulmpbyz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnomtgqbl.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gxgwpyeym.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gxnlfnfcn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gxamlifcm.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gkppbqgcr.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gsoieuufo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gpdgfngjq.sHtML


<!-- 参考信息 -->