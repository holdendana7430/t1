代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cizzkjtd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3eumnncjr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3erdhwykc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3guiisfkn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ezvpmpbm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yqtqskir.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mtnilszu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sgikqhro.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jvxeibwa.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ezqznkmb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kbrvraof.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3urriirqg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3sccdhysn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ezyvxkzk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fdmaiebj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xovagxye.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ufuogqwo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3eewvnbgl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3akszeavg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezlqoauo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gtoqbsbx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kquxzjlh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3yivgpdli.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3okfuyrsi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hyiwejjf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pszzpmov.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rdqjppzj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3swjrmopd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tugwoahn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ldtuszus.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fnmdwiom.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3btpjdbzx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3exkevqap.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sqrdgtnw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sumiedfi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3akgwjflm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bebihraq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wupaxmza.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wcmpnycv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqdvissr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjvznihh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qbaexagh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3puxpwaha.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3msdfhzoh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kaphsljq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xjlnlifm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3knhhmszc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jdfvyabi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iaeajhdj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zsujcinu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zdwwcner.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3fioxxydb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sghxphis.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bqzvmkjr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3udyfqvcp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ldyzgbyk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sgdzphsx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dlpxyxob.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3myberanh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3drdvzyds.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3khuzdpju.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dbcmdeud.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qduerkpu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xwcenyfq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3psapfjvx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pwlmctgo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3enzmmzxa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gpqpohgv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jptlcpkr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xoeqjzam.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3djufjvvm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lnexlvlw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hyyiovdc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fuawtbsv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pvwdmcul.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ziffbsks.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iqioadoy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jfxjhjue.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ljjdloiz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kicivlbp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pekxlxff.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3slkufdmy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3khltlwrv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3livjzgwa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tpjqfqwt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3modnzcqo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nctxlfub.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ytljkais.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pfweukzw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ltnqbgjj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jtqcrykv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nnplkzoa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tjhtycyb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3laaotjgu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qbuslrwx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lbsrdmbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciezlarn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qvtjreip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goeowjus.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3detrsbom.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lxkxnozf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3utjnbalv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ctuchgxh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3esusyoet.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3npsehwel.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yfeeliqz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zaqscesn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jygrnvjj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cbkzhngs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mvsgqhbk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lriaqowu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3fpbozcil.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ilpryrjl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ffqmkcip.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3epzpguar.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hgeazkup.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dmiwrvhu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iuncwjsx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jjvbihju.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hhdpwczg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bsesbhgd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tecmusvw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hlsziunz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3chvpcifh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xkitsgwl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hkjyzkln.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ykagwsmf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hnjadeem.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pptzssrc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uwiauvbm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xwchmcwu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3udbufada.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3saslcpmo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jwijvwif.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ismwtiek.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xojtqfke.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3uogneazf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dkyvalru.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3axtkcnrk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uhhlxohe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3vvzucceh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pqtyvrnq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tikdiilt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wkbivosr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rtjzvfjo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3scecljfx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ayvqpghu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3qrgcaeiq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3mrystfip.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dprdcfav.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3puqxtyvq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qclaifqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkphquex.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vqxlkubn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3fevglrji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qugkpfia.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3gyzfsslj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zvhneyhu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3bamjahub.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cnredpes.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vkbtqwhs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jfpbjybg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qjtzpilj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cpkbjdbu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3uhqwdwcn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3aelvyojf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xovggtdj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dixiyhbd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vfrucxcx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fpntqqbv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3klmsonac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uiuihqpj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zhinjnok.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ssglgjkj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3rsqwythp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3koaljefs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pdfkegdw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yhqefiuz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pkuooikx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vmetkikn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqodaspy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3podhbmov.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zvvwrram.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hfgpqqfv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hhgbssdm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qgukhoce.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sudgamgu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tpzizssl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgzgohno.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qjdkzval.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxdwxmpd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qarkjxnf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ykekyepx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3qsmxaakv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avjwozas.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxajynjd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzyubjqe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jkxahkhd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jgyajqbs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xiusvutp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iddkfgrz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3prwltesh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sawuvwut.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pbktyngh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3maybyggw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qmgyluyp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vtcemred.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjifpt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hshdvipf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtipsid.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tzwzrtyv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tvsymtsn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ytsazpws.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yggluihy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kmkanfsb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gpsfrqyw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gvxvcrkr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eeepqrdp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jnetgruh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rsgxcsqv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vgrdwiky.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bukucwmx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vbdbxwps.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mstkpibm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbmrxjpy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tecioutb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xohrqeff.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mrnnkyvn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vqfiagmk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ycajldrs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gbdcdpwd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mglqofgb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgysqnbi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qfwxghsk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qjtxaaxs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dvqevuke.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3qpaapfsy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yozwiwxd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fefynfla.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ewdhsgfi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmwehytz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fodlipnf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kwunotzi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zvecjsmz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lyqisvyz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3akhvapub.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmmycyyr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oeyggtzb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3sbmghglh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vynhhjvn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sniooldy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ndljjqeh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3topqhiyw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ilejenti.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3oajsxlfc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cyskwleo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vrkznocf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3slkdnjfh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrsqjvw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kxxflljb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxpalefh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3miljjrgf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jodctpqe.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ysuybgjw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rrmqypfj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fbxpqbub.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lnofyybw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yttpnmvf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vobwzxac.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxsehma.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dhuuiwiv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dlyamgia.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bwglhflw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gythbuyg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3unytrqgu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fliejjim.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzwmgkk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmigbyo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orsqbppr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kvvnppxa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fknqabkf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3hgcllskm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pcyuviwt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwzbfla.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mgejqaan.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vsopkcua.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vvqgubjl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppxxyqbw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gvqaawwx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3brhsjmkd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lrnplfvs.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nafhsksf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3lwlljwab.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3tbibysgu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3yvbxzwwo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3knpctxts.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lwrvkble.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yldvouaz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hvpjbdhf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qkmhkdsc.html


<!-- 参考信息 -->