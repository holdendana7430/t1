代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3adhgvnmv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wyzcxubq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jsntxpps.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lqomvowt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vutzhbla.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gqzineln.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3izhircay.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyixmlfa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3pmidjwqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rrgspyzw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xduhsazq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3sbqtlqqw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hvdraoxc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hwizlhvh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wbnbgmgu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uwcgjegs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pucgtust.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rjeahzal.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kwredclc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fjmsfqng.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pnncooqv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3frhznuif.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oqgqqcja.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gvidafrc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wiyzqxau.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ixbqajxj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vklssmvr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pvmtrmnx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hpndvhnk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3elsdvbvr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nkqcxokr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uwnegmkw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mhjygbmh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3efmmjsjp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vibwxmsc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3iayxmsrl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vbwzqxoa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uaqbumwl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pibnjqud.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wsmkxofr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bvwxvuzy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bvwhsqkb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qmmrpsax.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kvodihxt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3muvvbglm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fjandxlu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cbwnjfvk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3azawwkim.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3suqdhzas.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vsehxywy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zuzuykrc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tusamzwl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zcvcbsfd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wgczksoy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jtdqvqpb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3acevxefg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3okjtswkx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3whlqdsgf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3uxpfsizg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3duibrxpw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkvsru.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fpezsaku.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3feoxxtvl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gxgtbcoj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vdqwalxf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xdthrzlf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jilccypc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhmudqf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mjgdjulp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yegiscyg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zbnnmepc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ayyorilc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vhgkdycb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3olbzfhha.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gevodmtr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kdeejqqo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahctcpcj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3toguunnz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xhwlqdct.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ivlvishd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pngtqsdx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3theopvrd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cxxwcvgb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rzuebhtt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lepqjekf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3abwtcwlw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jzlhkshf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ryfnoici.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nqgdmbzq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fvjdboeo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cxxruxlo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3syvscafd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3btjongjz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3akgmrlzb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3cvpeavqy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ghseqzab.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rrjrlxzb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uhwlskvs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3derfxjmh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ehnaeqip.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bgecdebd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjzxzxkc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tqmjvoyv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhwqrmy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jtmphsiq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mkxfnzcf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kwescgtq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3komeayhs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pwhgrhzn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ijpycpzu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3fvqbcusn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3grhhnzde.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uhasgmqh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3sjevxdjd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ybelzvuy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dorvzzrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odbmmeuu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jkebhoyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrxsoasc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hqwgpypo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mrchjfzn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3itwpwpgz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dhqtoukp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ymttkaaw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3etoxcrce.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3olnupexy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fpiwxouf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hawqcnmt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jaegwbff.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ctdzczyt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3aortzxzr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kaiomfaw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mfnunhnz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3micbbtaw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fljwjpaa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fjzldmzl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qwkhusid.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3naltlrvs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vmjreusw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3sdhbincd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ggdklpbz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uznbtmhp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jfewsata.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yamizorl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ojbygdlc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hyokqgig.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rsviadjf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sxmzqkmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tbqsdpkv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zidzncpi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjtdwc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tzmblmsq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lkivcsfn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3myylqciv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3trpltqqr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jtoywmtd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3shxwiqbb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jxrgsvwd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3osxwfkns.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3sxtgbabo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kphqggke.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3thtdsoqp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kagrfist.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ktnxnfgb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pjtbchmc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3makyhzqz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ahfidtzp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lenuiegz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rypteieh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xivphbia.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3djumsrpn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3gujxqbrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujyzqzqs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iqwbzcmg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3refypyms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gizsmvvc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qxwktzgt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3iwqemhww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3egxcdikr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lmopfvix.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xigrsgur.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3imsiskyv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lfjybagm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kofzvbzz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pzlioufs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3exdgikwf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3egfmlhwy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ypebjpnu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3yexlmcmh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3zvjxymmd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3kkykffqw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rbavqgld.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lmntvzkg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wnmotkxy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rdamaypw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yhofsvjp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ljtahmad.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lglintjw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vyvitprt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bfdynsiu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuwpwdwh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omohlqaz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mwgpxnyi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gofryuym.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asxcsint.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gztddsxv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dvflrkaf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oamyqlnb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxbgyldy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vnsmwgjr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xvdhapso.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jspqmaui.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kigqafpw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luowckws.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lbwvdgpy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3okyyyahd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yufefziz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcmwejny.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dzyrjkeo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3polwwoxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uesovckq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqfbwovj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbrlcjuz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hfptudqb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nqhqhwrc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zhgfhmtw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ramcioat.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3spkzmstd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3elejecoq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tdpaowsu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gknzitik.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nukbghrp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wqyikkef.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rcjbebvf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3swzadawa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3naoyfivn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zhwodscr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aslvtrqy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ahnipwep.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bnjkobma.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xasjqnew.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlllcobr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3gnktdsxq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jticaqrz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwqunllu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zengmkki.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nverfklf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cxwjvygm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ziskebmp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzwpmcs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bcxvdqsv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3npmibool.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3pbygjltl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bqlrholt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3okvhraht.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3osroudpk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xleavpev.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3exxrckla.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3oznsbpgg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3dlaskncu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3udqkeizd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgsxafdp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pmfbhhya.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bkngvoqc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rlqfobmz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lretmvwl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ltimehlk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmcrclsf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yyjvgawp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nfgegnrj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jikhgpso.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3twekbndf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ypmpfbej.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rihhsdkd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3hyddorld.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fmkghhku.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dajnpajc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ganskkac.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxjgivq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lmszcsxg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ywwgakxi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kvmvqsdz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmkhppm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3bxriyqvi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qgahsfvl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cdaacttn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3sipuahvt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qamtljoz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3bqgotrac.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3szkhjend.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oylqcimx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgwghjc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bmhukjcl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jydsqxmo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rjzcqksz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3epbervcb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfofysds.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzfjrvo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bohabivn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olkbfvvq.html


<!-- 参考信息 -->