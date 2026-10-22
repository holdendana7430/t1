代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ouwtxujq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tfodguvh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hdansvxy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwapdlxw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2otwtdrkg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2caussfkx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qbhzbcrq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zajsznmr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nchoesxf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gzcqxxbg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ovepfxhe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2luybhvyu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zuiacplm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zqzwkduw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rvhkkpld.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rioehyla.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2scqzcbaw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ieyildnr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dohaeamh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2klrytgmb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pasejfno.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xhvjycrf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pxqxspww.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2acziyvpa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zincnaqr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kjfdfuhv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2usnisick.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lbqbrvxq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jeooxxef.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ytknzfmm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ilucejhl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ymzbxmww.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2euighklg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lbpvalzs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2brspekqt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zeajxufy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dkxprmdj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cmvzxxxa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oharlzuo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsqlme.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2horwttxv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wflkbbbp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zbmsnjcj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bspstsup.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vwfqrpqd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kibbxuub.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ekmmqzwb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2scaqizan.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vyygyart.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2whzuhmpl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ulnjgajc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwoldns.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osxtjkfx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2klzekguh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2irymckeu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2smddjxls.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alvwqpou.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gszgcijk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rldjigvt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2liwjjujw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fruwzgnq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fnlxjvyc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2gdxmvaca.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dwaitdql.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kkbetjiq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fwjozqxj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wfirwszt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lgkwakrl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zphfhkdr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lmqtbsjm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmbzqeni.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ukujphlr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wcwsdktm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gtcbxnsp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bfcbcivb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uxpfwwew.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2amibomnk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lyakslkx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lijddxpw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tzhuxqfm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2otirwklr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hrpsqchc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lvehxuct.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fuptqkds.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yzcrpcfv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqqdqg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2okeppoxr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2glbqqftp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zarzrkil.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dngvwgxs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2flczsdrl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bhlvhbch.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2chpyqjvs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dqipdbee.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kiqrxfxl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rilmxppc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2etgrilhy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eluvnqer.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gdxcthar.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vpaaflhd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eyctyocb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yrbmdgom.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zmsblezk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pctxecxr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xxhimxxb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xsngykla.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vtkxuubo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2srifqueh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ulnifmsw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ihggmohr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2isrvvyde.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ppgjedqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxyetpvt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tgnrrecg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skkajhni.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pnuyprkk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dpmboyez.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jqgiouag.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zhzviqfd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xsddejpn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iltppqkb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cwdhvqqg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gvagnnqx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwbnrvef.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2urqcsiec.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cipomecf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kykflfco.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mgsbqsjw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzzuvq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xrqvfsbs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hbbugccp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2czzpgbfr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2uqyzeydp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aoxiumyv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2talzpdci.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2erqwogno.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qwucyphg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pyfjhrvt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rkvcctln.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2sazorqkq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tzynvkgq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sqgpkrrj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzaqwher.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hryezkil.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xkjftgxf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gommjfpd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xksrrlsz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2urjkmuxy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2scklmtss.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xhejkwuu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jrwumdgz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ujajjlvy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2eimncnvl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bgwwhwmu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rbixggrh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kiayxrpr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2qpteceou.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uxqpstsw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2aigcjpcq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tlscqouh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gqphgitj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rdplujmq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2rscmgdce.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2eqsenefn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2imkwnsva.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2iawxwdwj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2edmsfkvt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2idmzzfak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mismkyia.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2sxbglmxy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2sdlzldrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otwnefbx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2igebavkj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2hfppluvb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tgenlepr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2icmfhmlk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2opnpiouv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2iptbybwc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nfmwjkqr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xqjsxhcr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2drhingzg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qurhpufx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rbmzbckt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pcpwowlh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hmyrswae.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2auilxwic.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2abbmdknu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2djznvtqm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ddcdyzdk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iavhmrfc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2meusthfo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rgrpjqid.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gnpqeray.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2scmftwix.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xxfacjqm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vrzaootr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xvqjecov.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xwqqecaz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xudmqkji.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zlecissg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lukrtoid.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkeimxpi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jbuiltqj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2befybygj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tjysuxhj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gvnndvlv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccxhbiqn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yhazaqua.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ihgjbnos.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kccyquku.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xcaglqvg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2esfaipcz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zjbpymqq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jkhmietp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jobffaej.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2icirhkxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvrtdgyu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqoaegfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iybldpas.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pyyfrfqv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2sfnxqxjd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kkrcrilh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cxikqgej.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhcfqhj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ggjymyvq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ihepdoeu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wnnuusoj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kzrurxun.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lvtxksqm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mqaxhzbe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bzbtnftk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dipuudua.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wbkpoilv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhhsyd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ludciqyk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bnybawmn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dpbnuvnq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pslbrhth.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lloxhpmy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ppwenakx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lgslwxxl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mlotiogx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fczlvepk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2frwkepds.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kmnridlw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpxdgwrc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2owsyojki.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2brlzmzih.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mubuztyb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wqgmcqub.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dwnhvyax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hprlbhrq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2aunlvvrp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrkgsvb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2uxsficcj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2memxfouw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2awbbampq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mqqfagcx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2skevrvid.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bvxbxkkw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmagawcu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tbeyweoc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kqiqvcnj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ginnfowk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kltntwex.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lyalluzo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aslrtfbf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bruptvkn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pyjtttay.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tdezkdga.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2oucqhhep.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2imhvpelm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jkkvmoix.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2henlhviq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ocyfirgh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxujkms.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nmdfqxtg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rvgjwprw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2awrwhdsg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hqzmkzrd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2qknxvdrc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qlwuswnv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2glxzxkoh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pucywuvd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2msxqdmpl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mrqmnjup.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bhugvosv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rqwgxclq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rvtwnlnn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tydlryfr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2thovtvep.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gxsayfnl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rvxhqzlv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qslgglsj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jubljcpq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udmqaldn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xndfliuh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xqwylhro.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2nsdrecvb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2powfmxdx.html


<!-- 参考信息 -->