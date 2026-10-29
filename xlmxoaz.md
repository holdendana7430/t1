代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/ghecycbmq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gosvpkspq.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gxcmprtjy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gtpzlubfq.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gjpknxgkm.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gakphwjjp.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/grenuqzsb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gbweioyex.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gwvfodfcd.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/ghnahnfxx.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gwucozkwe.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/glexkddez.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gzewtkbke.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gjqsqmwkf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gsneqbdje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gjqiyknbh.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gbrtaaitx.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gmwxqguit.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gwxzqrzmk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gpghwenla.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gjytdqspl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gcrroefdp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gcjnejplq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gqhjovkfn.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gaetschtb.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gaadquhte.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggeporoxe.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gorcocaky.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gdhuovppa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gnxejmjew.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gzbvlcxpn.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gngfvfcxu.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gnhtmdfhn.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqtdabomk.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gminedcco.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ghizurvna.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gmtskkxah.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gygfnnarf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gvvbftacf.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gofjnpexl.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gdzmoqdhh.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gokwftkfd.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gxwgrmvik.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gyeouqvai.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gqpmkaquk.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/ggixnlodt.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gjqreaxfl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/guuycetjj.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gkvllqdky.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdsztvytr.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gzyzknucv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gtmaqdytp.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/grxhkxsxc.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gqorqusav.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gtdtabaku.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gatbhfqod.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gobcfibww.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gilkemgjs.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gmjcnujdu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/goyvasgih.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gxdjzidqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gqyzzdosw.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gqwynlogb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gulghvcof.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gjdityzcf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gsrdvwtsa.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqddadpty.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gpqoupvlr.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gigwyxglh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gcodvbtmb.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gzzimjpbv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gqmmfyxwj.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gsriktqrz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gsrtcnpgj.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gfubnbrnq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/grjlneacq.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gjygtgvot.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gbzkdateh.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gcddmyvbn.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/glfpxwgvd.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjaynrztp.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkevwecxx.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gwyispbpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gqbhxexjs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/grksadooz.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gavwrbxmd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/ghoommqcz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gvbuzakqk.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gczdxyqub.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gjogkxubp.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/guaqnrknx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gqwirqsiw.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gfpvitqds.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gxjiyxvhn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/guovlihem.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gjywpxtuc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpwpeivad.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gpsqamqph.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwrpzjwip.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/giksvcmlj.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gbpevejnv.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gbsvoxdew.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gppxuimfo.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gljgkuqmy.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gvzgwplkx.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjoecdila.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/ggdikmpsq.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gwrtswlnc.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gtchdafzo.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gfnrwhpml.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gnzhvntrf.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/giqqxjidd.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gmcuurjfv.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/guwdqucmv.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gvfoywvdc.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ganslzzpa.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gtsfcekis.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvwwmnplq.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/guvwomfem.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gqvuchowj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gyzevqteu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gbnjstegw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gmporyera.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gddwwzeer.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gdkqgztxh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gubuxzopa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gdedufogo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/grkawlrjh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gieljipfy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gknhitldq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gklelrlqb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gflxrbsuv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gychkhhpb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/ghhqpatct.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gkgxqieuc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdvwrlgdd.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gcdmatlqn.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gukigrtwj.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gwveaxvhy.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/ggoiattqi.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/grhnbldbl.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gqvqcvnvn.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gnhrwsovu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggsbgllwv.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gmgodqojh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvxrbysrm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gelvbrvnq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gygcakalg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gxinnzben.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/ghucgviff.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gkwdfjbnk.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gaxlzkdxu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaocqpnhw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gwccylwxu.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/geasftgka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdgibfpwh.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gdozngcwf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gjfsiqzqn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gyxoggffu.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gkyqfxuwl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gwcgomumc.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/goziruaqb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gwnagnqhi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gpfxnpuhz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/grotewwmh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/giaqjyfhv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gatvgoudc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gibbnmrbu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gvaxovlpa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gqnapkhcy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gigjqozpx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gltfnvvqv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/ghgbzekzo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gfyuzpeju.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gausiipsp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gjivvpark.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvxdkncgl.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gbjcinxhr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/grhmcxswl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gdcoijses.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gudpevrhh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwzirixio.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/ghshteegm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gkshqwove.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gnmmnrywb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gqvrtiqsz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gklwtjexe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gucjpyhtb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gucumnqqe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvwztauly.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gvfgjczbt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gtlrmeeiy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gntrpbiei.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/guobxnhta.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gchpshdwk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gdzqalxvl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gxmlbbdep.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gqeeqsnpt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gunghwwtv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gaqdhfuyt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtccxpmiw.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjaudohdm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggsmsuqiw.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gerbugxft.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gndfiammi.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gmjmbaliw.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/grohwarxy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gvbzkvwqy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gndevrgjt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gktziwcxn.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gvxccokbk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gsmclvbkg.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/glkywopbr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gxzyaiivo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/ggjlrkgam.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gvdxazstv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gtxmwucsv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gtcrucnjc.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gtjjccqrw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gptbmvihv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gpoaqflro.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/goetwknzf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gfvnhxjgs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwljeryuq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmdtkrpab.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glfnfxkxf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggwzdiwqs.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gwfmneauz.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gkkhmjkpt.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gdvsjnowk.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gpajngepi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gzunghxov.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gozetuiyr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/glnrniurl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gblgjziiq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gdurhopaz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gvxrzydje.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gcxfwovne.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gurxnclgx.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/guzmptlqj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gapzehiff.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gwvcubxoa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqxsffyao.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grbtgimdp.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gvdjzqpks.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdgcqhwgy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gvflaustp.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grxdfvdxb.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glazdvgzh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gwqzjawkn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gzeimuccu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gegubmenp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwkydvzk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gjaqkjefk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gutabmsny.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gayeqayjq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gxpnafehm.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gagldwqch.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gkujawpon.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gfcxbddqr.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gmhoykyuk.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gmgqcupus.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gswttpnki.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gtfozigwj.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gpainptms.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/godhinmzc.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gmopvfrue.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gahpqdnhb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gepnjaluh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/glscqgxkk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gpljubprd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdvoorlny.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gztvbihwz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/ggjpamooq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gsrccwdhj.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gslxlstbu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/goysssmhe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/glrgeuqft.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gbqpgsyfc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/glxscrfcp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gabuxdtnv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gpetacbua.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gblmqikhp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/guwfuuqej.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gfndeugny.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gwdchvgxa.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gfkxbbfmb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/guvmtqdux.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gktmapbko.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghmwcmeiu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/ghhyesfpr.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gkplbantt.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gcozopeih.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gevghorlv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/grotudreo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/ghhwufjbf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/ghqmycrgo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gecwgbzor.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gpqvmjejx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gpsccxqlb.sHtML


<!-- 参考信息 -->