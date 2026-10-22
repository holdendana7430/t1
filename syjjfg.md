代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lsnngrpj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwdcsyi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dguxpyjf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pnfoluph.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rndrpcfj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jdidcbse.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fyhmalkd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qfmuxiri.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fifvbunt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gbjsordj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ccosgzmd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cebndhwd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kedrpwic.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qulckzgy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ujlterdq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kyqdvtal.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zreddqso.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qlbvrohl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2anvegimy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ovyiiviq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2oeruyxnw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nogfhxla.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iuxszrge.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jfytebei.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ipeasrgj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fptgomsa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gttoznrg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bwfpfwcw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cviyhqdz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qvfiozau.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rhovifat.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fizdcymn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qilxzeel.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pspcvlge.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lqzxzesk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ivhxybrp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dxxqiwwc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ltphfxzl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dyfnaetq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cizkvghe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jwpucpow.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nudwecjg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dtuuvqba.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdljyyz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lkbrksoo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rgldzwnl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybpkjvzp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ypfxzuoz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2uzzjwwnd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tdbuwols.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcyuhb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zvbafjdr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lslcuphi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rwwwclol.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pbepqhlj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mjuolfxd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gnxlmahf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nhvicqlx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gfponxxi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2waqukgvj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ieyhduzz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sgsqzvcj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xnkgzyxc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ssosikhu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2uzjcqtpx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qyterzcp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nmdetzgw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2elnsozrp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2quwhsnwo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bqbppvuw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qyfvyfto.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ektzrkcf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2avxcmyig.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nkhzdbjq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ogdctkny.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ngfamqng.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ylnkgebf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfydgyv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pflguvfj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zszhqkhl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2djjchafm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2acxipmpz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ovoinmpq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lhwnzugg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2uoxuzpgz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oycwlkss.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2grzilfpu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2saevmufp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aynbonmk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqxmlnq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pwnztkim.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyuvzbb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cburnysk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dladozyd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lyjvydvd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgzgmocu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zqffroub.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qkgcbfnt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zmwlqpkw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hxshsosa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ojsmnrua.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dvdmkmuc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sqnaaiec.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xveczbjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgfcijwi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kuihqdaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjddxbyt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2irjmxmih.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kmfiajip.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ondehmpo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hlgbbrqt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxciai.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hzndoeme.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mmdbgmed.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vbcpsciv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2azemvdsr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xpoxxces.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dchfzwjg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ekxfvbso.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hedrpiuc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bcefxbla.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ujuwsege.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2drlpiuau.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kyfrqxva.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kiznyyzl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bzikxrch.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ulxnptio.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rfpcbwlv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2amndolgh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nrglabxd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mchyfjpl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ffcdgujb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2txawuffu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cncyxzvg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qaekbolg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rchiolvl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eqxdgxfw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ekeifnte.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jbmhrjhl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zaqshror.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jqwfbplu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ebltdezp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2aqkrxxhz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tvvtyxpm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2emquutsw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xvholkhh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gxmzovme.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jqnyjczf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2oqnnealg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xzqyvidv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2txjgyzlj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2liiwgnar.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2riuxmgnc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zypygivx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jrvwsiyy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vbjatcad.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fsulawja.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wsbrrarw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fbceduoh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xsgxbcxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jglkrcsj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fzhughnk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dhrbgfee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjngswkb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnxnsk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dfewktdd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kmmqjcyf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2aeasbspg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mjzookah.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ntdqrjjr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lgivhblf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ehcohjcm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2eseymuql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xzakffkv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cetvokhu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2sqbrvbpw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2kmlrjjmq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ahkowfho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2erzdvgji.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wcrargch.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2yrwlmcrm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2fchgoswv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2fckfsnnx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2rzdvuhjh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yhdnzkmz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dedphpsx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oglvjnqh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ahkaejnx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zdtacden.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cujrzapy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2htlvwbmv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xqbjcnew.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pvjjvxrh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2iuotteol.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ezskfmxj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kdlxwmde.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kdrvlhqi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whxejzub.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mtjoewpe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xvmpkdfz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgnozkyn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2azqojwjm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qdegnjtm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abxmccwy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jmijoqed.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sjzjjibp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cguuvmnr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2poraagsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csualgsi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2kktffldu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfahhvzx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ilzismxw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dukyxjct.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2flfnlrjp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tsymmjyk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2licyzljt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jzbtawbe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ysskzxty.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2achdlxxj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nwsmqevf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2aysafjyd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgxdbmfd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dahoygyo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pqgqqpwc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dyofyuby.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hnogqpxv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jxqbnrks.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nzucwxgo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wumdcbsl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2dvrchdcq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2fgawybpp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2etjnkxdz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tsiaahfv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zerchofb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2glmbrsrf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2clyfpjxu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2higotjzt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkymoocs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2nclddjzd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yldkmkkp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pgubqbnj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2atznvoyh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2elqgzqlv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2rwlniopp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2uiwxtxqn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gzriuzkx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qlnuatht.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nolvtofd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ueydbitt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nfzbelnd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2atovnptf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hieolqji.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wuajlyvf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcqhsuuq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjltqdve.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gksykech.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kuznvizc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2siriafmq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2amziidme.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2axkoiure.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nwwwwpra.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nerqztoe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2wfryqehy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mlskicua.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iezrqajn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjbmhwby.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdydwli.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2syrztvcc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xeglhuqn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2bfxmiaid.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kbebovim.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxokqza.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tquohoib.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xuudxkiw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iomswicp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2drbkfgfb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lzihdhfb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bmrkmcsl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2cldynfkm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwybqh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxyckka.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2degdudgn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2acclqtct.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tkzkjncm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocjebyyl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djjdqizr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eoreyzca.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awxkqlmk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alxfsfww.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2unudrghv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2nadqvwua.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkltzwys.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hoddjudu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2uohsbisu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ehujvxcq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cfdswpfr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lyjnyfxb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2asfuvvzb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nxhwlbym.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwznvum.html


<!-- 参考信息 -->