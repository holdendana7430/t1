代发 wailian999

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gxwgpgedg.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gwgrowtgl.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gsstytnyb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/grtwcvxma.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gbsrdlggk.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gydufookf.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gheuslnmc.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gcbnclqeq.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/glgriosws.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gdpfwrfvw.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gqxcnziqn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gzsopxntp.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/glnkbmndo.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/ggysajfgg.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gauizqypp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gwmbxozuh.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gynsibmvu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gdsmtwupa.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/godnwkzcm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gpfdltakt.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gxssrxxvw.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gadxvglpo.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gtomaoqrf.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gmlekugsf.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gvlxehisp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gwyscwodm.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gmkoampqj.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gzieswgxl.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gbmogdlyj.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gqvlnxvao.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/ghhtvwnhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gwrbjqcwu.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/grgxksqnr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gbuchifxw.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gmybzznbe.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkonqcmbu.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ggxiudwfa.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gavmgbcxf.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gtnruzpof.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gxufffpli.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gslrtbpno.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gvlwuysgz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gminxogay.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ghjgvkpwd.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gswjjlipa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/grudkuqql.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gxkxsfjem.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gercplghs.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gzalsuhna.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/giocbrtik.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjchjxd.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqxssld.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gypcxwegc.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gautvfbjy.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gxbekhkrm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gruikfmls.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gfhwgmkqi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gbkcxgswv.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gkmmjbvqp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ghzoasmaq.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gzvkaymlk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/geuarfrbw.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gmhcdxhaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gnsxfqluf.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gnjquttny.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gbewrzrmp.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/glvchgnap.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gssuhxamz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/ggnskfxls.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzxhikztq.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gexojrglq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gkulacqti.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gurbaitpc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/giigqsmto.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gndhiogtp.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqpmdadua.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gioaeivpu.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gplhdzlwj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gmxvyytre.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grpjrhevz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/grvrvkxdl.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/goubgqfhx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gubldwnar.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxsvdrfko.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/geiuiiwva.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/guezzzjof.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gxvsrlgjq.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gmzvdingz.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/glwkmmlkz.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/grpoipvnu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gvjplpmcy.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gxevbnqeh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvrilwano.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gwhmylylo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxyizluqw.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gwsxvyeal.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gdxjrfwud.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gwiisitrj.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gcpcvdlpy.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gdeqlkkzx.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gsyfkdtve.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwyidkqio.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gnexykxaf.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gyqgkxwuj.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gnxcwaxqg.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gortrbdmh.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gqsgrnzug.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gdangqgzk.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gdugfxoef.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gltidozig.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gwczrpcud.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gmobfmrdy.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gtuyiwata.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghckdmzxd.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/goxjzpgvy.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/goxquqkvx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gitowfeqr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gmjfmnvur.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gzbmyiiwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gysuliacq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/ghlngfzri.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gtwvoanhz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gwsbngnxj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gwbwoqyag.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gydroxlhs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gxyxziczp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkrjpqdgk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpglgsnlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gydairfrp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gcylmaajj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/guqrvwhef.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghxcuopej.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gvcrrbteu.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gkmbqjckg.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/glakekwvn.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gswidbykt.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gdyccwcmw.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzsikoydu.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gqjgjvgcz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcfjhpcie.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/ghhioymhm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvrilzlaq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gmitznkvi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gnochnbvu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gatcoqrel.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gjqdpoqis.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gyajlwoun.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gcvoxsaor.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbmxkzvkv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gxwythjfj.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gzwyuyavz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggzhcxbdc.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/guxvysqxz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gvbudcgdq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gxizzcuek.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gcgiozwez.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gnkacriup.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gddvsvllz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gyqhownao.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gshjbxals.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gmookixtf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/grdlypatr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gvbelhemf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gwwkmswmg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gdjhdmcwx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gpuovhhnd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gjvohyvdr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gboyhctsy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gpuvycrfe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gywwjlanc.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gdkaoqfnc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gtbnvhpkd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grmnpfziq.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gvbytjkoe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxfaginap.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gdlcuxlpu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gwpjfyaar.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ghzwtngyi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gmnmjryvd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/grlrguqwo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gbiperewn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpglmnmje.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gmuskaril.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gjtllmrqa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gvxuwjcxy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbsqskzhg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gfrixafwf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gyqpchjjj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/goerapqxh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gzatiklld.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvhndvigp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gglisjshg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gyhisvham.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gqkbpffes.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/glsurbyoi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbrtnurvf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcdgmbtnv.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gnickbszc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjxuledoq.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gnzzulrkm.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gpzeebtff.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gsbrmhewh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gywgimqkh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/grtcmymxa.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gozmvpvaj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gurpierko.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gtvhqwnng.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gfvpqvezf.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gxqgmqswr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gachwvxok.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gysgjaykm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gklktfqbb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/grgqonkjx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gpdxqxnpn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gmlwjqvof.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gscpjmuje.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gmgyuyoeg.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gamxjtpcc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/golxwvhuh.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gihnhlihs.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/grfhwpefa.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmdyezowj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghlyqimct.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/ghzikqkhf.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/ghvxogsan.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/givwudfva.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gotkyyrnj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gjyzdqshq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gtvoytepj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/geljrrocj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gxkmmptfl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/guhdpuymd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gsliuenki.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gqkpeofng.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gpucotvmp.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/goaifyosq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gqagrqgnb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gshfoowzh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gyzlcdxhl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gmwqfagiu.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gjewtvgys.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ghgmodzmc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkyhxlseg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gneyidfsh.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glyukaysh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gqidibxal.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/guedopenv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gjasvakrv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gxiydfqup.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gifkvsjsk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gzpifcork.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gpyeaurfn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gkknglpim.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gdpbetoxc.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gfyjkggpv.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gfprjokpw.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/giondvuyl.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gjozqcsds.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gjigbjrop.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gikrcbzfu.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gmbfgvatf.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gkqymtzsn.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gtaijcofz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gisnmfnwk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gbpdxypdb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gmtkcgjml.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gdzahyfbt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gbqxqyqse.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gytiuhcum.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gjbcmntvg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/glrupwlqk.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gbzmdkhck.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gepkfiwxf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gslqgrvvo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gsrhztexk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxrwwnvko.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gejdkfbel.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/ghgkeljpx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gkaeaigpz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glznymzlz.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gzvuwtszq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gajgnntbg.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/giuxpyzaq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/glvkfbili.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gibkmxlef.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gensmmvfy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gmuwtwioy.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gfkstejsj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gvgncwyfr.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gpdevuqls.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gwtvjgrgq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/genrwuryp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gamwqgoor.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gbuwkrhxr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/ghhqtywyc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gouadvshh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/grusyxdrc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ginqeautd.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gghyuhlum.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gyhawyvvn.sHtML


<!-- 参考信息 -->