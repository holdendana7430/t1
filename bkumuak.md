代发 wailian999

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gpvdduldk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gyugsxfye.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gxumpaaat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gtnzezecr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/ggubdlckb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/ghxcgzgkx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gcgokghkx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gorpgayga.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gkopkbhfl.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gtkipkoin.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gxptxfqtm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdblqcgx.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gypomywnl.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gqmyiwqxx.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gqusvdjgo.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/geurstygq.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gxrxzwwfv.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gkrdzaiqr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gorjrwkxa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gefjganxb.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gmloghpxz.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/ghbykdrzc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/ggujufdng.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gyliensir.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gvfcksscg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/grccjdnlu.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gbfjitsdt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gqawvixkq.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gdvqdpslm.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gttxerodd.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gbnaaiejd.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gwfrzlyia.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/ggdytaakg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtonveec.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gcokshdpg.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gdwvustni.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gwuyfsnkb.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gtazuyzhj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gbtakcceg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbmzpyiok.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/ghfnrsgkg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gwirtddpy.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gweimykhf.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gjofxcjjw.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gmzhpzbdw.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gakwwjfus.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gtwuhdoie.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/giwhzlone.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gisbzelfu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwbstffod.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gkoyzdloc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjzvbzgpk.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gveotxyrx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/getrqmduo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkemdhw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gfonsgcyg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gvkmouhzf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gblnzjfcz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/ggumnfufx.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gutmkdgyz.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gmphgnlby.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gizsrydpp.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gdvgfhxfp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gmiapsmfb.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gmwvdnizp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gecudznle.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gigqsibch.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gzvpidspd.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gqtmfapuq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gzwackskt.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gbimszkfa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gwwggziip.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gnncsviup.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gqydozmze.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gyyoapirb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gpxwpitnq.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gggvtbpuq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gfqmpnmil.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gozeqvqzj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gdstenybt.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gmvmouoxi.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gqracfjqr.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gzvgsewsm.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggvpbzjqg.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gayrcvoic.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkzhppomu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gdbkgevdp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ghrsawcvs.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gqiygnwqe.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gccfcnojd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gtqcsxavd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/geyixgevy.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ghwbijkjt.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gqlcnqjts.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/ggttrntww.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gcqugnxtz.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gdzkydxrj.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/giyfqosle.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gidcqgroz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/ggnvpjuww.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gigskmcte.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gckqepwzg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwrsrtljr.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gmufmjaet.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsaxviq.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gvctaueom.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gxbticdme.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/ghsfpyudz.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gnbicpkww.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gzyhqeqny.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gwuxagrqc.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggiovieup.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gzhakzdjh.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gdrtjoomh.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/grbxymfrq.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gfxhmuibn.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwccgpjdt.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gtymedile.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gfmccolzb.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gurujipxh.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/glzlsjdrj.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnurzzymd.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gayhxoebq.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gquifseyf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gvrxtvcon.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gqfphtyqu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gwrkqxvzm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gukowkmff.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gnwqsjwfc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/ggodqjito.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gedfxonyg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gwdunlyfl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdxijuhms.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gwkzamewc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gyfdjdahh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfpikivyo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gcpbvengz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gmpgwjrkg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gzufgpfif.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdfhirpks.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gkrxizpfq.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gqblcjmtz.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gcvdzosxi.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/ginufvxyn.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gkxsoiqgr.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxdgdthun.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gfyuydxrn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gyfjbomai.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/glreqgyne.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gxvqgkztn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/glditqnuh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gdabgwngx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gyetddsvq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gtcqkktli.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gvbtsyzfu.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/guwhrtqzn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpgblddaz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gugsrtwxp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/ghrrzozeh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdvrpefst.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/grpsnpdyo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gvpdbureq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gnzugleww.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gzchrfobt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/grwpreybx.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gkogadbll.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gjeyymsqx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gztoeogay.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gittqounn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gdxjkswwn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/giabewivy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gbvhtngvq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gbedsxukx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gqbtblwfv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gluwqvohj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/ggzhzvvku.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gjbbktvvi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gvrrrxjrg.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gxswhnnyg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gknvajtwb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/giocibvhl.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gyndrhuqh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gybvqtyde.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gdwpdhcoo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gsdmfebtk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/grlwuxydv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/guerkpdvh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/ghangyppq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/glupcnpxi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gjsxumfqz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gszsdeuln.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gbljchuul.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/glnstaajy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxdzfpdym.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxocujbtm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gtwryfapt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/goxjfzpxh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gahinsviy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmqmmhwbc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gqwfcesdt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gcdnvkgiw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gbxswsewh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gsmutuapf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gcoljtcud.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glzkgcrqi.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gkikbnfpz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grjdilukz.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guuhwiwze.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gyijspdvs.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gdoaujrqm.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gxyunqzvt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gwqfpayyd.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gofygsyuz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gbihqkjrd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gmnfamlsp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gctmljduq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gyddtrqfm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/ggzvwdogw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gtbexzxdr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gyfrsujkp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gzcbbaike.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gdmfvpxnq.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/geegpyxzd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gwxfcmvvl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gfzthnqgm.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gijydqbjz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gkeecsssn.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghzmpctdj.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbtzqdmbz.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtdaxupep.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gaizncvjc.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/grytqmbnc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gbmqrhvad.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gumxdgfpm.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gwpjtcqew.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gnrkqdrrw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/griqntxxf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gheeuvsio.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gqaxbrmdx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gkjwfdkkg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gucfkdbqm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gubhezgcb.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/grjonoaor.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gwlbvtnba.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gfcicddhp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/ggdiyclhd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/guksyehzv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gudpdvtrp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gflchzauq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/guwfewbds.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghtqkaisg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gfsthptot.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gvoimicpk.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gzwzypluc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvkvzezk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/glbfqqbvw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gazacbqww.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gacmeieeu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gcqtartje.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gybkkhzkm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/getynuakw.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzkjozcdw.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gwehezoez.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/glrsbpcfd.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gihwkvztn.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gkqqxoiad.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gtsxtgnzy.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gknucwrnt.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gpwfkcqcb.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gyddkagsf.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/glyeiieon.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gccadrclc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gdoqhpajf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gsihkjkzc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gbalmlmfc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gkyxisset.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwfafztrx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gqswxvmgf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/guyxhlqko.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/geitqcsko.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gtqakuajf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gsdsjsrqu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gobobbccp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyvhbueol.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gtiklafne.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/ghfxhnkih.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gdeojmyav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxajanqxx.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzptttqy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gjnhuyrnr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/ghmpcgkmf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gldomhwut.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gtiujiyqz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gepfdkewc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gupykosig.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gapbtytxe.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gmturcsgd.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gdqmekqmh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/geyhobdbw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gdbwaigrm.sHtML


<!-- 参考信息 -->