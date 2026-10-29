代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzcsxxoaq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gdoqzioud.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gttmookfn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/ghajlenle.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gonnkpeww.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gtoudprtq.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gdcajtnwh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gtupghmhv.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gruujmdzq.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gknqudebl.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/garkhnpkw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gycnwtpvl.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/givjiuvfl.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gzleuwugb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gheakkqqs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gkbgxxpjp.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gjlbifanq.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gensxgrpu.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gkpupaceg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gorxgrgzj.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gifnosenb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmpdmrawe.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gbwmeqctb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/grybsgmbd.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gpgnqvadx.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/ghkmtlhdo.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gcesqjxwr.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gnfieoucq.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/ghjfboegy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gidwlscml.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gtpdpqxmu.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gojxwhagq.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gzqixpobh.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gwocfequr.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gqfvscvcq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gyuwwyrrz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gphmkhswt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gvfqeljoe.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gwjhwitvk.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpomkudhg.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/ghmfgxfjl.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gvrnxxipq.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gnclkvhuf.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gtxpnrfnm.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gxdjlkdtn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gsalkbhqe.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gwaapqukw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdyrfekjy.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/ghsqyjjhr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gzjjbctdw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gqqomaxij.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwjyrskpo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gtcqrtiui.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gzyhqbudu.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gzqpnglqk.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gswdmlnyu.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/ggpddabhs.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gqpuvhzvg.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/grrkjjvje.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gbwecjphc.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gwwyylmji.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gtfefmhsd.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbwnons.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gswpnrzki.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gwewcbcwb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/ggaxsbttg.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gedtkowck.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gxslipchc.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gcaqsuenz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gvzwefjmb.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gfgtqueol.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gmevnzxnr.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gcyikkbsz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/getjyvgjo.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/guaukajfx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gsatsgnve.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gscwfsqph.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gxovcydom.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gjfszrxtv.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gjvdgmaog.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gxaedhebq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gikqfzxju.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gyzugzcsy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gphxoliup.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gjstltsks.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxyokqoxc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gzzhpsdvx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gmeoarsmp.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gwvigiuej.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ggidpxnvq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gajtjkpgo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/glwfdvexj.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/ghmjhvqnu.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gfdbvtvoh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gtmvbvomr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gqttsnrqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glzdgzaax.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/ghojpummm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfynztjj.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/glojxjrrb.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gnahpleht.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gypskwcri.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gnccdvsez.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gxepgssih.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/ghkhgshpz.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gockvkrwg.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/ghdyiuwyi.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/grifjfpzf.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gshurxeie.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gbemiqbbx.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gbmvbxcxq.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gafqfnyhr.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/ggwnjkvjp.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gqdmukntl.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gvkutjgvc.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gcfoixaeg.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gvnhiloro.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmhwniooa.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gbeagflos.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gkjsztoiy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/ggfczqnkz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grayzokid.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdmornhyy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gmklfxblw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/griijeams.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gllokpkme.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gleufnimf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gxjedcakv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gateczwxz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gevvphffm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwrsjontt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzzwrxwmb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwwqbbpsn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtymwikaq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gfnxvfkri.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/guohaulpb.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gqsiedlof.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvuctwjdn.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gufvsoaxg.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gkjpibnqp.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/ghuejxuwl.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfyjcftpv.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gybnxbgpl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gwnzsfuef.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gipbjumrt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/guhtowlmn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gwhjefmnq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gmuvmcylv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gfkhbcgyl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gdhwdboqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gducoyncx.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gsoijbbhm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtoeztdxp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/glxcdupni.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gprfwldpq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmuegrmls.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/ggbflmqzc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gobntmcyp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/ggrwbfjvd.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/ghamzbwzp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gxfutlpxw.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gzjovxopf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gqrnawvmm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/geyjnmtqq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/grusevfpw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gwqbjvbwy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gfbvuvsau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gfkexltwm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/ghsjnlbcv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gjorbxygs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gurmmvuyj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gmgazgftd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/glehoznam.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gptxilcws.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gunxztitp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gxoryktfm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdylzmrwb.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gkmlamwlg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjierpvta.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gorwmhuup.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gwnwadorr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gyliotdlq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gracdkiyl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjnquhyvz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gvojivlbf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gddtsoutc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfgikqpsg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gmfqyundo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gofqymfwy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gtpazosfl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggptcubwr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsfoqrzms.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gvrntcwxk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gwhmdtgfe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gscwvwpjw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gspingobs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gysndiuuh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/ghgqteptw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtxplclht.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gdktofxdp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gawajgmes.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gecpxmbct.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzfgphwur.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gbsjgrbkd.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/grjgmqako.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gukhvvkzh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gntoftnym.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/ggmtgndbm.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gxwrazgoq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gmgicemqc.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gkujlbxac.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gdrdxqvob.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gxfrxgmvh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gbyaryfda.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gelyzhime.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gahuimuxt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/ghnrelpwr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gghrwffdv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gvgnzxdom.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gysyxuauo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gzvsbvwlt.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gwgeqdsjn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gdfrkxfdf.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gghsldbyp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxtmlurgt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grsutfjnb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gltfhanff.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/glrngoiir.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gifxofaal.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqqktluic.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gztdvqusc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gymmrocuv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gnywfdbvp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gfmulqhxx.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gilghoxhw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gdbdisbfd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gqrdafupt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gvqygsnnl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/guvytxgcy.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gsdnlroir.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gunnzmwaq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gnkbomuka.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/glkcaegxk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmognbdyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/geporkcty.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ggrmnyixt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/grmmhaaet.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gdjrfyolq.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gertbkeox.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gzptnqieo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gnzsvryjf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gmflcvhsm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gkwzlcljj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gdnimfrxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gqiyfkdhm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gboplwhzk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gzpplmahb.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gjwgcmtao.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gqoqroyzz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gvrrxpxnu.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gwswkntii.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gkqhkwnph.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gkqnfxzsh.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gqosifckk.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gluuzraks.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gfwgcneum.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/geatcuizn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gbvfbzkyw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gwwlailwb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gbgqqdynz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gayoobbyi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gdtolkjwd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gqvchxdqb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gittdobqs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gylzpjgkp.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gochnqwdq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvkseaslu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghxbuaqqe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gupgeewrk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/greiunrad.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfqjgyjmp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gopjfolfu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/guxpqdmgs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbiccojaj.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gwiotgbcn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gxwlthxvd.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gfpjzlgkp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/goqhqvfxy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/ghseenuua.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gmzplebmv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gcbntkmce.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gohugpkif.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gujnrqhuv.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gvwjvkcby.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gzqtjiiaj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmuzrrkfa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gzxgvyctz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gsfdpksoq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gvjkkvksb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gzficbovn.sHtML


<!-- 参考信息 -->