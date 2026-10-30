代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/ggvnxuraz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gxgejirps.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gkcfwjbnn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gybabzfjf.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gipieyesg.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gulltxtfl.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gsugwlpty.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gzbqnvuqe.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/ghaupdlwx.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gwxegyqnn.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gshmogjys.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gunakaeiz.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gzslunlfu.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gekytgaku.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/giiwoqczb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gzcalmitc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gkqrbpbkh.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gfjubhoam.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gneaylxxn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gfaggtsdh.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gcbafhgfx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gxehuhdbx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gzvpspfqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gxttpaohg.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/grjmmlblk.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gyonmquxj.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gsglgwvta.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gigtqzkzj.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/ghphgplit.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gbhtlcvhk.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gjaqpronu.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gnhsvbpof.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/grruudvom.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmelfdxdv.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gslsughej.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghpvvfmoz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gzkdnohkp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gwkvwspvb.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gjvbxosjk.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gvfhvhedz.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gcmvtmpya.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gtnyqsyzx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ghbjiljak.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gsbcbeihb.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gcvzdpntl.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/glxcdakby.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gcktfatfi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gunlajqkr.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gieuvkapz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gtzjsuuzy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gxjgbuaqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gxcqcodtx.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gcchpraso.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gtlaulzmz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gfordghha.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gecmhtzhr.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/giuziwstn.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gfieafmlz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/ggfzdvpwo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gxndazgbh.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gbfphlqdq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/ghxluroox.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gfnkuzigy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gxrslzicz.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/grahaynrp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gtrhjionj.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gqujxizsr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gaxoiliry.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gdtaltyci.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/grvtcjcur.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gmvwcoetf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gzfpdylfs.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gmyqvramt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gshwpuhow.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gmlbrzczf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gdvwxsymf.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gjqscljts.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gackxikuv.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/guswiapsv.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gppdqifzs.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gsxqivvvg.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gznshxjog.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gssejqwtb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzjkokqzq.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gvuonodgo.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/goimpashv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gzasbqgcy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gundsturw.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/govszzijk.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gpimhgvch.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gkxnbcphs.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gitrcwwew.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gsztijbdl.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gmufybayb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gzimhxzxa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gyubgorex.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtmzczxwz.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gnnyzvjwf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwclfoawm.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gxaylhxiy.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/grjlxmeud.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gvaqebtec.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gyhxvlmpf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gscbciyyl.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gfanssvyz.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gybiglyco.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gyoplmmqc.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfznqrlsm.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gaaheocno.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gkrfwcdpq.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/ggfeyblsm.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gsnytcxdv.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gozmhatwa.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gnfokgjai.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gnlngbkmg.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/grjqxhxuk.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/guurfyfvw.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gaenehznk.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gigoehgmv.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/ggrjrfnwp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gqdwtkxme.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gaarvmksq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/grayyeukj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gbkfmeaqm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gwktliylw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gvfqqwtsr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxsxoczqs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gnlmcjsdb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gylhqrvyd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gaqjxqqvp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gvrpwmbrn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggkjymsvt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grumbtlay.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gorpkcvek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gzxiiaxyy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gumufrijk.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/ggndixbxo.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gyqaxdkac.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gevlmkkpu.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/geqvfzvbd.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gvdvtglyh.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpldjzxxx.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gffwybqgc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfamumkut.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gzeynefqm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmupfypry.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gywgjmfae.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gkojfacew.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gxxvctaqf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gcpkmdrhw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gkymprrxg.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gofrqyvxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvnpzbhuo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gqrbulbus.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gqnhbkbwo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaykbwgmc.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gsrfgxbtd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gndcnbfph.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gxlsgfpmw.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gtvidejvc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gtytypnva.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gnilgfpqx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/ghbqiwdwu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gvxxbuvom.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gjrvkcphp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gfbdhqvgi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gomsdbrvi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gdlicztgy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gzikvvzka.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gbknlubyj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gpbgrvckr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gcvfcpvmm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gyiqrscmu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gkzgdmdrd.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gnwxcvqrt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gijcjhfvp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvczflcox.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/guievwhlv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gimwcxmsd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gudzmlcol.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ggwsxloqg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gxodhehpm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/ggpswyfnp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gcltvtbpt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gzuwgcwjx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gyfxnlxnk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqpcicezh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxcvaiwge.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/giibckdnh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/glxtejoct.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gnuescoyy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvobyoest.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gbmohzfsf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gfwycfenx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpekshofu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gkrywbrhw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/grkgwceyk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsatwrwyb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gdjseqkbd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnicxtqka.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwvmecnha.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gjrzfxzqx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghtkiybai.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gimqjttgk.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gxtvmnahq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gtyuexqvb.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gcismzjyw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gfenjfxni.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/grprlwyfh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gkcxgosvu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gjwkmjykq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gcwlixusj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gyiujwmgs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gunadtzcj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gyefumzfl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gnmhjxwmi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gdwpwqogr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gymnnsrog.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/grapbkpur.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gluripnuc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/glbxrnqvk.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/guvbzwbtz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/glvvzipto.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfkyhicib.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmfgbhqcv.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gihecdkrz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gctvsrgna.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gnmgqjhuo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gsngmvgjs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gplcaodjy.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gszanemea.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gomynbmig.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gniasgtyp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gseyzopez.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gitryhzvi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/grpogfncj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gwukoafzw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gqeyjdxwt.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/genszkiku.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gkgicpnsy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gfsovvsqq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjgqeykpu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gzgvxjmbd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gzedmfppw.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqjwascvb.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gprzclvxd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grhsdgfhr.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gkwmfrltk.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gacjxtsrm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gyavaopwa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gdkdshzll.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gaslwhnis.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gjxocdwss.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gvapvmong.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gjaemwhgl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gyxztciox.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gxsqohalu.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/glaebrztv.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gmyggabaf.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/grseifwom.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/guwaghmbt.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/glnoqkexx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gguwmaozi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gqndjczdx.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gkflydifg.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/giimpgtnb.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gkjndjyzq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gvpchakni.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gbilpnjfd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gvtrfypoj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/guoltsvok.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmpmeqqrp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gduyozhpk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gajjtamda.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjtvnkoeq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gvnaacwzw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gsynianvn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpgxzgbct.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gddjqytzi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gzpwsqfju.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gowcasltq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gurbxasbr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gfqcsjrgp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gljyazdij.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/glglxrprl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/goofucrmw.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gqhklimqu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/getoszskr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/ghzvsoebz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gxmhpuceq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gnwzvarvc.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gnflgrkrr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gaptxwecu.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbpyfgh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/gjxcwifgt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gbccvenpi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gvhmskkrf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/glciitckp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/giontbwkd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/guzxtcyop.sHtML


<!-- 参考信息 -->