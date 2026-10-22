代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zdkmskov.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2laiauqrr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgcrvrmc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2frutrghl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2efgklenk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2higykjuv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2idurwxdv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tgwzztdm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ndquyzoq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ytvqngal.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2majxdnxq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2klvayboe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iraojxxa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hancelxi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qwbojdqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2oimtrisj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bbhtwvuc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uijnzueo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jrecwkrb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fjfxquxa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vzgnatno.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zissfltk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrfqgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2uwsvidaw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dhpkixkb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iznswizm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yjzokjwx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qjvgnnus.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2inszthzt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbdytwne.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2orlmwdlt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2invlegib.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2niinymor.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zoxnuckv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pgffusaa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nswikovu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mhdczgdo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzgxqhbp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2njrqjejk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qhlkymip.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pnedlvjt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nwuxvsak.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qjskbsnc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pomkjoch.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2obpkcmrl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2lqibfhjq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lpziujnx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2cvjmgpec.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dzzgwbsz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ymaesqxx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rluwueug.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kxargmbz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2crrtszrr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uaglfghx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qqnqhqsb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hvyehulj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2avgivmnr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qedemtpr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qndzbejq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qjcxjept.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bqbuvrez.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2othvqkjm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rrsrvhun.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xsiieebw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ezninzgv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lsrtvbkp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dyotbttf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2atovsbxl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2njxxovly.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wxemtivd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vuizvazt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2aqjedcjt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mqnseviz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2belkyojh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eokjnghg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2romsjwgn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wmcgnrsk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lagprxnm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2huionyph.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgobhrrx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2prkcmxcj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bmnjxlxi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oixzllms.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scxholyc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2npsjstnr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lzzafzfd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2auhropah.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sjqdtoyq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jajpzsdy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fnphewfd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vdgoatbp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hssqhwnj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2naznsbor.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qpamaojf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fkjvbqrb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gbjcvvja.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fvipxkrn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fumpuodk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2haccvhvt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xqhjupyj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qapsefyu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qtrexzvt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2iyotssyn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mszyairc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jzawossn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2crkcqbqe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oqabinsn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pucmdzhg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ozkckuwk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lsiupnfy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lggqxgmo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ezmpcinm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ydakwwll.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2neksxnvo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ezensywi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lhekvzfa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tmlknfdg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2carmcrvj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uantokfr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dqgcbccf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ymkagzqr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ywriamgu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2goumsfhp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tazvkfjz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wiopoaqx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dbljtrcg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hcvqzzuu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhnisrb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yugdyajm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dshljtjt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2prtxocxl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjmfzuzp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dbehgset.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ybmrqvhr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2baepcajn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2isbdyqrw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tfhpezhx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2iczpebmv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pjgqxazq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wishzcmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2patkyxvb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fhavldrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdzficgr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jmkzbgpk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2izrtraob.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kvuvlxns.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nyhyolii.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gbspydas.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rthmxryq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mdffjmpi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xuahcsee.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2drnwcqqn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2efiknlor.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dsrtvsfc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ahnbavnu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xjlwgvda.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tcwyobut.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lqljxsrc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2uclwxnho.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wogjcshn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dgjtfjcz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eriagvzn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fnmgfjpk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kxlpejij.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cjmvjiev.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sphqvwmp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tkogmrfb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bnjklieb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lvcmlpdc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rxuftoem.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bjnqcuba.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lhbateaz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oxwmwixs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2eiyurtjt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pdrfqtum.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nevpmwgs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yfmydhkn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2srcttapi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pvkzqhio.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nwggqmei.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lohqfcqh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zhxrdtda.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cwhyppoi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fwvavzxn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sjgkmsxi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tzfafivh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mwmhbnof.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dwgsqepj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hqfcikmb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ckwmdrym.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nlejyadp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzbvxm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2tfgwnuhy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mzmmcucd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bivstrjz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2qdatnxke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlfwntbl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kmbvvctu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mkqzxkpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kveysltz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wouvhapz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2reautqkv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fedrqdmd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2awknotpu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2iylgtbhl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nxwjlztl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gnsehnch.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nevzgbxp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ifpknyus.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vaocythq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gszytjoc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2svuffcny.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ekxlhvbd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2chufjkoa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yaujztrw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kzdgndyf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pnsoztbo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ybqgfpdw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nrxjkxqd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2yucilmod.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jvbocull.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lompqqjl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2extgjswn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lsmrqmhj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2slnhzwur.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xsqeftky.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fhdfzysb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2krtmzssl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2sqsyseof.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wzdpatbw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2apcxngzu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kmgrxfeq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ssvtihns.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fnugfmtu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqwokaff.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sabvynef.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2beyqikan.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ojcdsmrx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ozykzqwv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nddrnevq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2almnkyyf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eboqdesf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cbbqxdlv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xerefkrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmaqzhec.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2lcveugow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixiusdjl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qduneldf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bvckehcv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kgmuewwj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eqshijdd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2edkglfdr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tllbucvp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2clmwigzx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2snhljiwy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aovsvsei.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zsakvovt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2kkirfmqq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2whpwqofl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2emfgzmtj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bxesnvil.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sgxkswgj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kqagcyhy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2enbstxxm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2syfpjhnr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kdqhelby.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zuqgaoms.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2izfirfpi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gbvbilkf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sxcnilxb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2feaksicw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2modvhetg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lihlcrbp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2upcnrnhi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zsfelfwf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2arsmdfrv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nratfkxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sldbkxyb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2raymmjkl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nprgzeyl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2avrvjnvt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jmhofwzf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tjzlwjjh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lrimzizj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ffwtfqng.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wtcsnpbo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wcdbtjsr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qfdopzdf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ecqpugji.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iupdujnr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfjcloyp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xuigctzd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aqhdbbaa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wvzclhsi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dhqbubha.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xljilbez.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rzdiulfr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qfhcsnbw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjyhwra.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yyoghrol.html


<!-- 参考信息 -->