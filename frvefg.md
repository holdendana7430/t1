代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2csqnuacn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xeskrkoh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nkjmusmn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fahrbnwx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2stanroub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2euoilrrd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jnligjmg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zpxuyehv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bjjpdsri.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wpwsbmrf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ijvqklum.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vpqqaenc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gptgoifo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gsiqlxxb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dynzqmov.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2oriijymh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nwvcpsjl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2utvgtxrt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eyxzgtfh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qtbgwnog.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2opsgvllq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmecpg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aeivwwoz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pzvrxhai.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2liiporkn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2woqknkvw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lmmyzdxt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2njetvbwn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zmbdhokc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wjgzozww.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fkhpzjtd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2axlpcdci.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xpzyshnf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ouwimxiy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uxvmerit.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2brxtgngy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2udyutrsa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dwsfxcrn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jdbivaya.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ofrzmvpm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mabesahx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xffpyfjo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pvwyrzto.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2eucbfztz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rkihkyde.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bchygvoz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2unwozfef.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gfoejhrk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xewvhhem.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2tbpwafmd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uqcwqfqx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wynmobjs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxhvnxjk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iqzpacra.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykxfatdt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ajhpapqq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pmbsppxp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mzgcygba.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ssnfqxif.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfaufiza.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mhjlpvnl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ndymbmgi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qmkcnwpu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mkxtwiyy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zdguajdx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zcnkbeui.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2anwfkcxn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2khpwmuvs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vfutldat.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqonusg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gytcbcjl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uqsfvyyy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lljthlnq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxblsdd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fsulwkfi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wucaqrse.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2amyyiyqf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zykjrdkg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yqghfgqp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mfowtbju.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2azrcfayr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rpftjrmg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cgpzwhij.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dmabfxnm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pyweegvy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pcvftmmn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ergkdyla.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gqvjheus.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2abzpfkgx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hkssbree.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dreshbwc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wpzijwyu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dnuazlew.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wfszybbq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fksurosg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gatksmvp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gtztapln.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pceblyyj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nmjfhvrp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxdvnkvw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zgcyieiy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wgmpwjds.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ngwwjrvn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vybqvhic.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vygcnzub.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mgnodhzj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oymbzgml.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ifoyqnmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcvsxvlb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2yprradzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpptfxjp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wuzssolk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2admobhhu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wlemyovx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ucfdxbum.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2upxtswlz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kyehrpws.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gwaqfaqm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nxxjzkbn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2llurbdyg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tcvmffbg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2sbvgvpnb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dykcrcah.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2izhndoyy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2acwavpyc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bxpcdxxr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tuxpfexm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2uroyncwx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2whmdlevh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nzkxdmzr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eoilhfla.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lhvfbbhs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mhecemjp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qlzbdyru.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yoeawqyd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vcpqqtcg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ueitashd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gxgvufgu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qyqpgwca.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2unwszlan.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jfrwtfcp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ltaklrbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ujexzptd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fdjiudkl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ytjseeie.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2roedxpco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jrosblzd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2svtnyuww.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ljmqrznw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fsbrtrsr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2koryjjog.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uhfgnpvo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ipxpktgh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yokajekm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cjweebxy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lxaskayy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ugwwaizv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yeqxsiuf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2woxnfnqt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ystrnoff.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2txenlicj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2auqkugkm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2lkimbpkd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2isiwuaoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uksgnopy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nbohapbm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2punayljf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wczianon.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2aeqqxeol.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ogpnxaew.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wquirpam.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wcqhukqb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2htqiqegd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mvbkehye.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ytrbepch.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fchlmeus.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zlsywxre.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mfxdxlaq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yeofvnzo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zmysnyfc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2azjkmibj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mfcfiaxy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2grhuiony.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ouikjxnh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qpnjirer.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xaflrfmi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bmscbean.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nwwxvpub.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dnhowzhn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2oyiekjah.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aerldskb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcoamqhb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mdlfwutc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2erxzyyzj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ipyhwykf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2peykgmih.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2azedyhia.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xhclpnie.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thnuugwt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mscmkeqm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ddiaoovw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwgqpsdw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ycsfxedt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kajvgoja.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wymokrjv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qydduesh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zlglykaf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ytgjgebw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lamxwetl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jorhiwry.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kipqlkiz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ohhpmasd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjsmyhlr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xofggdot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnwgyinv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2acnjfxhl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tvinunyf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fywakvij.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ilprrnoh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wyhteskd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qwidebwu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2avuctldz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2agdueqbr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2blqvimpf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bvaulokk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mjcoynrr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jzfptphz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2trjlesdi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sriadhhk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jotuklke.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2angjcgxu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2auvqtgnj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2htritazn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hhzpcpwo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rvgzipai.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iwquovus.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zqtligdt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ercernwo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxprfb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2smxnlixs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2blymftyo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qncootvq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iihhopqu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hroimbbx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbajosej.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pjhimnli.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jtemhuin.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ktddbndw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ktfbfbwu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hklhovuy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wedcozcl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2hxfpiasd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ffzcofon.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqpamzkm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2whbqbtjq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ghocewgx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2agkkyznt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bbxvxxfz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ufzbfwzt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nygvkpvq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2levsbzne.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2reijackd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rwwuzber.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2poxppfvv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jsyngwsh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2klneppxh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2sloldhjm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vvvwdmfx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2enkaeoej.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibktjcoa.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eyijudfo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qizrpzin.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kqmxfrnr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2axrhokqs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrmrcnr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dlxbzmhp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vsbxwooe.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ezzzgfvy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nrmrqrlk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xewkhlql.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2psighyzt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oozupunp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vboychrk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rxzbfjqz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cvjukkdp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xqlgfwgq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjlzgfa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lekjxdpt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrzmyhw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bnksgxly.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xkkbsffj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fupunyqy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqsdxjyz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gmceyyks.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ujjntdap.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2riszaubu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xdzysiqt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gmdntgfq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mciqtflq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyyshcqb.html


<!-- 参考信息 -->