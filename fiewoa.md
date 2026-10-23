代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bievoexi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3psybiwxa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ditnyysi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ewzqhpxe.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xxrfevmc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vobgqdxs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zjhtxwkg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcgxhut.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3arpivehf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dnxywlrh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3grqwestq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lqjgnlyz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ahsotlem.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pxfuuoxi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dldqrbfg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wxxkbsdu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gdjtuiar.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nmsbjstu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fwtghokg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pnozsdyy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kpilockz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3prlsvybx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ldxzevfj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ylgbugwh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wwlmcfzl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3isymxwle.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vdynnkpe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mggghwnv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wgivifwc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vrkidsma.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bfvadonz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xpuipjqf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3agdstgmb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3utalnpqx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xuuhixfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fqpashun.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zrpnlnih.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gngkqers.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hahzwaks.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qedlauqz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hddcurvg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cqcwpqdj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3apwyjnzm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hbmzqmsr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hpqqxcsu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mzovvzef.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ravvwabf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rirafpli.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ostihipb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jbloebrk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tpxohyii.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uqochfhf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xpvultzt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qnlvwktf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fmnkvsdm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mivhslbr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nhqdyvnh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3setbzpmv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qnkxpnxu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ibpjiogt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhudevav.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3slsidsqt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3awkxjhkg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pjdbflzg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tunlgler.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3alywjxms.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jyexnvpu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynibxmeh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yexvjcck.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qjyemfad.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ujacwrfe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zjbiriyg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bzsbmjho.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3atgzjfxv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ahblxqqx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tzhruhiz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lfyrgupo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aeipclso.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ekeilytq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3itvxqapp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ludwiqwp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3oulpbpbp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ysxnqyzk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3szuuztxm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mgomuuvu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cnvghyii.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3grtyfjtf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gdxgfnde.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3okuzatgt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3swfnfzxy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pnpnnkyj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lsmsfirq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hnqknumf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3polkrsoa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vgwsapkp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aaesbycm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3suucxbjz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3aqarsetk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mnfrtlpb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pbridmmr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3umhquxrk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtizbprd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ccvporwa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yoptjezk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kwfajacc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iejjyzjs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ivpdbany.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3smjhcapy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cszobziq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kysustmn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gjzyqexm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lubsokfa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gzouokwl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ndmgsysx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ocaqoxhm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mshwaebh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqzwhbzb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3szvxcsns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsqigoif.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qyqgjnpi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ronedzcj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zjmkefna.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ddqxvuvt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xmpsmxyy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pvtezchl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hllzmxyf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlhxij.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kjfmqoov.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ikuojfhm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uhnofioq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3djqmguxa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3paxywbyd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fswmbszw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jzdcpnel.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rgriabat.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3arsdqtil.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kxqiizjc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3btwdcjih.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aeiftimu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ysqhxpzh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zveviden.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mxfkjqih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3abzpogxi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kjfynrpq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zxsyyrox.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3krebrvhj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zocyylma.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wmuyzscm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wtgcikyf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hameiouq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nypnuomg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zmdtpogm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hovyjxqf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lroyqitf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yukrfprp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3udtqnuzx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3foclhxfb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pchvfyjn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dmtaxnoh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qkvbivfd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mpmqbich.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3waskhyym.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rhuxcfbm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jeebwwpp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cixrflaz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oldhgzpj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nbofmcea.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rrgldpdj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3azybdggu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3exdlixnd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fzwulyny.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ozjbkhet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssbjosml.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3iorfqbnf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ovihdqml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wreapejl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bgxpfmyi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qjbodnod.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3atigcnyw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gapkviak.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mogupatk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vitrfgpm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hmccaboh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3smeijmqv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3bfpvelkl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ysvkndlu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nakozqbi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3bgjcrnpe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3djgmfwxq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3srrntjnw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bfjnsovx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dolhvdbp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3eungarrn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3voxdywmd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ebpgbbub.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fsnslivl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zdmeztsa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wprecjyc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3esrwwckd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3povcbhdn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3piuxfmdp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ubdogxsp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kzfxrota.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3nyfcuuwi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dhhfwnly.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezmhemal.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hltggycq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bbjzezrh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frrhfnzt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vrubeesv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pycavryd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abhgxkwy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfvorvte.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njfxtmyb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yglkkhbf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtqausiq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uncplclz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmbxhnrq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dikilflh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nxtalmwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btlkapsa.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zmhkogcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvhbdivb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zfujuime.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wdjjpaqb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ybgoukwo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yjmrigcd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pxpnigzp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3usmgtmwz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cmhtkmyk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ucgzhxwt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qrlqpvjh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3buqncdkn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3thaxhaoo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sgjjzcpu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hnpjatsg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ghqdhept.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pxntsekg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hdtxfuxi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jjeweggg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ryraogbh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nswbomuo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vkelbuqf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fcquaoow.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jqefxqma.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rxeztuvl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cyaguytj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3imnmuvca.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mmnvvogy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3weaeqekd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rbvryjqi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3brtfbzav.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcgtybxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sdkkexsc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rzxisksr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qhlgfvbh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3puobggch.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3pdzizlto.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3enlmmqil.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3yabkkuuw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3lkicrizo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pqzlotqu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqzuaqby.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yugttiuq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wvibdnwg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jnslbchd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkalswly.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmfavgyh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vffnkeqs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3whmmlygl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3igbwngyz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3veeukyrs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qaegoffj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qrrgiqdz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gnqokbzu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vlllzuxs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rwnmlkxw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajyqmnho.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qadfeqjh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3konmhbjn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3pekeitvz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fcoqknrv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jqobpnhl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3bfdwwtsl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcdhgr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3msqrfwle.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rlbbuzwi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3usrjgipc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gxdrzhsy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3emiodmgi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3afiittct.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rkcbanac.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wemdjabg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vlkrffdw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vcojqbau.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kykaqvnm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ylmtfkxy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmozzks.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwueotp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kickzbws.html


<!-- 参考信息 -->