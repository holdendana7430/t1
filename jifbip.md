代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2krrxmbfv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2frflxaas.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jvhhztyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwendia.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2thfunzry.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zolexuse.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2elnyzsdu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qwhccngf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ippoyuxh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bprmmguc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2sdqhzglv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tahdtasd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iqwylaby.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cxenwhyu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2alleqiha.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kdixumou.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bltbkymi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kexodepj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jiawuoms.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dfgnsqxe.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2oysaayzy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jsrnxyir.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2inahucfa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wokobgdx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2djnyowjq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2tufsjkyh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lfatkiwq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bhrlknge.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lynyxons.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wcbczeqh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zigwwpwj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zvumrsfq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2esbnnupu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zscmlhlq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2eepzshyq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gidsemhb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2djwrwqlx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vqcejbzf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cgjlryae.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mlltohox.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yijaxcpd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dqjsqpxt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fkzsbjoi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dplicntl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2amgakgjh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qqpiscqf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qtqdsgxp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2juqjgoly.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzyjbc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dfacqbbx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cslmgiqm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ultkspzl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qlbndnke.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2btvzxcok.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gvzszhvh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvufxkwn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnulbmtl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zotrpxlr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxouqfqa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bhhclryz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xicxoupo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ktmniagq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ztjvpgzc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vabccqxp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2euwnoaln.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bvjhxljc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2stijqtug.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bgrovfvh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cgynkkcn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tioozzit.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xysrtcnj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fcgjtmfq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qrfclzda.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2yxfgohut.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hafuoomy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tbicnqmk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xmaravlv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2duacvkqq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fipiqhat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zzdhpfkb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wqgrmrpb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2czyqjgrk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wreaossl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gqontzxp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jaqjrvdi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qnuyfbav.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2btveaknd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wcjosvoo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vcedyqkk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rcsdlqta.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dlqvwouq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qqlfrypr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kwgupegz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xgujzjeo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2afhqqqzt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ysirokxa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ubywhhdb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jkufaexh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2muljzzfw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nybvvwvs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2athgqudk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rjdeuaib.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2chnbypri.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuxfthuu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sonjgowm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rkcwnleu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cemblzrv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wtgikkmf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2adbclkrw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2soszdmmr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2uctetnfx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2jarortcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xejcqoab.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2laxousmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkduecfl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wexscnci.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xmfikeep.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2luyvguhi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ttqnbdin.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2euhzroes.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hfcsrosd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ubujbdws.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cavyellt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ydwoaazv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ihszighj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tdkdcgqs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2sfpqshak.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zcqubvxt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2znkhryit.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jrftfupl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xjxgklww.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uniimyki.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gplombrv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ftzgbqit.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ebqwxhrb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qrhgwsbt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tckxoypn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ujgsvqhn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pelmaliu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cpkmkzgr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ccxkcvcv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wsgybaql.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hxkkhctz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rxgoeavi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xhufzrph.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mbfxcxts.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jtjijuur.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2isearyfa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qmxxactz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fvqxisuq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nypcahbr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hhesknrp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vkrokupr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tbglgcok.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ugughhvh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2avbfkgvy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ubzqintn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tfuvbusx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ccxfktxf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zjasonom.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wpevcqjr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lipiwqtq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dremrghd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nepnbebk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ryoglzcc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bymvvuxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dstzvmuw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2enxbueac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lujtxgvn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uxlimxvc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2duqevrnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecyiqlct.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fmtjmvfg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2mntxccmk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yhfypanx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2iuacxnlo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vhdworzg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2uzxzyped.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gxdvnlgi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxlvfu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zeuxzdej.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kbtpvrno.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wmhfmmtu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dbruwhnn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jkfybiyl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2qvphucbe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2txjlqwgz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hwejltpf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2aiiiwijy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2eaudxbqh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2gclotbar.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2uiitqdjo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2shmfdaay.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rjcntkxc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uuuwflne.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xtefongz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdzvunmd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxoccxbu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzktacwh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmevizmp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzmqjnob.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqdxpmlu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ntqmtcgy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sipmmzjp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulfvduih.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlfnzqmi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kweafdrn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nwwunvry.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oksbifpf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pjonvzwn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2neqrlvwk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2imlsbash.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yspgdirw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zzegjvwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xslbhcyz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ydegmhha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqkjlarz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wnoadibk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwtnywtn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ximrjgvs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gokrcpil.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wzafyqpj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ypurwzsb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jdjnzphf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2guljtxxh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pbczupxo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zhfdlued.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lsohfiwy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bqibzygb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jccrbdvh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rlbfoine.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qdyntrlm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aawqydur.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xgifxufp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xbktcyfn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bcjhxnty.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2omgbdhjs.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2wrkzonnv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tdrknyjo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cihalsbt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdsooofo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2orgkmwal.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vjuirjqp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yldjrisq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rveqhgsv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nyupvqmd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qjpdikef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mfvzjjbw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vamaezdm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zbldupum.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mylsihvg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2azsggsfw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2bewpnnnl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ugdjnsvr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2gehmrdsa.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2rxjwydzn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2chtnyvkd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cclmgzig.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgrgtdrd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2swqybnng.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wkuqworq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvrlguko.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ckyooeaf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pumdfkzh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mugfxmhm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sdaoqewv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ghxzqkoi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zwnqiapy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2edctjhnl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nfnwchyj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ezmjefwi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rcghyzci.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2psldisfu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lecmsxsw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oioikcqa.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2muhpdrjt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2otaclkuq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aujhfkgn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2sfojumfr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rmzqullm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kiqkgjqq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mctvhawt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bumoyszh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2etgvwzdz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmciodv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2inpowdhz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcdarqu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vhweuima.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hvshmxpn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2siowylqa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2daovulyv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xyjbvyjz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqbztggw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sobngvac.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qhbefegk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uoclidzp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rfoielsg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xrymibni.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zvcbydfk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clcsdhpd.html


<!-- 参考信息 -->