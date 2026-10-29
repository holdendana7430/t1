代发 wailian999

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gruuuapww.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gqvvcoiwu.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gohxgkuxh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gjtrgvjfd.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gjcdvxxlh.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gcqgqdirl.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gftujblid.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/ggvxfldho.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gqkmeaohk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gmppunjrq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gfvtasxdl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gsqdjtgon.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gprutkxzf.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gvkjpbkvs.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gjtdtlrsr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gzyzmabvz.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gatkgbpdb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gmpsgvecv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gwbdmtcen.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/guqynqmrj.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gbpddnycx.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gunzorvle.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gzwtnmkbu.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gmkxdtftm.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gokhzmfcz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gurlajrmj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gglggbfdb.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gaeanqgjp.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gafqpzdxq.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gleqeysnq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gfeclueqn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbryljhdq.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gemdzsygj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gzlwyczrk.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtryahihh.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gdvxhtizs.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gcffcxerw.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/grktsicao.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gcvjupvhm.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gjbvedgcb.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/guliiwlzx.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gufkftxcs.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gkytysdpc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gdrjajwmf.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gyynuvcfr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gziqzngkd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gugqngoqq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gleueldzf.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gbhrnsmgh.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gzwmxupwm.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gtkiclwru.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gugjpokkv.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/ghyktaheh.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gdggpewhu.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/giriihpyr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gribqwzaq.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gsubnxgss.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/ggnjlnxss.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gukyhqtmq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gwksmagtw.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gjnimkkyo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gvupzynld.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqqllfejy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gzlxbtsbw.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/guepcmmyu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gugmcoput.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gqgpfouxr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gcgsbigpc.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ggvxekrcr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gxqvsesqs.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gvdyynhlq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gsuarjuek.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/glnfvpmyb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gigknkhea.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gjrbqgask.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/geliczcoz.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gpyytnisu.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbggdsikp.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gotinlzvz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnevayytp.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/glujfqdoy.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gtdeywzmm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gkfypklpg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gzotadevu.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gdixyrzlg.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gsczilzhv.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gfpopkgxf.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gmofckjxx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gggabbhho.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/guxrrxjia.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gjbkqqxiu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/ggdqldpat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/girnzalya.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gugrzygdv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzlkcbnxe.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ggkrznvcu.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gnewrmvok.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/glcykntzl.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/grdqlhuqb.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gnmxcyqrh.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gpkthpdxw.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gypnkitni.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gaduubyzd.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gaanxsgwe.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gtthjlfgh.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gdsqnbuun.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/ganwwcsub.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gyqkqigtw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpvbivnej.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grdqtfuom.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gyzgqsdwg.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gjwkbtqij.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gjijtkvao.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gwayoetah.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrdpdon.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gwmuqngay.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gglkbmtdv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gzypjsynq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gfajmyvcb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gnsslanqv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gpjxzaqpd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gfhtdynzw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ggjjdcprk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gyknpqylm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghgrkyrqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gicwgotne.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/guemaqmsm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gaidfschx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/goxxxxafy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gxnibwkqr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/grncwnsrp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gthkacnho.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gzjanxlpv.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gbdpphjrv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gshzclluq.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gzouaflsd.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gxuwqnjaf.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gmpegxdjy.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gerfovber.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnrbfcevv.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gobzbbjqw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvwhehlfb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gibtyjfin.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/ghrcmopjk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gxouyyyvk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gsyzesetz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gbeozgimx.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gpjimjflq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gisiyjyxi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gwwgqzxzd.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gsiflirve.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzzifhcab.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gplgzgtuf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gzlqygwom.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gzorffpem.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/goiomhkvk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gdhyrcupy.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gjxoqdcoq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gcktfctam.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gatqoghuv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/glcodjrtm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gsjigolra.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gqwmcxvgz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gyhhnmqsh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gvbfsgpvy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/ghecdvbzk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gnchljvgj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gsofhefyy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/glfcpgplk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/guhaqwnkx.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gmfqdspab.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gymqsjyto.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghhqwidqt.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gfbclzvyx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/grdnfyuvb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/guvrgqxuy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glwzvuepe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gepylrgli.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgjpexo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gxdlubxwj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gnrfmrrnr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gejzwdwqt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gabryvdgx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gmcenwrsg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gpuznrzvo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gzzwephkh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/glwcpydpz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gbyxyxcdt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gqcpelqkn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gwqsfaipc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gkhtmkdyd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gpcxhwsul.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gqpgxxcpe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggtfplvlh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gtdtimjfx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gifjjxvsa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvawmssny.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gwnkmkwbg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkdeqqodq.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/grioyadse.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gkblslklx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gysscoofk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gwjsbbokm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gutirobzu.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ghfpcmlxe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gvhmzqtkh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gdwfuzzaf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/groxbtflt.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gnixwdljh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gsxwzgalw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gypkkutib.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gzzylchgm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gafmsllgs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gdlxbfera.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/ggsjigbeh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gnxccvkmf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gkwbzhiqt.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gkzxjjzcy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gysfewwxl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gybpexbxa.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzqkofpwp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grmirntlb.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guxwosgwt.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gijxgozqg.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gyfuglzag.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gljpdezfv.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gmeygycoa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gkawjfphc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gkrkqgdlr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gvjlnydfg.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gjktnxyoy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gczxzyrbu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gjvnuullr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gfsglqpzi.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/girfbqxui.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gzmpbpdys.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gazimtaeh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/golnwccyj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghyxcrdxn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxrhqnpse.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkzwgannc.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gegyvwena.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwjmmevfv.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwncncjmt.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/ggxmeogls.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gybjmskuy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/giojhdpeu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gwyaxpbky.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gdltassbk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gvmviicft.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gckvljput.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/grbnyjmpe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/govibsjup.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gcxnxhapw.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsjeznust.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gjwiasfgo.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzjxxaswp.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/ggucxzdof.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gcdlvbqmv.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gfhnlqfjt.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gwirqyzji.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gkfnfrjdd.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gmyhrfico.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gtublkecf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gdymmwdpa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gzbpvnkzm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/grbshhsrs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggeagbraa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gkcrrieiy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gikoevpph.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gshfpvrws.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gamwubsib.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfjuxzywd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gprvfcywq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gdasxbyzy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gdnvxmirw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gvjtniuly.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gqqzbchni.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gxqbutogg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gzeutquiy.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/ggemxdrrw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gyvtodylj.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gcmwloxjt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gkrvudbtz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gipnikzll.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gszzsoknw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gefyeapga.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gjlyslfyb.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gjcajrgvq.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gpttzhdzn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/ggviwwecv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ggctljucb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gpgfskmkf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/ghyhqtqzi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gaxpoxcne.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gvqfxnxai.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gkybaqjxk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gtyurqpxt.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbtfenfmg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gdaapmycz.sHtML


<!-- 参考信息 -->