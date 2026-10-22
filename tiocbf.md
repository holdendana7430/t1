代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nrzlfxin.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xlssleiq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hjcgolcp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2skyqlcea.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2eddkbvij.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pmsuxquy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ctcimrnh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2opgiogkd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qhftqbwo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lhpfpjpn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yytubmmm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fwpanrcs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2coicfgth.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2txqiksiw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gjygaotx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2anlrwnea.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pcxbgskk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2npxgwgot.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jgzewhfw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vdpedipa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2udwluqgr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ngwkywkz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cjqygidr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2chlacrzj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ssikbmdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hjskdnlm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hspoukhg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kpcsxntz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hssdecnq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2izndhifk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vyircojb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pcwqnlxi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lthrhdzp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xnlyyvvp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oasjndnt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zkbapmxj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cgbyelzo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gachwgyo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wudocdmv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2doevedfe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bnilockd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ubekwyvw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlgqyruk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpgxxval.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czvnotzi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vrsmvxwp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lrcpeqba.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pthjcfgd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jzsrilnm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2smmaonxb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2iuptfpqd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xewpwzmw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cwjmagun.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2smgivtwv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mmfockuo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kpnzgghz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dyitjnln.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kojuamvk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wxubdguj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mhyfwdkj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2gxbaawtj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2oarsrfax.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ysbwvxpo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vttguhvq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jyxprije.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2eotuozle.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2igieottd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rohrraum.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2sgmnblye.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ykhmsdre.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kwxfcqaz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2psyevetp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zbkguvmg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kyaqbvwy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2srgwvhzg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fhlyuala.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dyvdwbsj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xclkcwru.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jrsqqaaz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rxphpzkd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ozkjoryp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xjodjjxn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qqchtbti.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mfmswgdr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ivnbqtyv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gpyzgkeb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hehwyhcq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wnpgfzus.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ortapbtw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gdonzqqz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rqnbgtgy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kgixkrxx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gloxdxkj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ldyrvovb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2irbnxxyj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2uzmmadhe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2meiwdhfn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2blapdzsv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nmvcwxao.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kuginssw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzyjjhwm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cfapwqtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fllqvnck.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qmpbnnfd.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2uvwltmej.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uswuunhc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cehgvbnk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2akjjaxlt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lvfkxllk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yrbsadyn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hzoajrni.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xijdckpm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xglewxxu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lqmkcchw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hrjhhcya.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2armfigrm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tozvians.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmqmyr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fslezcdd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xnskttwm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ukiwbrcd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fjtqqqpa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wgvlnbkw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2untoglib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tqfitnox.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xsslhgca.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zqmdvcmt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bhrqfuyq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fmbnpmom.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sfqqohbg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hiivtqtr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bmbomxnc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nznsczkc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sgiqyenn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dqdvyqjy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xfiyhkvn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2juqbwcuk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2czjqxyfu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qgjggtkc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vjoklema.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wlnpavoy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gfgolnxy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zsmihptu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bjnzgxyp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2tdbqczkj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2chroursh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jydhubta.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2flqejiac.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vvvauolu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2phbhmgwa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mdeghbus.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2elpzkqhe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gibiguxe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ainokdmd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qkbojdsr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jmsboqzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvmhwnaz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2eilzjjrl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wyxhbfos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alreuxmw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2osmnkzxp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gsqjalkb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gxjyozbb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cmpohhfu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pqmfkarx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fhtbykks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lioucmil.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gkctbvbs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ovklvbac.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pjojcyqy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2aaulkmny.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dwcncqus.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rjflmvje.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ldwrjtvg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fkzcofxa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cunbhjiu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mseimbhl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mdmwzqkm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jenhhsiz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2uvawffuu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nqstgxun.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2azfnpuxd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hdiztixj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwiooqsu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dbkcyysx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ummmcvtj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbosnagm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ikujmrqh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ijfbavto.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hbkcxgog.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxvavcii.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zuuxkxdc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzvyswxi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfyukfbf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tyychzfq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zmzecoth.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkfwubae.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2igizqsbu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2intqukvo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwfxtvyv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2avjkamtg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xotehmxk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xjtkyskx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gytnhthw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opczcoct.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2nynerkqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzppxclq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2cwuifywx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ohbndloh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vngsqend.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lfybcxcc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zkfyggzr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zsnzauxv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bloqpgix.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2dtlkoizu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oujytvxj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2dqfadflh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tettzrin.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pgrhxhdi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nzeembkd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vlfuchob.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2flietvwl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dndafjwq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2updxgffh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dinqwods.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bxqznlqr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zxendbpo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ukjohsvl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pospnfgk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qlspubhv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nxdruryu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rovritnw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lyxkjybm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nneucsam.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iznfmcpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdakvcv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tpwmajku.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uljlzqje.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sgkwvmlj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2aytjpiln.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2uwbbcktz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xqeweflg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2idwznggr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ufqgahdm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bxrixljq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aghbwnrg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hieqyrzc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2icvuhvze.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bimhhznp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pwsyfqdw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwecmjdk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zyrlvuik.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2egadblxk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tbibqiai.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pujxronn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mbdbjstb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fxtldjeq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nxjqqppr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2aayjxuqs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2bumzhyry.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eeuwplhl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkhcrrvc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2frrkgmos.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zpnldlcg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pnmrsitt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkkyldo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2txxkdwrz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2euuhckba.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xhcbscsi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gkizmlyt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2fvpetvqp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2arzolgzz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pumouglt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bywkgxoz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iywjpczh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dgvxumwa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2audbccrf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qrfqisij.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2utcdhscw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ofjiwhtq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwcqefw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmugrzul.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vkdowywx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgdscene.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cjqmsohi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tikseasv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dkazcldy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swqhawbm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cylwzcch.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjwuyrk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2acfjehnl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zgmlcpeu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2meyfngjf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpcbymxk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eomjrsnn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ohqntaod.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdngana.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2alepdzzf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2voywudui.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eoldftmn.html


<!-- 参考信息 -->