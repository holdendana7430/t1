代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gsmfkqrz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lwmmtxdh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ofgysrki.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rjkrikps.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hvbfryhx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wcbwucsq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dynxoccu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ltsucwyc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wjdoxbnc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bbltxufi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rnfmkztz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ybebvchn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dluheexv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dneqqefz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zzevmjrp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rmeokrek.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jenskwnk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2agqbgmip.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2suikoxug.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kiuoeyzl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hnjthdmb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hxzxpdex.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qufnwjkx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vmucswkx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kfitjwip.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fywkbfrb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zcnkblwu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lhwnqacb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lkwffsra.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gansilyn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fdijurus.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bfbqeidu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ksufesbq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ecahqnxc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ckolmkix.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cygsppqr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxqnge.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mkjiprnh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2khfxlqsw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2oeyucsbc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2eqauftku.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qgkndwoi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wnppnhjy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bczxzctt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2atpewbcn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cbrtycov.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xlqiguxx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crqbvjdz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tluwtahc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iyfslbhh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zzlobxwg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jerroupw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gtkwjzjn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2atbqggao.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bxryvfar.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfhtleys.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xepdbdov.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vvyoshzm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uhctmcge.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2slavgwwo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2anzybxwp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cwkcbasv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2epylnpdk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cmrqxosc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2spfdfblu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gxftolxx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dynpdysk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gyflrncj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tvuffdgg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hxfnupaf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mmfxwqrh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ruxksqir.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hlplzade.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vwuojuww.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mmbsdnfo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sjtjwipf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rujeposp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ruogtceh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lkfesxbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wunvipms.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rrlhiele.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oclmemkk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2doajtiwq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rqjaiwvt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2txqlsxbf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2stwvxerz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pvuscvjc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2akdyyjrx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ytgleeyk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2arnmbdwa.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2grjdnlgx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ywwitver.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tobkqlrg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2etietjjs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2azlqerpq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfakexjm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xoevtowi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qnrcpbpo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ejwtaday.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wvvdjvxa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2txnxxold.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xkjlgfpu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yovjeqby.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rucjwuih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsgcyumi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2egrclxtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpqvtpsv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wzwxczsf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bprpahmq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tzbgwfjt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iyvbvnxr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhunjhoy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kogomdns.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mqjhiqdy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nvuzzcwe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2erijpkfx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zhdrohrd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mssqfcvj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2kcptnvep.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tbjhkggq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tudheibw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pduxijag.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bylxrlck.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fbchehqs.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gfniqayu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vnacrsuz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fcooqyrm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2aogrblnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wrvrovey.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ffmqeamy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bryyfjfi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2afbbehzt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fczejsmg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yvpnqovn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2joqlstkr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2erjhpwna.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2esbwtkah.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uurefkpy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2angukceu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rjygcywc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qjdtxdxk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2idfjffwj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mjdqzrpx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xxirhezi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgedcn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lyhnwpmc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mooapxvq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pvyjtlfc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yqhqvcuu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2afddtknu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kwraxaxr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qpvwimhd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2trvyjazl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nsipyvsi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ejznkvfh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hdbntwai.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2chzgqama.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mfhrkmhe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wamtbjsl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qmrjhocp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrtgscnu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qnoauxva.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qepwhooi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owxoulov.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lwiezxcy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ilmshsxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wexzjpyd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tlmqoaaq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rthpulls.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wstizwhj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pfzlsfzf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nooqwuht.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xppfmwfw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ndrbiqyw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vevuqskq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fwuzktdt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bexrvmro.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kzeesqil.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ykjraehk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pmxkqgsq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sgilgkrv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2efvxsvmr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dfqeyzgd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2oxvrpfqp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2upplelvs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yssybyna.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2csifpsqd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgmnlgrh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ftjpcmbr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nctzcrmp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2feimmkan.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vkfazaco.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kgmicldy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sbuzytej.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pjzzcreb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wkhmkpmx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ybxengsg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bagghsyt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yafqjhvc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zbdaepph.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nfxtzbgn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uesqcvrq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yajibazr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2istribuz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fjjcqlpl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqefcdrm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ogukpeeo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ayggxxtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbumlggl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2meyoyocg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmwezpgm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2zljencwy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mviyvaiv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yhcptijz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2phipfjvw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2fqxswlwm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bgfmnpdq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2clagegqi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mzuicfak.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2baxvqluf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2mziivssh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2rkwsteyl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ochlpjxj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tdwbsaoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iscjoita.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hknkyzca.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nnymdzet.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zeyoigpo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jfvkstke.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2zybsqued.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2gztlxnsz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2obskjsmk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flufogrx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gbvzjuwh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gmqsonbx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vdrenntj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2uhszgfgi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xgrgzend.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mvtyoecn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wnxdamrq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oglxokot.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zybsvybj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qygebnrb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fahghrdg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2llqizfso.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2psuwasnt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vencdezg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2btiahbay.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dsxhytkh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtkmykhq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kigrzyyd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2prftppiz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awbbelwa.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqwvhbgz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xfycnbik.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2smqglieh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2foxlixqy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ruhbswgd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tazswnji.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwuzkep.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uavmwzfe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xydicznm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ivtynmld.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ebdcakdl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wykgxllm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrtgajbp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ywdaogkv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nlsnhbrz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojptwqzs.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmyjzbp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pctdttkx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2awqdclcc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jgfbejxb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ouqbkcqz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2laawckmy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mhrvbxvy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mwbnjaqk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cjvygsdf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxtzumq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2prrbpzuc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ipfhxaua.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2zsmkygwi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mtdicgte.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uyrwphsy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwyiphq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbphhwzx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xiostzei.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrbmafpv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqtwrnva.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tvxizhxx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ivhftlla.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxcxyka.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pknoljum.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pymmistx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dcugaonb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iaqnanto.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bmzxrlfi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kxuuxrhn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eteeafcu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2elfkeuui.html


<!-- 参考信息 -->