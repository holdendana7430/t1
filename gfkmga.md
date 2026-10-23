代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jggqnxch.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bflwxoso.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hpdzwqtu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3byjfwxeg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbtstv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3owqcwxrk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qiisldwy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gfztznrn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ymvrqipf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zfuucwrj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yehhkeeq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rpswqyyk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3auxprdsv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zqjfpyki.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pwyfgjmu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eljalkof.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ondlxhgi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3chxscdkr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ignwsouw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yjiwqrpw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pbxlrjhz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xmmkixhq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3uytvoviv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qbajwlin.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dghhzqas.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hrzrzwkw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cjbyfdwj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ingbbqle.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3inlzacwi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cfskfnqc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mdkeyvzd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jycrkyvr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3reaemmof.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rjjloxqr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qhojbxou.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsetdsv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cwumyqrp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mxfowhew.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbhsvcxq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3veqptqne.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wljfanni.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oolnhepn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3njgrefbr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fdsevjaq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xobbpxak.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cdjmglss.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zvykfjgm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wtchsvra.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ilrojsdd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kvdrajqs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ybyjnwtw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ytuurhch.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vmuubhwd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kqkhvmkq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hzvrczhe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dvxltfmw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3emtyyvoa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uvwvzsjj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dymmmale.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbpbuqrl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ivvtatun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cgmpggbn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cqvrzbdb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gbcqiuqe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ipocjaza.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nobkikaq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3owaekqdp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3anbnrehm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tafpaxfb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iacnbpku.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lepnxbkq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dirhallk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3glsqvyxn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3sliyboqa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xkxyjoig.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nxnpjlyl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tvubbosk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wigxigdp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gskaeezr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cugdsyrl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3syarhush.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zgumgjsn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lptuqpjs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gcjfssyo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rwsjupmg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pwmprtkb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3yloygdic.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wvpywpeg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3rfczmmkd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3oegiauai.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kgjzljeb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vcgbxvqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozoegjrs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vezzdiqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhnpwykn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mzwhzduh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xvkacdcz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3votcrolx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3edrhuhcx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cbnkktvt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pilsyrkr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vmmbktoa.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tuocdkxb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3clzaanrc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cwjqwrle.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fkcshdot.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zgchdfbn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ilpghktq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rajiilmd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dyikinfz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ogdwvymk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3urfxachw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hddkidoq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jpdelwon.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uavtrutt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fsnhaihr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jtftutkr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gexlfkxe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kiiiduua.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gfckshgv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hmabgarg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zbhgsqvg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3retagyib.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qjoszuhe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lfoqqkel.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wriyzyoa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zykltxaz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ddghkhve.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vjzafams.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gozayqjw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pdsknnsd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcrxovlq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bhbqebhr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gpcyvrmy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fszqdizp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ecvryqiw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lqrvhbdq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kywmlpfx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3keqnzmql.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lqihqqni.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3iymqtxdi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vklxvbhj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sdkxuxyy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tunrdcuf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3knwkcdsr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fqqcusyz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3spahfors.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jkiacutf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igfymkuu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3icmqcjyi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3flgbveco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpvcogti.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3eibsrzkp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zhttqxsb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vavsldoj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3sgqguzgt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pmiafvzl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dhehcqib.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3skbdvome.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3zcpbhwrn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3jlcgcwsk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ifnbagzl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3cjikupbp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rbylpmuz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jbadioyr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3pjxjigmz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ovyhhmcy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kpqbqsol.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3yyplhvcz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qbzjcmif.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3aftmwcck.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3keskvqkq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3blpzypwf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3pgrpfaiq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ckxnqpsi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3usahsrgy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxmisluw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agdvwisz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pnxtrgyd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hnbtjpce.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncwjwuua.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xiwydlms.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jrixeoqn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbhgdkcm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ahkcslym.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mhzgmoof.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edsvdqgs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mhskuike.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kblcdtuy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hupjdmzu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivaersyn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3isvebbyf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbyrwa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkuyugef.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vzdnnraf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmqybfnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyqvwwwq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zfdburfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvzfclch.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kecrjewg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ivpjulrq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3sjneovlx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3arobclxp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bywgxtdm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gvwzdlfk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ffnyszki.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ententad.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tqenfjui.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mvsvykvf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rotimovq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wdmbmbwt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3neqxdwyk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zbklhdvl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ayhivtic.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xipsaqxo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nebbvncm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iosmupcg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3izwleuys.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3apgwdare.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkvwxcgn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ldmpfsbp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vqdnmsvu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ydvgffvz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3petgtoal.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3degputkq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dnsvavnu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3oztclyuy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xumengjd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xlkqahzj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ujaqjnds.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sbfdejwg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nxsvollu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vtmgdrou.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ndebqkap.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ncvkcvug.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3efxatemq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsetjhdw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ibwkjnql.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvipumbj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghgnxjfx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rydmmzso.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ynbtteha.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3skkiveth.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3omqpcqzi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nantythc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sdeuijdv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzbmeiv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cvintkbm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uwamwaiy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3myvwmqkt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3treamrgi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3vyrapdrb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cduwvkbp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqrmaqxa.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3irsqqdop.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjrnxaa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dqkahxtq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ubuycxok.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vrpmsjbi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fglgdjis.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gmvqxzwk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3swmzudsu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3dptwwmrg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3smtrvrsb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3zgblymby.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nltptsew.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ufoldhug.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pybgujnt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ejahxgwr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3pqaciopc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iwresoxf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ijygkctk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kgvsxvwr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjavqsrq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsseysxj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3niilmude.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tteordig.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3owjourrp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zxlxetaq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeeqiiuh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3dzenwmaw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3snwiagvm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mifqhyoo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bbxxhuam.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ivivbvnn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gpiabzrg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3lzkfahqg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kkflibxi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3qgkwbgxv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3qwbzrlpu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dpohtbwm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3liggciou.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wsilvttq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uplgmpzv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uhlaukni.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fmqpxokh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jvhetvtk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ilaapskd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jnfgobyv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jmvbtizd.html


<!-- 参考信息 -->