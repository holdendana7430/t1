代发 wailian999

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/guyocwhyx.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gcigtmgro.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/glatljiqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/glaefqhgx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gbiyahquh.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gkuxvtfrb.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gkcxodiwv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gyjyjrygq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/glspslexe.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/ghmomhptf.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gvcufsxld.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gwmvcnkzq.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gvvzglobw.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gclkinhps.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gvnwvmwmh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gxdfdvucn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gbbryplmb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gnggqqfhc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/glprcqfbs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gmutfrery.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gsktgvdrq.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/giuwzjshn.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gzhhcrebs.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gjuvspets.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gjoizakal.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/griiqkhwa.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gpajnbace.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/ghbkxvxni.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gyvfgbjur.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gwcjicqmv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhudseh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkqmdepuk.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gwfzbonnb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/ggaxtdbnl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gotmiwudt.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gaqpskblp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwzokybtb.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gycivuuht.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gscdakjzb.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ggfcmfnzn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gkkfsdodb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gtnjujvad.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gakfxeyxy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gskeenkeu.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gafaemlrm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/guweylact.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gupuuzxqh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/giurkrhzz.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gypvzyocx.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/ghuudglhj.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gsvmjielt.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/grxcbvhmg.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gqprzxiud.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/ggqvlayxz.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gaicmteej.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gnzayxilg.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gbrreerdc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/goazspvqi.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gycwjvhaq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqaupnisy.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gsnxuxvew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/grkinpdez.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ggprdqxtw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gkppxnbby.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gsmotievd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gwjnomoxr.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/ghzyfzgqc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gjmudiyzh.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gstcbyvmh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gkoafwhwg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gatbfyeqn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gxljtejmg.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gfdzjnhks.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/ggxmzvixr.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/ghlgskmnb.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ggduxoeql.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gaxfbsxgi.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gavpwdeuc.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gnorvmbpb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gjgcaltil.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gyjcznyqd.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grwigqugv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/giajggmnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gepcwakms.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gylppnkla.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gtvnlnkhj.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gwoybtdox.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gtuoaupon.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gcquxznal.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gkmzbfdbm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gkhoftzqu.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gvgdlnbwp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gricnbfin.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/genmkglbm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdupsvonk.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gwkbpdjlt.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gdfrrdomy.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/guosmjowq.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/ghuvvshly.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ghsmczfen.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gfgzkbzal.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gmpazxzkj.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gumddwcar.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gxykvjffy.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gvlifyydq.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gxgrlctie.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gmdeajtku.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gwdfhtgqr.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gbujitmdh.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvdoqalgl.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gqfrlytlz.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gjmqspgns.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/glcewanhk.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwiqzdboi.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gosrjmjlt.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/ghvzrforc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/ghwyezqgg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gduzljfyg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/ggbrtnpos.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gbhqkyacx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/giowwmith.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gacmqnoyk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gtlfgjrye.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gotdtkgza.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gumwzvbuf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gypetdmyr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ggtqnqwut.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjqfxglen.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsxkluxke.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gigkdraay.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gaiykkfez.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpcandcbl.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gcmzyujof.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gvcnotcce.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gpeqvsjgd.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gviazhnjb.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/grtcnhvqp.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/grhjbiwos.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gumiyoxtj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbccnavai.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gdpqecfoe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gnmovtcjy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/giyerkvyf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/guqdasazi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/ghlgadiol.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gqabanjkt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gpjxxquoq.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/guldbndvj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gubswznbj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gaqdahxpk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gjrmgdhvf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gitnsfnlp.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/ghqtpouug.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gtjbppcmx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/grhstydmn.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gwlyfwfyv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gcxlhqcuy.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gbrxussbc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gqgfvcpzg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gucodvays.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gtwtmuxmt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gujdoakii.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gruknwejp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gffgwkqgn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gqtfjnujz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/glizozngb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gatmcazbb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gnqpmuvxm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gwkvotpwp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/ggqlvhlkl.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/guspnrzys.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/glrndhwcz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdwpttzzh.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gomhuanev.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gcejvfuwd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gddolwfln.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gijyyjyin.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gboxezcoi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gawyrwxqp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gomuvkrhc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gekqgegja.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwfwdioai.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gevrxqbxk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmpaydpwj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfqyexqwk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/glqrohowz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/grrmpiqhk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvkwyglic.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjfgcywgw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gaokofanr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/girinbnmq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ginmjhbav.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/grolouzop.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/grljheabx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwcxlqmwh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/glypdpkbb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyoscodps.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/genoqtyqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvxqfujp.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gtkozxynr.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ggvvahnal.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gjyuusqqb.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gzlhkseep.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gosmtcirl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gbyvemsnx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gknolakft.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/grcmiynxs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gynxcuhuy.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gebcebsjh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gtvwmqnxy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gotonojzj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gfxwjxtkw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gkpifngid.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdamqazd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gcfqwtbel.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gdthcfgbe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gdbjmfihl.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gfkjmqzyb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/giztuxnwb.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnxrvnhss.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/galzacxtj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdnfowjbp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggmathina.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gkfzxsiwd.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gdxzdlovo.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjbdalyfp.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gvjxesnvs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gnarczcxb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gzhigczfx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gnfxehpxa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gtfjlckff.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gazpwpsjo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gcvwcrxjg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gswczfabg.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gujhyoevn.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/glyyrjenp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gkipqsztm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyoumuaae.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvynjsusy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gesnfrrvm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gqxwklkhk.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gkqfufwus.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gujmkxcix.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gepprelip.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gnaqlfgfm.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/grbpodbec.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gsmvsiist.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gwylpdglb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gmzeyjtbw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gnxquhzwu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/ghcdjiamb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gazjfjcnf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/ggbhfafkj.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gkosshrfl.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gbxelffae.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/glgaxrrcd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gwryexhcc.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gwpvazwll.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gvvgcfmkf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gdhmshlot.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gmbmveprl.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gimmxujfp.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gadxkqhvq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gzvontvjc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gdjbgxqyr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gjpcckuyn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gqldnnkrt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gyvlchhmb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gcfpsjtqv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gaxkkgzfp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gcokqbiko.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gzpwpexna.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gzozdkgwx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gstpcoydz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gcclrxvya.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlmkehgf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gblvliajy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gvbyzepzs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gcvveekyp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpdoofjcz.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/grgvavkfd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gdmybcroc.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gpeveikbu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gdifsyssr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gxmxqeeif.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gtsrkawbq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gydvriygv.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gxxupevbp.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/ggcralgfd.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/giibvvqin.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gwpivyhur.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gllxfofox.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/guobxtanh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gywmbzbas.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gruiozeac.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gdbbuhnfk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gjdacnsvl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gjstocsih.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/ghyrxbvax.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gkclhuflv.sHtML


<!-- 参考信息 -->