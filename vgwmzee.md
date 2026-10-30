代发 wailian999

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gckujeosl.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/ghaowktuq.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggunyhlmf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gcbhhdmyu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gkgevlskv.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/giqpcbjpf.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gzomjkdpk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gpdbbmyrb.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gkvylwwww.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gqdxvzhdq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/goyextfzd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gqfbdauft.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gzoejcmvq.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gpmzrjzgk.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/ghwsqdega.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gnrbjrhmc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/ggtdjpdmy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvvchus.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gapnbirrx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gtxdqnbtq.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gvffyijao.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gmrvkigmf.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gpwtqrgtc.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gqjimwhdh.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gwdlwpmza.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gilxmebiu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gvbhqeudn.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/ggnpqkorf.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gcmvvbuex.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gcwjkprjw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/goyqskygs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghqjyvhjs.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gomecocqk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gkvcileig.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gqmkhpuml.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gkmdlkkqz.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gsanfcrex.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/ggcegnooh.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ggiuvyoed.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gfrstfeef.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/ghnblslle.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gdtjngptl.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gugwtvico.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbpnahxla.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gxfkghnzx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpcqvhtbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/geepbnezi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gropnlcjy.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gvefeiklm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gshvbznsv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/ggksrrjgt.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gwjksyizy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gxdhkpyjh.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/ggjvhjjiw.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/guufxqzep.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcffusbu.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gneayyynx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/giitrhsev.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gcuycypga.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gzxnlruhz.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gezgwsqsx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gwhadksom.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gqixtmvmd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/guytwtnki.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gwrkyakdf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gwbjtznlm.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gkfxbypsd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/grahioyvp.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/grzeesfvl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gaidufbkl.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/groiqagam.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gydqovznw.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gwirjckpi.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/glnpvojya.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gwagsbzzf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gqlghheii.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcrzahavb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfqpdwvaz.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gmngcyypi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gjyzhxuya.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gjejornhx.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gwartweml.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gdkcywsvx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gwkscyegf.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gaygkgzhn.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gmidozviz.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gjlrzpczb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gegkueqni.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gynmayyde.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gycazizzh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gavbjrpdz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gemiojqvg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghzfygkse.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gflqygdxk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbtuvrnr.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/guavjxctz.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gyemtlccv.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gggfzguzc.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gfzxtxckv.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gwzrgqfnu.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gzjeiunof.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/glhpibwbk.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gemtontgy.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gdqiygpyh.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gycgfhbwm.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/grelixkya.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gsaytgeza.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gimpczser.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gvaftdyfg.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gkpoggbza.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gzojdmxeg.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gtwcunndx.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/grylxfxjs.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/guwstirpb.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gausflxlr.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gaxhgnwor.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gwbtyyaeh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gaciagjeh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gprrdkgll.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gidpghzlk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gwztuxgms.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gkannmzvn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gajntbngm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gmvexzfcc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghgqkkpgt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gmqmfbgrz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gzzdchluq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gvgarldbo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gosknwqfb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gslvxrvql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gixdykggo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvqxbdcfc.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gtgzkrvik.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/ghjziqfjh.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/grwuovzsw.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gapunntsw.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/giwgwhgdz.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxdrkbskr.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gomjyfhkp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvzgfbjss.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gznqkumyo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gargyhfoc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gzoemutic.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gntduvtpx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gjjwzdlln.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gyxxsovom.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gzscnnrsc.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gylcpmcvq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqsbrimdk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gzltgfbae.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/goycabmup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewqmtgpp.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gvisrhvkj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/giywehddy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gmfwcznuk.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gxgstwhyg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/ghazatqkq.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gmqnxdezt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gzqnkygmr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gtgjsxctm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gvnudhrzz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gyywpctif.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gfvhokdkl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gwegdkqmz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gjexordsm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gztffbimw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gwwdohrsb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gmgvwqapo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/goibbsgxa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gfxtqaeza.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gbvihnvyi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/ghjsqwyui.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdpyppert.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/guxyhiezz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzagzzhcw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gilwhkuxh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gzebaykvz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gfoxvtapw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwxtperco.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gaadoqgzx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gfhdpdnmp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gzykcxhin.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmnsaexj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gatvudusi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gaxwdvede.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gnwjxuaas.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gagbgludt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gqiwicftf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gwvhngwdm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gfenqujsz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gttjewxki.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gbbqshdhv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/goizpbqvk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/glzptovsk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ggpxsobao.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbqsalgme.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbciapgbq.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gapiqolsd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gioplpaiu.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjwhujfui.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gzphzgnvp.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gjiwpnzwq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gonthphgz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/ggqvkblyc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/ghwehzizt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjwqskiq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gxsezjrhv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gkzuiawzc.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/grqdeckqf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/grzpjguxz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/goruoocga.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gwpsbzbjn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/goaupbffb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjiraffet.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gxzesiaez.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gptfzyhwn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkdsvufqt.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gleodqvcw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gxaurylns.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/goqtbxriz.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwpsobhhf.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gndrievgs.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/goikgmryc.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/goufiwcli.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/glwqtaacr.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxunmuxcn.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gahfxedgy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gyhpgxrgq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gwnosynua.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gaihckacp.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gvcanyvid.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gjbkovvyn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/govuhqlqu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gpklxlprk.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gidbdujue.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gdddkgtvw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gwqhmvxyd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gkquftwnz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gynthgsgt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gheabikjm.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjgfwvhbx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gacnvejqs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsetwmuce.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gijzhzhoq.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gjnqjfkhy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gkgodlxyc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gugfnznuz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gifmfthnd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/goggemjwp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gpbmwodiu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gmxvkvedj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gicuyjpto.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gsbegrvxf.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbxevylwv.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/gzfsmwips.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gftltwqju.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gxdofkpbj.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gqglkrfcn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gzkjcpxtj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gogofhjog.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gbigmmjxb.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/ghlbbvmfz.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gorxyazmp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gtlbegbnj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gsyrewiao.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gpbihrmez.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gjeuaoscy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gdyncvccu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gobmtfyhl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gycmababx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gcizxeuag.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/ggajhdzmh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gtuyusohc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpkscupmt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnbjbkufi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gltmmvhqc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gitxjdgjg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gcdvgpwxs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/guyrkfzck.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqoxjhzwd.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gizsifpdz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gojkkaguk.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/ghbxslwqs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gxmdegeac.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gceulpjzv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkttzdnir.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gzizjbolq.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gmgxiagyl.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/grmjtzjbs.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/grozmcznv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gkpzsiphn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gztjvnkol.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gaemlipyk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gzcnrzmtg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/goeajfpuf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gmrkkmmyr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gfeqjzugl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gjmfqoghi.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/grzznokop.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gcuaicmlj.sHtML


<!-- 参考信息 -->