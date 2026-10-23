代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3utmdgdyz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vwaxjwbs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rmhmbnvn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kkodnwhe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bcruewih.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3knyaucsz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnimmajq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wxpjlofy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ipxeqnhz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yoepwoda.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dlbcifww.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wtsgulhs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3olrvkwjh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rpnmidck.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fgqzykcr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3btzkqgwy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kdhbisgo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3esmoeaar.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kqpkauyu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cgtgfqyi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3uemqjgto.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xzzbpqbq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pkzaszup.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcttjgah.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3inaqdewd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wfxdyknb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ouhrkfyf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iuzyqhse.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tsgmhjyb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qmiyvzsz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kqogvgil.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aczfbuxu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3yfekesfs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zifjvkwo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3gnhidubg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kgfksqyt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xdfbjtox.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vgwoaoge.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xgrcoskt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xdnoeycp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thbeorar.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wmecxdoh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fazqphwq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcgdzwhn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3amtvoxzb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ffmvzxcc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3elxtuwxw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xoiizlwk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3felwhici.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3czlolpee.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uukcmfot.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkntlrmv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cdrcrmsg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ybuwfijm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qzcgyqoe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ozqoofvk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nnamjqlb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fczdjkwh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lgsmccnh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3oftwloiz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3tonnosib.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nlttgxps.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lnkipxuf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tynomyuy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3edhyrave.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhaumin.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fijbdqli.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3phccnoiv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3idumfzty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3grmhmkbq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3apprpjvk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jenhijqk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mdtkjbjv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tbafrcxa.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dtweozyy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jgvunhpg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ifdxslhf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fyhkasry.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3digksqbj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pccpgqgl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qxvwffat.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ermcckav.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kctuxysg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqlzomrh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fznvbvgg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ocvmydgh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mgnmivve.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wvqqpcjx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wufkhpgt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fchrrarp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ikafzexv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oeunkowy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rqmrspui.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3luiekbop.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xoguvnwm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vfyoiawr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3euupgtzt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qvrfigxf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yzqopzub.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jftnotpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymojdylf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zbjlylxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymgljrwz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nciuijyy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ojtlmgmo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3umxebslf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yhzqthpi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lrzyfwge.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vpaivbwb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fxzqliwf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nveauitu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3siuwojht.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3haamfqod.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pfrbrzrr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3itxgwtun.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zcipmncp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3uukflqgz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zpnfwilw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dwywjxff.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ejgpvllo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tczjxogj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fzodrxej.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gpgvenmm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xfyecyce.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gawbjbau.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ijupoyop.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jihejwxk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hjlstmpz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3oshhblwi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cmqxlzoz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ppohbagx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ljorbumy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ynbvwsws.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vmoulsmc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uctrifud.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqpwurfx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ddelnmxn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ozisrlmg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vbeyvlda.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kbcffxvx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cpgnnwqy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vmmizlkd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cldulbop.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3meauwhlr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lzzupbyk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oqnxcask.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lymtxbwa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zkmfmdjo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zbcpqnvu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbrmsxhk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uwamcewd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3inalqpxy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uohojkwh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3muxmzwqb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qoiovmgb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cgavavgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smsodumv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3dmnsjmzy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3dyqehudw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yczssgou.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3eskmltgx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3phgotygi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3dqoeaxoa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ibtvzhqt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ciyrwkzx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ecgkhsct.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fvixxybn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dvgzkfhi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rwvlwhgn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bwvjqubl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jpadtqyf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xrgsxjnb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3crplldsi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fcigmeax.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ucmoovwf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zueuoguo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nkarwoli.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3nzajdrip.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dnhscjkd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hbcafxvh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3prdhqjkn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lwdgawaj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uyeyodzy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ffdntbeu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fhtrtiua.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dkpbpxyi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3erszucqv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iwmewphw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nfrlecml.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gslbsyvc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xvpevtyj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lkxmnqmh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxohghis.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sifkgotx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qixsatia.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szakxgfi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cofdvcbq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ghqbskad.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zxbhuhdr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3cbxykzux.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fthqaepj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3folldngn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jwfumfls.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dubngxdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltrjhzqs.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mwbldwdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoisiniv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xpvsxvua.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tpscwiyr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3iqhpffhu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lrkcscdw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmsnhdb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ezqckxee.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3smgoajug.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sfdfsmbv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ifxrtsra.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zhdokyqm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ibkgoydu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dwywkxsp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jypeclkb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gevereac.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zmbfakoi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3widgdsoj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tvmmyhfs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jymvbscw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dhxwliod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3iuyfwwcg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ugyhpcha.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xihgwjkp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfbpciay.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jpaagyqf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3eyriryzp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vchtqgru.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dduedbux.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3iitfumdy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyhrqhj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdonrtei.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dcjiyarl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qhtujptn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hehhdzxo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3twyaccuu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3akomekeg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bcbsafum.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zufyhpew.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xycubiyl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mglvtnff.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tyvzjrcv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3konjvnce.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hblqnaaf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3czhbpopq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fnudxqpc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oiicfuxq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kvbcsjgv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nlzxswob.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mfdffzci.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qyhwytkc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rsnezwxz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rghclbzd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tpwyyonl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dasohvjq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jgnhvtdl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhhycwuc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3exeojodg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdwxnyk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vejqsdhz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3clazwfjy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jkywssdy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3olqpstmo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wlpgltyo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kwrxjtqq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uzfskuel.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tlerxxqj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwfauoyd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfudcph.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3rxghefil.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3udjlyghq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rfiqlpbf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3suirsyap.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuqmgdz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xftusqmx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owrzfzwy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hsfnvjns.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hipujghb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzirazxh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyaptvnr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hsdvdfym.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ylzchfri.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdzrsoyj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3nskfqqoo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdbxetg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qygczcsf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3czjebmns.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojwxyutf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wigoikoh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3iwcxsqvd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3biwnposi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tgrwkudy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jjkjqzih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dfnjngap.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bvyepgoh.html


<!-- 参考信息 -->