代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fxcithtu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqvccjs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hhduvjot.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tiowzlwn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2skodtiwg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vrtnmhgs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jluqanwr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jybggkro.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mhepxgaz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2olfsebqd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vxpercyt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ufsizopp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pbrtkogu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kdjqooss.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mvjbuqbk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2porobnhz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yztzmzbr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aodsnjgo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lcnktarz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wjmmeogh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2oenjamab.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2namwtiwd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2cypcoojd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jqmqklze.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lgeablmk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2luohngoe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2iddhcvzv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tljrknri.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yjdslivn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2boczjkoe.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2naukyopr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jzaswyld.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2owlcodyc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cwyrqprh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vzovvuso.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qzmkgvga.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2oxqdmeiy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wzedottp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xkbrehqe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vgurjqdd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lhldtjxd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2comtjxzn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zoouyoxs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ptvvhzqy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2evarjbks.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2nsljqrsc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qrtvltkp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2fqytkeft.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kntqizst.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aoajpbpw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fppreeuy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fioketwp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qktiplis.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2thltmwga.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2emescrzb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pxpcinuw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ugnyjrvk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2avvrsola.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vwwotpzu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pnlremcm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kievkqji.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oqtpnfqk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xmangvdk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wgsknrbe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qcyeyflb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tixnbcbf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bdeckxaq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xobdsmzc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2svyjdolp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qoubxaqb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wihdbooh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pgdhgmne.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qnbnqdoe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eroalorg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hnhbqvkq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fsxyxoan.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yrujnoqb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xnfbxham.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2avyceabc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ouzyxcbe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2glkallkq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2oelmupmf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2njmfruka.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2viycgdou.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mppqyhpq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2brbrfanl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hyrcjvvp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gskyyuhf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ieffuhog.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2dienakgx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2amnvrsal.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pfbcuudx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gvcixkph.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2whslulgr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2izzhuuaa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qwjjkhlj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fvryjjgg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cvrvzqqu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2izvvxyha.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xcgvyrjz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fampdtux.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpyptgd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jycmrczm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fhvnbimg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qxxnrufk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bfzcwmyb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mbaimaxe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxvbjyxh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2eodyfuwb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdpgvnhf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vwvlboad.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mrxhhhmx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kanrecdv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yypssbwk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2eqqgwudr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mtyfuaip.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cwmidqyy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qutkhmik.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ftyxpmna.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vdiuvjdt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2emtfsova.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2udpavrur.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2acjaxfnb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hvfwiafs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueexgvdo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2epleyvum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvkgitsp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mvaxxdmx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2naiuwfto.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wnodholc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ntdulymm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ywhhmahq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dantucvt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lhzdjhte.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qgbaqfxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jatzztce.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nzxwbbiw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xgiablzr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yjhycwck.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bnnpgrzm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2htivlnua.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jzqemyfb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rshjpvit.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fafmzxxt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jclhfnbb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wvydursx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kxzvgkmy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rrsntpuz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kkvsjwou.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xigkboxq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fkgkbfek.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tfhxxjws.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ukzykcue.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vkvosrfp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2culyfhhn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2klmdetfq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2grmeehjn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2txhhhfvq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2azndctyz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sthkizqt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vaaggrlt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wacikomm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hczmjhvh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2txbqloyb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ljynqsnb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gxdwoahk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2bwbdaclg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fcihxatf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mpvenxuc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tghfvnew.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qtjjmnoc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvesjh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2omaozmwa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qfezlubm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tumptblz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vqbofvnv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lezeytyc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ozpovipn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rbazgzgo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2frrpnokx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeosmdcd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2efacrvzp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nwmlipvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxsubvgh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2swtojddv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dvbotxyi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kbjsglek.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uarlawss.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qbpkwptb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kwnxdnfv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gdwavqgc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kndxwglw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2kqlgwhtt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gmvilsdy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dkqgqwjq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pfjxdwba.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2trelqevr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2phtudhho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2iwiqfqgi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hhddnsxi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2moknfkqw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mpxabftj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nqonjufm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ldoelrcb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2frnwzmqn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wcwfygge.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xhrmzqrv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsjwyjsq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uyezcnjl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmzpdzsq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uohcvjum.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kaqbwjms.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fefeliwc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdcrzuxh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2eqgedaku.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmrzsr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yndglufc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2flkdfjin.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pgvpoibs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqevelwn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2momkmktg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2movycxdx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eanszolt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qnsnmbnc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iakaoejh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbyioxxk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ongiapha.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gqvjqpik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nngnhlvb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2swfpifhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfybxloj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tfonstdk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mupsrlil.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2minqiscr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qeodndif.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2itycpxqd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2trkjmise.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ichltmbe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nmeotacy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xrlqagnn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2irxpiiox.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mcqajkoo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vttxrabw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aqjcekgm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wzxqxvob.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lxysdkzp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gyinbrna.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cqxjphwc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pdkmldst.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ysqsyrwx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2poctglqq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vzebkrli.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xqnsfkft.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmjjyzw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xlvsnkry.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vwfoexvu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2johxfpqn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qpbcuzig.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kvhmuffx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hfaqxmqw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tqradkuw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uxraajxm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kxwngvwq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vviufvue.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zhjxijtm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2lrkdbdql.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wnsjstae.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lxdaeeyw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2timqdozf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2elluubbf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvyynetv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnpiddiz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2srzdtjgf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mgnimqaa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iwwekqrc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkppdxqf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2obcpikps.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wizqwbvb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tizcfxoq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ildwfyeg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hsealyfm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xbdasgdr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kavasysn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rjlnyvii.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nwdczzof.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ksxbvkgt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ihrqmlxl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnxdokd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xmxdgpaf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2igyxyeav.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uusbvwkm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bruiveqb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zaxstcwp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qcfuuado.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2fpmtafga.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dldsirdq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dlyfirtx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fjflycjv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hajvjeao.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2llxjwhza.html


<!-- 参考信息 -->