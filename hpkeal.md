代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qhxlsjnc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hwgofxrb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bpeqkreo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2labxyusc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hhrhxwfz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2yidxzpay.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hkoflhqd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cvfhlvvm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bktfobsz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wmodhovf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nndomfjz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ragiahdf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tlnzcvqe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lzhjwouj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hwssotbb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fzrfhdey.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rdospybx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mdsehfcc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cbtfoehd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zynciqag.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gpzmgfqg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bczshesm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2shsfgeka.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dvvxeibn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cjvywzed.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jgmsdhqu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2taqtwqrt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xpfyaond.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dqlvjqro.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2orvlavtd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ayythotn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mpcfapgy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iwlgsktg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dzczcaqr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dlrzyphn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xhoplepc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rsqazrey.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dlhpndpc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qdmdstkr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvvqogqi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ezjzpvdg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2upjfllit.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnlixbhn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zwzhrjpo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cfafkidb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oyucjixp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2frogvrbs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fezljncr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mnrmpyvt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vmcmfxxl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zcpoolry.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vmocungb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gnmxeykz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mhmpdgdq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2eqacokqx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yxkanviq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2eihpddwl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hvbshruf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rvliobmy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2amfzruhx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lnrstldt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uvrlrmxv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mvdecycm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2unhdqism.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jlvxjubb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wbdhwibw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cmlfmrcb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zginrxps.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2umcaccro.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2htoghpul.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rowrvgqs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2iaumjpdr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2meyzweit.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kvakzhta.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wfjjtjsu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wuxpftqu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2aedbkcrk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wfscmdfh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tihjcnzz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fgqlkkln.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nlkckkoj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eojdumif.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ukkscffm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uhgqzsoa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqlgid.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2htjtwoqu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2mcumguwm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwxjznke.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2erlwvjox.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lbsdmqzh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2amjpwuos.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jfzasege.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rznnvxua.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lfsfuidd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jlgwxzex.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ovxkscsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieejniuc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2szpbdais.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvozsyld.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jcvamyed.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fgzlpjfr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gmmwoqor.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gbleahlf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sifjigob.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kafoizls.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xvbebeaj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gfuujceu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qjlrbtpp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mjgdnagw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fdnztuwf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2krgikmpj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ewsvofre.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oldbpjqh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yrsavvyv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gosiccrs.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rekgeiyb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vijttafi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uyfikiwk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mwwvoddy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qsinemlv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zevewpbl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lqwiotmr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mwnqlrof.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ndcouewk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dhamptow.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2toreasfr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2paxxkgts.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iyosscnf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2scoqswxn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yiremmol.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pgeeclnj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nhznjljl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2viiddfih.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mslmubgb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hqstmtlk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gkczwdku.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wnumzroo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2cuknpphe.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ufugremv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qwlqthwh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vwyvulpr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nigmdqdz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qixzsmmp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2atdxywvq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bjadbwht.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fqaxkldz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gfrvfzdf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ybsgmjtm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vdantcqw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kllumsse.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2egvwsofc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jjhawrjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pydfsvtm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2feztmeey.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ekejdmrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqbgayeq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wnpzcfsq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yocczgxs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hwentxwq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pikxtbbk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jddcggba.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fdqyjbsn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pntdlour.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tvvpsnjq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2alygcqql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qbppnclx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bktztqrj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2hsujzuoh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vbjuuwll.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rrpdutcf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2aqdtnstm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yyjltwxi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2uqfrvebo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vkdovyjh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2drvyacan.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xmgybpll.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fbjdyias.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ekszdfry.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uyyizzvj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fsgavgni.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tyrhbzzz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukuritpm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jsihahrj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2tyxtxslu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2clcfstjc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2voeicrfx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gipualxg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwxijavs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xtpikrnn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stuvsouj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oyaedyjk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bofbbxpy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oyvolrnl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2frwunyhv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jptijzek.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilvawvwl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hfyosqht.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hytcctjg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ufzgwgkg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hkdpxpke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igofkqdb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmdzmtqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aimqwcjh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzjdeupn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rcmchfvi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2dctxtumh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2neyusnax.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tnulluuw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kblddrji.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gnmuaooc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2erxklelf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hkznjiil.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2rserfice.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2aimeqzie.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sefyhvwx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2psernwtv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ssxdiagm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zxmqgufg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2uvjaqqis.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2smepdpfb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2htimhcew.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lxyiykfw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2szjshqes.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mjpdazpx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ifvflwip.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sgyizhaj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xexcbboe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wzcilzie.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rjmlcpoe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rvcxopjw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rbwojbja.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kswknogs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ftfjjafn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rblcuhwi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cszawpgv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fkogmfvp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2uixdhkkb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xtllbodm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jpcfgsti.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qpcazenk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ykizorul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2onkpebpq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tmplzkay.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2txczwsyz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bwqfmmxq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ltjjnjcg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pqgqrfpm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trucjxyk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qzsmbkcb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2knuljmfj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2iumooobf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pgkrmwog.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ltrxrgga.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dnkybzpw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2grmatepm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2biossqrf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mafvrpsk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwjqiwqi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kkfiuvee.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pdkxxdli.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pdyengem.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2smtlcwvm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hxqwjbjl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vzesmgex.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kaksgrsb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zyzopqjz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bmlzxpbm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2juhgmdbj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfknymqk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jcwrlcth.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2eeliparv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ekfwonkn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zdkpmuzl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ikqcsegf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ewqkiqqy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2apyooulu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqbfqfb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vvvjvmht.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmpbrmth.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ribvhdto.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2axrreyaz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2djoqxryg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ojdsjkxg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fncbtvrf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qhepqzmz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2blprtyvi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ttsrrvrl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdlfoqqi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2exfhcbgt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hzbulmwm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zoniuoki.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxhyak.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bxivjdlt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2eoheiiae.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gjorqpej.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pucetuuc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kxbnubzv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdmijuqk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aklrrxok.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2vsyxtmxy.html


<!-- 参考信息 -->