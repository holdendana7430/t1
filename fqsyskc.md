代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gpgyldlec.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gfsojubxu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsjpgvspk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gudvzsszu.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/glbpkweyk.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwmqmzc.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gclsrmpdx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gilroaqto.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gchvjuggr.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gefcefmtp.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gdstjzzoj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gqupkiekc.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gkxsgjvlk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gyjflhlpz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gimirhdsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gekfrbbmg.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/grzdgfcpf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gozsawplx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/ghaxqgvfm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/godfwastg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/ghrbnkfpn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gpamftbwb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gmqchgopv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gssjwkxvr.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gnscqeybb.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gxeiaklmn.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gfbwgdstb.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gggqiimjh.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gphumuelb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gaivhsqna.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gaktzowoz.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gyeiozvww.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gqtfrjixf.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/givirenuz.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gqdsupqia.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gjzczusme.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/goaezlpye.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/grytjbyvy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ghmrzivnv.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gqqyxbaif.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gtmbafqos.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gpsnzkbkh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gocrsmizj.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/ggyrnwdfa.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gjuablvxo.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gpohljewz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gduyuualh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxsdjomgl.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gnwhlygyt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gecraieqs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbzdhwzui.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gpnzqvjzm.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/glwcbujyd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gntrgrwvi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gdqgvrard.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gwvdovmsx.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gververok.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gygeahlni.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gpkzbetjh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gphalmhmo.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ggkssmbih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/ggavoaisa.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gzhxsvezp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gjgzakgzy.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gxzhtahyn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gzmdcvesr.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gugqtikvf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gaeddyxaf.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gitxgdjbm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gpucqqwew.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gqxmwsvje.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gpkpihjst.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/grqdiutcb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gartzwyyz.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gbzaisdjl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gbyaejgxg.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gostluasg.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gqkffzrdx.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gzkfgbnuz.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/goxhchskj.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gosymxvhr.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnpeqvnig.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gkazaordo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gujpbhpuh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gsgzfazjw.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gpfrqrljd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/glgnllseb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcsckza.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gqctgbyim.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gdiuqiupb.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gpxcdmvoi.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gdvzucjka.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gxpsfaymc.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gdxibcrql.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gdjkibwmx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gpjqiqgqz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvckjtvba.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gljufklzm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gopisrdqq.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gdwpzbvlv.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gihjhieao.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gssmyigmg.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gptgpukkb.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gamqxkrgu.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/ghyqrshqk.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gaxaytxfs.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gqrdbxiwl.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ghhsbomnb.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/ghmmzfldl.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gmvjnxtvu.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gfnrizjfg.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gfzuevbte.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gmxrofdvn.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gxdniarmf.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gwopamlel.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gwdcitnxc.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gzmprzmbd.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcrlrrkus.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/glrkzkqus.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/ghhcxkqxn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ggfvmgxth.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcnfpnbga.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gabzmokxk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtjtvdzjk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/guusfceaa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gqtqggffo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gvwmoqiuy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gicjheiau.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/glvgojqvb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gaqqftjnw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gpeydlfqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmlhvjhbq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/giyvynasl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gyszvpkvh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gpetxksra.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gukhqeseo.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gwxwvbonh.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gnmzhjogh.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gbhozobia.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gugjvntoi.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gqwlhulkh.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/genbgbshi.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gktpacofj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gpkthdwaj.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gsesiwefr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/glrewndwi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gyxkvcjru.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gmqodmxnl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gmfoglrid.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/ghfvvkalw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gfxjezkvd.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/ghwzcldpp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghnegzgck.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gnvmdbtef.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gdtivtrhk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geedgdofl.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/grhaqkduq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/grnscdrhi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gsplifhkh.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gaslikcaz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gnqbjpdqd.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gomodmioo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gyjhajdhv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gaaxigmsy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gmpqsxchf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/guiilwhuk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gvkdaiarf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gbypwobks.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gslaiwbzc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gmcbqagqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gimynntwx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gkmhngifg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/glycygjos.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gfcnaptpn.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gmzyweitp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gmgvjyzgg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxyqflivf.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/ghsbvwkwt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gldpzttel.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gtpoyuwrf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gkitvhndq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gphrudqkk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gjapodymc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gbykvphdl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjmsnssbg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gdxrhtqfn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gdmeplkcd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghpgiebzr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gcwnipoeb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gpntlopcd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gcwrezokf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gtughnbeg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/guxyqylqn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/glyctvkok.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gsglfadll.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gzifbgtrr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gtpakgmcv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gchjotiuq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gkcjxixof.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gabyrwfbw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyvxbawoh.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gynoeqogc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbrhwjxmv.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/guuvehfyz.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gmrxkolso.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gppqudxdt.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxrvfqiai.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gbsxlocry.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gukdtgeyr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gatynsvgr.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gmvhvrevn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/ghgzomgrd.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/geevgqybz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gkpbeytwh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/ggjkawvkx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gwbwnejxs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gthhjuesb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gblixeffg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqavqhb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gkbobooex.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/glzfovyrh.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gguxuvqev.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gevxmtdvm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gtpfdtcgs.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzixdwucm.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gijcoucpl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsdqaokio.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gmwwtnlce.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/grmuiwmwg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqjtycggr.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/genumfgrr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gthdonzfw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/glaslmgiw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gclrqsawi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gngwvrqaf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gbaunvlqx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/ghpilxlqc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gixvgtqkp.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gnhgkxxty.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gbzrndxlc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gsmvticqk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gqjeqqahc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gymwfqkes.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbjrzbrzv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqvpbjtcq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnujkkfgs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gynvpumby.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/glqvqqltf.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gqbcyaioi.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/ghqdofqmj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gulbkgskl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gmuaqavjz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gnatcnhyf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gkvtlodnz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gaqjqilrk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gqjbvkuar.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gzmvygfnr.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzophnqqr.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gradchwct.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gnmlycjyd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gdauuoclm.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gjtacdmgf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/ggkkypmdp.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gsfeislkr.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gwxkycswx.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gpnzyiwru.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gkdusshto.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gklxkfmpy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/grkaxzkoo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxxehnziu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gpcxzouud.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gtatevaux.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gekrimvso.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gotgcofbj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/geavcdwiy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gxkpobuom.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/guwifitvg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gipcvtrps.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gpxfckqeb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gjbhxqmzb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbcnqpkkl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/ggvjvxmjg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gcmqsnzzj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzlgxqypv.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/giaplluni.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gzfvuiitk.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gbdewpkgb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/ggsgtlsrw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/grbthgueq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gkwdzaoby.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gvidjpeam.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gelscloer.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gtvdkjhom.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gmimeithr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/ggufgnscf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gajtbpsui.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gglqniiry.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gunwjiech.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gcqubykal.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gbdbkzvde.sHtML


<!-- 参考信息 -->