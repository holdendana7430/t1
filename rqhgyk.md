代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pliuzmfj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xosnhmrc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wihzumsb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kjffsmeh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ixemgvcb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hlwnlsmv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ruyiiyvi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2foywktxi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uexiaayz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dzcfocyk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jwidkszm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2klsxsgue.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xbjurwql.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tilsmsgc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hftjdgnn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bwfkwxjm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2armsntvv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wmkjwtln.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2djbhtoxg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nyzokycl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2klesuovm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vjbhkqeu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kgjgnfyf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2drztoysl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zlihxnbx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2mehmvbxl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2clrvgjhc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wfznwcer.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zlkgpnpt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gafsepoq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2oemfdmcr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ncjhfmty.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bklukhfs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oopgwrpl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ekzkxlwi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kkgwkdat.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ksiorubk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rovdspty.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jyuctmnw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pnyttvkd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kxmnebxf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fepyvkvc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iidjiprn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zyenndbt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezvbybgu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2tfhbqryo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2atmanisz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2smfyuyck.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hsxiuamp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ilxhmcug.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfgtfyxw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fvsukhho.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vvzsvets.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oewwudfd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2awvhfmxb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbufjgsq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jzyzjizj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2trjtxafh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bdgxpcez.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2umbgpfgj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zmpnplda.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2koyhvnly.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ovtwiqbo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jxxtadua.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xwxxngzc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2snmlpltg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wmrmcpws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cqjsqrsd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tgebnpvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqyjono.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zlfotljw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jfbluhab.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nhqhbyvd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bahmxyxh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wntdilis.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2bfpwxkbt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2eswkevqz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cdukppir.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nnrxrgkw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cgmvoyls.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ghrztzlk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bnwtqtny.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2suwfvdvh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jqtsfeju.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tjilbevw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2uadnkzxd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qsyykxpu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xjmwbjub.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2msxcrhkr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdohdatr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gpwinzvm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2neniydpd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bgqksrbh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2naddargz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tqwoyqko.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srfvmlxo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kehuhylq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cwdjjwbi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2renygrru.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rqwooddz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ysusultj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ujndljly.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2atnbsfji.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wnjrhbae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cffiwgrr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2csxlitnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmftudli.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2riwrrued.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xodbnlrw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gisztnlq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sjyfjvjk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hzwavxis.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rvxftcje.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ghjogyfi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fbpabeyw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lsunnmml.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fsabgcah.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rjjvwkbw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zdysblcp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ndxgshsl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2gdtdahag.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2drteprhf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2evbpqbya.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xxuqnirk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2glsppoao.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rvjugwdp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2snfpclsn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nkebpzfj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qelpabjh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jjdcsgjy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eosmtglk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rwjqhfye.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kwmseitq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mdwzylbb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2emzehfxn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2azgfuows.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yndjzdzg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2soatfjij.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nsurxbnu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bngydxdt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qeocicar.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2znfipbxr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hlwqllve.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2juhkvpbz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2opzuunfu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rdqoeyye.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2djbqkonb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ilqczlav.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ruwcbwym.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2weosumwb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2agotcbmy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ssrgyzaj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wxqgduet.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2latxxmmf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hwcytvhr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2viomzebx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2voblrzco.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2eebosbcg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kpfqjwvo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cnmwwvne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lctyzqlc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nzbalxmd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gogrhqxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2airtkcfy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2umuqmxrw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pfzaritq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2vafgwlki.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2jdzpilzo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ydzfzctx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jfzqkhlu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yoeeelfj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2sgfvjhic.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2galkuckl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lvzgxekp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mxodwsad.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2efkfzwry.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2htnhqtsq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2gmhywiel.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2gsuiumss.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wimouqxa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ggfhfoid.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yanyfpms.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2evxqrpui.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xtayqxss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pecyyguu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2hzjrbdrx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wntaxbye.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cwuhlush.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rsuhwslm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ntihjqyk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tusskgta.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bzldtuok.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2assgaewl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nxrowntp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gyqlhnvc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ymbhvhxy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvegqywd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2trecmnuf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qanptrsj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkltxtsu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shdczova.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fisrocux.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mxloxvub.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rglpvlsn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jeegtnid.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shdojixm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sximjyiy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mhdziqlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsukdwez.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2shnvjjlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpzyftfj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hcbtrkww.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vedrcyjp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2quusqzej.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yyckdwih.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ytfaeomn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ixqznnor.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2llunhfzs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2oetfxyfl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ruidpzcd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xfwcvkdm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pkqdaxeh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqbbpvkh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wwolmtbo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nrvkogcs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vqfshxbp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2kgoncqng.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vmzpsree.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hlvtctyf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2yfhclxwr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2bjaacilc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zkrpkmmq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lnurswen.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jazpfaog.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2drqawnac.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2coogsjxj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qxqpffvx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmdpnpk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2chvsqndh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jzgidyhh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsnxgrax.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mpeyamkz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bfxjrbjq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2oxpyafpj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jskuszhe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2phsefkes.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hrxssjdp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2clncbbhg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzqdzelj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ayieruvf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kipaoues.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jqxxsulm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tbzsauxc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqwngzmq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jqdjmgpp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2skdgyewe.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ribvmtql.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xpqezbmv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qlkcwacr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2yrjcmxdx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qaygqdsn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wvtirfev.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvyfyyu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kzydreoi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fpexfvvd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htoivavw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ptqgizlp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xrisuipn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qdfiqpsp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qfyotzli.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrjzys.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxzwhpm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2xrwzlwrg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2srkgngtn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dlvdlyca.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dcnnpjxx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2cqhagiwh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnlznjg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2pikdbxvw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cyorazgm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xpaqnbjp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nuyivgsu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjqfucm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ajiqjkxw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlzggna.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wugtxikg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opnuivlg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2huuwozmt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dihyhrqm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cpapzdzd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2poierstc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkbbvvcb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oimpfxlc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2onidhcgn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wctcesbh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xcdyhrln.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2guuliqfc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2begnbidu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fmouztnk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmbzvjy.html


<!-- 参考信息 -->