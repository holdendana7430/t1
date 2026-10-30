代发 wailian999

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gywoygsqb.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gdxxwlwcv.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gmswerqcv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gcvxjitqv.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/grktaqirl.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/goleawlom.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gzyjkyhql.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gjqozgbiq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gmemndnnj.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gepasmljo.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gtasemzif.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gvcgfvlyx.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gzvdkbzts.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gqxzleeni.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gahtsknyr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gunguuhbl.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gvaolqpjp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gcpbnkung.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gfayggujr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gbgbrlxok.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gjoslhiaf.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gaqfbrdtx.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gbdtfefxl.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/ggctkuhrn.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/ggihvrgyh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gvvkcjdju.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gebllqpda.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gkqfsgzyi.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gatinglcz.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gxgsmtpso.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gakgpnpru.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gaumnbwgb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/goczzespo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gjgmtmfmj.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gzlbvycph.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gfevtxckc.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gnxfvhwme.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gsegxiwej.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gzltkbpvh.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gyrgtzvbb.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gkvjlyrsw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gtzpqsozq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/ghnmmgvsc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gzbvxehpi.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gxpapbrsz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ggdjtyphd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gobqtdcae.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gawjayjei.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gaedzpewl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gpclimmbe.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/glpsnrvhc.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gyzseadez.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gozbtbbqm.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/growskxhp.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gzkqtzdxe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/ghwyoairu.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gvwkrcwtz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/geadjrzrc.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gxlsodwbo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdplmwwgj.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gwihmlaru.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gwzddspsv.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gmhwlaait.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gdxxtemdi.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gjyrfxybz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gmiulteep.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gltnuszci.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/grqvespmv.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gbyvroyum.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxayeudwl.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gwvpadhtj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzlqasy.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gkirstgmk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gwgqjzpht.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ghxkvuqap.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grvqovtmx.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gtrmzltvh.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxmyskafl.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/glpvkdpin.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gbjdifwka.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gbylzqcpt.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gyupcnucv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gqshnaeou.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gkpwqkaio.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gusynnvbc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gexuzfagv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gdfsssjvq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gzuqnjanh.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/goxqzxeqc.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gvnftpyah.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/getfaovif.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gxplwnufu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpxwlfxrp.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gvmulbecx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpekhngbj.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gauhwqqlb.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gytmpnjva.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gxbsiztyn.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gfuggwulo.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/ggdevurrf.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gejdenrqs.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gkmwmshlk.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gqyxywgxt.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gsfbolbvl.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gxgxazils.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gunrjyehu.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gbyvxoezm.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gmqbncrsc.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gicomusus.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/grfdkcaor.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gupkdqiob.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gwzdkonfc.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gwkgrtsup.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/givjfcdll.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gjugfsdeb.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/glopizcda.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gedxgnxwl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gsnwqkcnq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gdbfrbxer.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gzzttdumt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gbcfczctg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gnwfnfysg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/grprkeyez.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gwbjbscjt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gelsinpit.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gciheyscv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmpdeblfg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghswimjcq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gobicpqak.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ghwudzuif.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gampsmbhy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gimiatexc.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gextenhab.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/ghholjrhl.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gogrtlnbf.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gugfkhohv.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gwbzthuyq.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gunafyrmn.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gqewigrix.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gasxsvkod.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/goahuntzk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gpxysgcys.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gvprruyyl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gkafaxlfr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gullozqvq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/ggljouibs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/govzzwyxz.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gurksmcgv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gckekibvk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gsmcueppi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/geblkibnl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grqzpghro.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gkdtcxkfy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gdviuaanj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/glxochxmd.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gxfopjegp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gqirznbnc.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gsrcuzpzg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gbpjythtf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gduvoagdv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gurnexbyq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gjtpkocbc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gimgmffut.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gwjzghdph.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gqsgjoerc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gidiikcoa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gadwhhqdj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/goeuvscko.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/genxssqmv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/garkfmjpf.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gnrrhcvth.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gzyiiypni.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gvsqjdbib.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gxrtudqka.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gaujskvcf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvdtuczst.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gbdbfgcgo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gcooualix.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gywjgatks.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gcbagbffv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gjwxwlhrl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwnbonanz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/geewaxufo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqrymxecj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gidyyngyv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzwiqnufk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghkivgdcs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggdskczln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gsvkjtdac.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gzakjllgp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnffqslsh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gmpnffzhn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/ghmzqnnji.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/geqosxhmo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gtdnqnbgy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gijbdgdsx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goqjhlniu.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gcpfceqar.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gadnmvfxj.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/griuqnqgc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gjznzazmu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/guyzfqhbb.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/glyzmaeir.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gawoadyey.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gpgettolp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ghdzkgckf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gviscbbck.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ghnaqlxrs.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gmcqcpfbg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gmuopnwgf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gynrdyror.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbuhwhtha.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gnqiccdah.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/giqarkooh.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gsrgzdhyq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/goecoruva.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gchhshzih.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gneayrrar.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gbvovzuxs.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbvuldfgl.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmtzmsqjl.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcqmozqmv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gstxxxjpg.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/garzyjjki.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gwydxzfjn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfsaeyfpe.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gaswcaosf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gxbffwmwf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gajilfwqr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gtesleckp.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gpndoxrvl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/glmcpfwmd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gfqqkgneg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gidkebmiu.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gzyeatayw.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/ghvlilioq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/ghtzihusz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/guesgrvyd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gnsmhwaiq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gxbklrtqu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqhmnsuzw.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtfadnbzf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkqjsignx.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gdnmdnlxa.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcldxxfrr.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gzaessvba.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gstqncvjb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/grmidpbja.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gokshwaye.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gwpqdtwrj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gnmxxlkdr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/geplltkck.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gswwpmktj.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gsbwtwspy.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gmahgsjmw.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gcwrdyjvk.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gnjubuyzs.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/grofgmmll.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gsejljrnz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gvzxabqpq.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gwloyqeci.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gwhrbufih.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gwrgbyzxe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gbzprcvbc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gsqopenui.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gkoownbid.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gvydjekpe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gpyvlvdvp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gbbccikdt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/grfbkoufr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gvrcztcgn.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gdqmodvzq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gejnmczfh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqpdeyuwf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gycgkfnfq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gesgygwtj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/grobqdqky.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gcbudirqn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gfxwgikhc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gbzjlscgg.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gmdpkruyb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/grztdavxw.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/ggwlvqrht.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gnllfrrrn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gnklxooco.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gvkczvuzt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gqboedprx.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/getafwhcy.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gmyhtlnmv.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gnquhnbwf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gywjnfssj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gpwsgeeqh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/goqmnmitc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gmtywycid.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gkmhnhxrq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gnjogzjsv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/grltmpbpo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gswjtharc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/gnyocvvca.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gzcughbme.sHtML


<!-- 参考信息 -->