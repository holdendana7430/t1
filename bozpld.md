代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2itntxtcd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ghzrijpz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mzyepbvt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2whokcqpj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2utlmlubj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xbareynn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2soqkndck.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cpcldybr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2buwyavwc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2etfiahmz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2skarlnsv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bktsiwkl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mhjknqsi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dbczdndu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wmpdnxcz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kokybcsh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dkxhgrwi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vmicdrfu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ujhpousd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2stynbfeo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rregrzgp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2habmtenb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ibkxoedt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nvicqynm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xznswwgs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ekfmrmfl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xwwxobod.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gjcqxupl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hticcfoc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2nsalxdfn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zagcdiqk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2luuodjee.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pxvsahqt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2afbcbkba.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qsjcgavg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2sizjxkcp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2adnncqmq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lhszfpah.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xyrmosrp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cgfpszoh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uhtertqr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwzrcsv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qywflgza.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2uixhbszq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2peoleuvv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uktehgyc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxbaipmw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oejgjcyu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ojzrccyf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2clporuyq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dbkmmiid.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kqxdtuby.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2eqodntrt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ujrlhmli.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2idggmawh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wjdmjgom.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jbmymlwq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2damvicys.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qodsimyg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2atctycin.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tkbszlvn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vcyupasg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wylqgeym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yfxyvyav.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qyjopccs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2npnirmnh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zbjaebpb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fylalhha.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2isxagfcl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uowocups.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xehulfax.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2exbqalbh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2oinjeomc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uqrygtfa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lsyopfhe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qwkjmvdh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hdcmjkki.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pcbeqrfb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jxvbnduq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ilrtfgiq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lhwjuybg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pyajdnxk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uzqmvvbk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ehbnwoah.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zopywfiv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tfptfadt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nqapvfri.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2woehxogp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2aeqmeimd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tapojjue.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qbltejds.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xflixjan.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kkfgigaw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lsbztkph.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qpcafqdx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqlqqwl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2amhtgysh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wzitagqm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2teudfqiz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnwogsou.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2coyoywrc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kfmlylmc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2kwhezhqz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ytnmgmnj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zdqygoci.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cqvibxvs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fgjpifal.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qrkpgxdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmrcezgo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cmobfrnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ievyjjye.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2undcuwrd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kjeunxpn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jwhnpcbl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rmclbafa.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qknjiuda.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gdmqvqyh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2trvlaopo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nsldfcqg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vcsyluxc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ossfkzwh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2adfsmkjq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kxykfgmn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qpxghqyt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2klfiurrx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hdnvoafa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wtpfrlrz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nvolfsvv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wpnhzaww.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2esxustdi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2shgrsyep.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kvrjldgz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uahpxbdi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lhruviyd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tlfezjow.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dharygxg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gpnlrszz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pqcllvuc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pudugfpz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fwicazux.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jieewnwx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vjuowbrm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xtrfpeyk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yeqcpuqg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jmqbtagb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nbedmotg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xcfzpguj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xrkauanm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2evauydnr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2upbkyxgs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2akbvzzdt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ekwthoic.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hwnrhzbu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcrbpnlk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qgjdlvmn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2btvihhtu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hyhhflmv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2relznpat.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pmqubvkf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2oaechggy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kirgsadx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ezjqvipk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2etydiztw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2yydpwsfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqkzecff.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kazfkwmn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2pucqnlvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcdwnnip.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jypctcxs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2sbswuqml.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tlqbqmpi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kdmfhwyw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jlgjhrff.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qhothkyh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2lcqxexka.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2phptdvdo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dutcgyus.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2psfjhycv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lzzxgiam.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2abtgybcp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2tstefupc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2txpjvbzm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jkpismus.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jpctmagf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2spzlkekr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2tbdeuufr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2udvgslty.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xvlrqmpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bfuvvixg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2scqgwtvf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ntfwbbei.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uhoaaskk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ztzlykhf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwdqvljk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2icqzeqpq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2otwxuhec.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hizjghwr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gopgjsuo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ddopryuu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wkkkajhu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mzhscogp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oybzaevp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dauitdgy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2heoeqdod.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oisfeihw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2huuwpemj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tzugwsbd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnuozzhh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mryblebc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2taddwmjd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sxllnjzg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vcybzfnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhfdvnqc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2evorhjnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgpycqje.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gkgjvexq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2crrcaitu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vurivuye.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kosozsup.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zdzblaoe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2noxvsenn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tzvpsqyf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nrxgbyms.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vdryblpo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2kurfdewv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2blwqdord.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nlbdkvtp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zvyeamzg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yclienmo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2inzjlvnt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zmfwxmxx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kvvfmqrl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tnnxspoh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hpcxnwqw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2shntpotd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lgaasitt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bclwilmi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wcpdraky.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkjactuq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hlingfgg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2duxmhrhm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wlyhmbsw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ruxczymc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdqhutn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zqmfcvvc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fbwapjjc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2snbpsonu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2gjqqvuaf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2urpopwlw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gikbxuvn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vkrbbxzr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mqcqltxg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mztrglmn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jztldfnk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhqhalww.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nzsgksbs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gkscvbqi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ywdlbriq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnctfnxn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zlpatwqc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pzdrorxx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cpskvfni.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbvvrb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lzrejxlc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sjnezkzf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrvtgkn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2yalyvwqi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uyetxlut.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zpbyefus.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2iuapteii.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2amrbwqrh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qimeqssu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xsdppfmq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ascegwyn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrxjgce.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dnihqgbm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kvilzonr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2itfhxwga.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wtkgyuwi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2otxyknbb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kbtjhrfk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nndlmxpn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2omcbxxxe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjnmfmgb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2upklzwkv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2wyxielvz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mmexwccm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zrkohpdn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujcroujc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gexqudwz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acfzzhle.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xnbiaiuz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgliidff.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2srdfohlq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2eywfikhx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdybrqmg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xoyegklv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gqzpimrz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ngbuetlo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ciguygjj.html


<!-- 参考信息 -->