代发 wailian999

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gxxbrjhmb.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gsitrfjez.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gewzgnlus.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gwfiqqovp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gvcaeiwxq.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwhlrkptv.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gtlzsvadw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/ggpohjqoc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gkroqlvvb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gkvimvqnc.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gkkwtlobf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gnqhsiaxq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gfnxngbhh.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/grsjrwerz.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gczmcsiup.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gmnshtbqk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxaeguuly.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guyibwokh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gmxpcvjck.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gctbsldlz.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ggbdwqgrf.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gctqqciga.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gvyelxlbx.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gktiyiqxa.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gwrrijkyu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ggbfvlbqr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/ggepfhnqx.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gcxzxcpob.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gsdvdlmoh.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwxyooevc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/grtdbllfz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gxcuhbqfr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnunwtvpo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gliypumhh.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gwgmbvrcj.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gcvlskyfm.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gycudbyol.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gtdsremtb.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gaijlzalj.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gilnkidbl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gxfdywkry.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gdvoozjsk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gkmqujcue.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gisgqdjgk.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gvouvxthv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gimmbvjut.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gsiwxczpg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gdxlpbrme.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gmkuflowg.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gnrvaeoui.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gzawjjaum.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/guvgtklhy.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gkxxvrbvf.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gmivqnmhb.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/giztwxdru.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gkwkzwkck.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/ggmdjoaxe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gqycezhay.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/golytlfvg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ggcrdxgzx.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gtcsxezcm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtkpfcnwn.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gujppofwc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/grmyjkfai.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gsdliqndd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gxoldudwc.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gbvjtkucl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gtftqdblm.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gewituxzd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/guqhkhroa.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gdqboehye.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gfzdccuzz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gnxdlnwli.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gvsgftcvi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gxwhnqccj.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtzlnnejw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/grjdguatz.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gntbgdfpo.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gyjhxhibu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gedvuyzcj.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gfbaufqoq.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gzoazddqp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gsxxavnst.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gxnjbfpif.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmbdkpqyy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/golfpbtro.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gjwvmerda.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxchnbo.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/guzridhzd.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gffsukekn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gnzvhleeg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gnwdwddco.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glrcgiabf.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/ghombkvcz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gchvngwmb.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gbebdlwcl.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gteuldygz.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gcsuvnpqi.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gevysndks.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gxlrihyfv.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/glgwleyph.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gupxumckm.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvnpsjfzc.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gmmuufnml.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/grkpkgngb.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gemgfvfhg.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gaisqkysf.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gsuetgdwk.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gvaluhcos.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/golgotjmt.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gndprzmgq.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/grxukrvvl.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ggcdocfhu.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtkazjqmt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gjwbkxhpg.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gerkeozsb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gvxhproxa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/glyrbqwdi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gckerbxhf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gqsjnfczy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gdndlcpmd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gwvlmdbqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gdlhlkkej.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gtwelvaaj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/goyknuiwl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gykqvcgdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkzxggsva.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gagcwxyya.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/guxyfwycc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gxsrtcfio.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/ggyofvdqs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxaqzdusy.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gtgsbwaqn.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gepdtznnv.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gfiyjfzuz.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gpwwrjhpv.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/ggmudyriw.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gzprifuaf.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gxwyzwlpm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gprwtdzab.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gfedpkhak.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gklcqeglw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gdphfelvn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gzymabqwx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gwwifiqwd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/grlwfyfqd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gqzrizhwc.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/guvfsyviu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghznonjsx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gmjsgazdi.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gpayktnyp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkjpsdifs.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/giybrxtuc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/glvqztwmi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gyisgyryx.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/glnlvlfig.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gpomvlbtl.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/guarvpsmv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gbexrogad.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gdvabhhek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gyygvvrnl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/ghrdaszro.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gbmfzqpmz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/guatzmkvg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/glbnsbfix.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gtpqwcghy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gxduobjqe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gkxanmcsq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gfshbezuo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gvihwfhae.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gkuwzzxto.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/grbgvmmuw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/goedjnqtq.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/grscubzsx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/geuxzygib.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gcpgaspxo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtpeikwwr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gmaldkfmw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gysbpkxbu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbsontcsf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gkpkkedmg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gyzpofqkh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmnhvxuqw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkvquhgxh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gwphnclid.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfsfacnrl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdxeuiys.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gtzgiguoj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gybizqdlm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gntgqymeb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gyomuykey.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gmakykxpv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gyhhamejl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/geststjnr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/geepcghzb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvfngfubp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfxmwzshi.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gyxluewyj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gopmxkiiv.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/glpoqrmdt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/ghkyvexiy.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gidmfkyft.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gxqxddcke.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gobnhaqml.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gwxmmqnms.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gwwvlrmgo.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gbcehmtqh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/grskaypmx.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gememvutc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gvaatddei.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gigpxihkt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqxljbxon.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gbolozetq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gnwzzaenj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gzucjcmrs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/glpopbspa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gwlrnwmuu.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/glomnzpni.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gtuqaosub.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpfdxdwjm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/glisjtlzv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gemevxyab.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gszasozpr.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/glitwfihq.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/grncmcoxe.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gyetfkapl.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gerubbipa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gepriqxju.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gaacrplfx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gouixwgbv.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gkochveut.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gxnmdpgck.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gljmcnmaa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gjcstdjar.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gpjkrjmic.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gbssiruwb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gvegfacej.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcmxemjaf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkrogsjzy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ghbxnofkq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gsqjeyjob.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmasuezta.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/giebywkgp.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdaldypwa.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gqfsbcqqw.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/ghmorrbqa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gfeakspov.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gedoezrri.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/ghclqqtuc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtgxziomw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gfvoyjqiz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gtbsppger.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gozsgcdot.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/golftcxko.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gnfffajfm.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gaogpnknl.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzzrcyl.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/glefsylxc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gsqsbsqiq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gdyqfrkxu.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gziwttzqx.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gtgkgfgdk.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gtrzpmpir.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ghzmvlack.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gatuxjrwv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gpklrqrie.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gkaqotxuw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gpagsakkh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/geqfojzlx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gmoeekaie.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gzfqrgixm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gzkdxapda.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyixgxknw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gersbwbca.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/glatonasp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtxnryevv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnikamnid.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gnoxupocb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gtmmgngsm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmwpmnhtn.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gtwikushk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gvshiwkxj.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gzciwihkw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ggvewjzqu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gcbsbhyfj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gwrgtkkta.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gljqmtsac.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gwqzvqill.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gjtjziizs.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/geluvawnt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gcpukrzly.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gamdstlyz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/geimtztmw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxsbysrjf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gogdxtotn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/grabfofiw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnhdqcade.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gsyxkjowd.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/geqelbust.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/ggukdjnza.sHtML


<!-- 参考信息 -->