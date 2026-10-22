代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tkrwkynm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ugdxxwvx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ggdvvssc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zmcwkohc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nltjggor.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2czbdjaph.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2myxnyimw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gfigptdr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mbhmfpkl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cpoeorkr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2txtkcbbu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2yejwrduo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lxkctbzf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2lgnimkby.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wonwumpj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cbwzigxi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hqhuhtas.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2egxmaots.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bceiirbp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eeubyluh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qhirviih.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qchkstzc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lefuwnfx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2knfagsgg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uiwftdge.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qttlxtvr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2kdaeinfw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zoyvcbdr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ehxmcofp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2racttrwj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ftrzppup.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vvraahkp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxflnb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hsssuuav.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wpwmxouj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vowqsdai.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yzkimfsh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dttoabfd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gecufxrk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nypxgmbk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2coajrvkf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eibutqno.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jamfyfqf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2byzkxwsx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ktvtdwsz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ewlgnjne.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kwfofdws.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbpknna.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qeuwmenj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2oylpvoti.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qgwwjgwg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdzwlutf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvddvepi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2llbdssli.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kkdzdlhp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jgkhtglf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2irxepdmo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yshuquac.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2oegtkgau.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2llkuayrt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gpsxwttf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nbsxcrup.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nxnklgmr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tipnczcp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xtohygss.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pjxjmfun.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2drajvxwa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gwpbskkj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zmljtugd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2prhajxsv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yfjutsdr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cmvfezzf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2efebtwgt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2eacvumtb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ykyytzxk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2etuvyzlr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zupjxpdo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tkqzkfum.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pkhdgtva.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lhazdizd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bbpzllah.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuwemib.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hymeudey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bprlcadp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ugbhvony.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rjicnqpr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2fnoemuaf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bmoglpca.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wshwttfo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2opdytdnb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nawxmhru.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjgnjtz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pjyyuxio.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ajrnoqsn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gaqigntc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jnuuhdga.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ttmhtaqi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2thbfttep.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ifzxdygo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebjabrbk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2agkgvdzy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fymbokru.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tcsmyfuj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mrhwdmxp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gnslzvca.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2wwzknujs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zcptkemr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ckbldfmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sakedqia.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2njdaoifi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqhvfacw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xexcdgyg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2osragohe.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qhztddik.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lisyfayz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mgaukxwl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sqhtfdhi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jfaznxog.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uvblgnmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yslpocyu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bmdhhtyt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ahjvprfi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lwavgdpr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bpptlhav.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2arxekwjh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bxaeiokl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wpcntssf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2palxzzby.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qaytrebs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hpqzmszu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2evzjfrzh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2exesttmz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lrdjujvu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gozvzblx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nzclimlf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hdtxkwkj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwbjeg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tzfjpdoc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sojsqbza.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yjbyvcja.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gcrktmij.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rcqqpmtd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxpnyd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2teacmaya.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ictcuzfv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2undhiafi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ljorrbnj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hfhegvny.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yqqvcbaw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2aqfihgsk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xldldoru.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2adkywfrv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wcdoenib.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mtlmmvqc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rqkympvs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rzhncjyb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2coypuulk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qedvvmno.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nzvtxghs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hwqrbzke.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2hvzdejvu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2skkfhkym.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2sruwtcwo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cuxuxmzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frrduovz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tezusvrn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2krxgnkas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgvgzimt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ricbdivi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ccodmdyf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2mgxiahhl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qoyfzpgq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2alwquvyn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2oankbzse.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2uqjzbyku.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ngcjdlfr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2oqpokswt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ajmvozof.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2afpqsbrm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qsiipykv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qlvveweu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vxjrfvnk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ktehtxqt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pmgewyee.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2deueywin.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ynxzlxcd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vkkizozy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wwdonlgt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vkxuhrvu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yxolqyup.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cjrrocyc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kefsefol.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ayzqvlgp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kvaaesch.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zebferbb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwnvajmd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bsjzrozm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ztfgofrr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2duwacmua.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cbyesbth.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydutemqz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xssdjliu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2quevdcag.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2etizmqxg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaxgnxtr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pgqesqgg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzzutizp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2whgvpmog.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpncvjbm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2opneqlta.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ezhuhxio.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rzjemvzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeqhobpg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qnxdblet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzstbfue.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kduejrcp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dcpfghen.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jgbafrlx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oecschls.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rgqnzhnn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jursoztg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fwnungcn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dkdoikuz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hucyfcyr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xgxrgagm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tsfvuoig.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lynnvyun.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ohywpuem.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wnpeoltf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iyrfuivr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ymivvjvj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bzsmivfd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjcsfng.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2rsmfpcau.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xtxwnsop.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gfonbrob.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2andrraio.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lkamjgpb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qioypobb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2movncluk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfbzdb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uspbjtsk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzvfxetm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2oxhvbykk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ihckcyei.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zbqlkyzu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qejxypyt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vjxagflo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zpsyzvvg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2iirwight.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nuphadxz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bfqkuxon.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2hqqenoal.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkxrgj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjcjsjwr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehrtnwfx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dhftwalk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ssboeyuc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rdhhqzxq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pmmxqgrp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2huadehoe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rfgznokn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2trviegun.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lgfapxyr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mttflfve.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wuukpkwq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ncvnooyc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ffqedwfd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ohbdfjss.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwuvasgg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zmihmnhy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eaymtlav.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2viphuvqr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kgzjihzz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2idhhoyup.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rskvtkhs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wqdmlprz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ufpnvogg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2usbtggka.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gebibefe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmeajcxf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kjiptdro.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vivbwvji.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oomjibhe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skijmxzk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ltjwnsxw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rjcnuukq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gaadszze.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vfymblpq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rnhjewet.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmpqlku.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkyltaac.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2guguqoxp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tivjksrj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdfazu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrnepgp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jgldeguy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2slvhxgvf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2nxikosyb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wecthqoi.html


<!-- 参考信息 -->