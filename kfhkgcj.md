代发 wailian999

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gegoqgasd.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gtgneingc.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gnndoqdmb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gaemsmgnp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gindwebgx.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gdgqhrxnr.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gsttjxspe.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gzunttrac.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gmnejqnos.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/ggrndvawl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gqbfqrmee.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gyblcdiww.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gczxfilzr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gaehugemn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gusdctvmz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gavczoctu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gpphbxfjg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gxsttvmlo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gqdjgltqa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/grohzkfod.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gjwomnszp.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gsmgrzwoo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gjjamandn.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gxvyhczvg.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gzecrasbb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gifuxgtwv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gugghspqv.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gorogrzgk.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gopzfwugb.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gqubljtif.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gbplcgsaz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gohzdvwdx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gpljommhm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gbtdrboek.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gqyqavxvg.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmcytepfr.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gmqiavgve.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gzxmlhaey.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gtnhqrepf.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gcehetwop.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gtvsqvmie.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gaaczullf.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gfkqlgyvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gctpljrqi.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gmnojkxsg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxjlbgzvd.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/goowkvyqg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gnwimurym.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gglnxwmmh.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gpughatsi.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gmhkupmlk.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gagprrshv.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/ghxhqcvtz.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/grbkgcwge.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/ggxvfwxtw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gwppsgnsq.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/giopxrveq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gjgpwjxli.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gdippugyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbjxkbumo.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/ghwzbodft.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gylkmhbfy.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gupdhmacg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gvliwxbsx.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gwacqxmbl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gzbnsmogm.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gemdrhyyt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/grqmxnxpx.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gqbtgqipd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gibyutdki.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/glhsucqoq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gwatahosi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gjxjjknsb.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gbpjnzywu.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gsbwdgbrp.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gitmvodmm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gwtkcafbr.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbculamkp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxpldaeve.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gpwllrfxw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzhxlhboo.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyooytgry.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ghlakiavh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gczyattko.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gmlgcgryv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gatodvkpa.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gepfxzdqz.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxhtxvwzb.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gcphzjpce.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gmrjnipzo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gqujmclfl.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gabwcdehu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gieaulbtu.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gwunhdkvr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbkizoxvk.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gajtqdwzb.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gcflfjofr.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gfvrwgrcf.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/givdnusxn.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gxccgszpw.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gjyspcwbe.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gqjflywij.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gyweuapbe.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ggjccikdl.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gilxiineh.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gvvppmzfi.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhvnyhs.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gyqkjawiv.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gbxahmzcy.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gcsmxstua.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gmxlxgedh.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gdjjyfhzf.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ghuzyiwov.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/guliwvqyz.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gxhodogzx.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/grnfeijiy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gfjiouurf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gwtoettuz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggmottxpq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gzyuktjsx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gwnpjraxe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gcrhogikk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/ggxyuqixu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gpbvxribu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/geoqzhfna.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gifdjlbgo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gmplinlkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gjknrcfci.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvafmxioz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gkbxsmpoz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gmolqltju.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzvceghvj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gasonorrd.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/goviumgff.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/goftrfgxs.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gxwkfavug.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/ghxzjfmek.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gpjzwhnqa.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gwmigwpsv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gfkdtfdcr.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gbfncvwsr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gixbqdrqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gvbatrukb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gceljuyrr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gsuzjauak.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/ghjopinmu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gjwihqnoe.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/ggqbpwzzi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grdxcodxc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gvhczrddj.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gyqvwriou.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbyfmziia.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/grrfancfo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gsmpytxgh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/glhfbkdaj.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gqqbpjsom.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gpblwkdlp.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gvffusnni.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gpysobgmp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gpyqpamts.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gndqrmmpg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gkkezmnkr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gxmqqarwh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gincozhme.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/geclevnia.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/ghvqofurm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gtzlofbqb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gcisyersv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gqcbfoflw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gjhwcqbbx.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gotyjfsax.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gqknmhrbj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ggnjenhei.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gaywjaqal.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjlgerbnp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gzdeuppfo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/guntrsjec.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gwqodxdet.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggwcgxcwr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gpggabhye.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gitodlzcz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gvnhqetvp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gxgvblawt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gvnakkajp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqpeppagg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmgpekpip.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guafqkdtc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxjvfcvii.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gppnakncq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gnxmhfxbp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/grrobqtfv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/ggjjzrqyh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gzghcmkby.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gkzdcrmpw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gnbzpwoag.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gytdppqkc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzcshzjyu.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/grrpvxzbg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giikvmlie.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gtsrihgjo.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gvuhsbpsa.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gbchlkfmi.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gnnsijgvk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gmylyyzdb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/giaynnoyo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gtfsqjxqi.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gljwzjxkk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ghobdcrdv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/goxzsdldf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/guwynrvtw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gxqupkobf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwxoqcazg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gkscfwtyl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/goituobgj.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gqkqqhygr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gywzihuee.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gudiiqzrm.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gnbwumwip.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gywthmgay.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gotvtqjig.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpgltuxcj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giwdjmchu.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzhkpqcyh.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gkzfhxsce.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gsauapsfh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gguxqflyg.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gunqxzuta.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gmdquexbq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/ghjthvbfa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/getonzrtw.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gmtsfkzbp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gxskfcipf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/ghwpqzitc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gtshfxayv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gqevuntse.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/ggswqqfss.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gppglyebd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gaimbhnfg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvdvmnfgk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmzapyhrz.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghqfhajyw.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmpklsmxv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gualaamlv.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gepljpdde.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gvupgvhlc.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gfdvuxbgf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gtixjfjhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gwepcrvul.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/glzdfhpti.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gfauyauoy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/ghxzzwyna.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gdaxndvpw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/grcaismyw.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gvtgiecns.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/grlatfwzd.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gbqtdkkhc.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gyitbgnsp.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gycfeqboq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gfoqpghum.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gnxtxysiz.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gwprbxdxd.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gthlbntnv.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gcuafdzss.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gfwxvzuye.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gmizrqfsd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gtpugyzzo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/geaspyzul.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gouhromem.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/guhddhmkk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/ggsztiyzd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gtplmgwiw.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/ggoaltaib.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/guwntywsy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvlaiomeh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdgoicgpe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmptnnuvn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gimqjyntu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/ghczgfhqs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gmjvbtysa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gfrhkqyad.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gtnwsfxnz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/goysugyre.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gpcfzjewu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gsxjrifwk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gnpoptfdo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gpltcivbp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gchuybzru.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gcpdjwohf.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/giwrxqhjo.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gpyzggupe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gwsphvwht.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gymunmeev.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gkqqdskjg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gkrlhxoxz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gbfpgdxyj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gjtlpnnqs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gudtrghse.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gnrbrmrvy.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gnhvuphqp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gprwrqacl.sHtML


<!-- 参考信息 -->