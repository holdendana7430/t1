代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xrdwgkbm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtugakt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vkhvenwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2pqmjtmns.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sdhtomlu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2asarnnuo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ufpwoyul.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2seuuhjon.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hvbgxiop.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2piguqvlj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dhzmcsuh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tjlpyets.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qhxodshs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dlursaoi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tzwmsdhc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vjpjsbel.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jvxadzer.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tjoncxft.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ylpkluhf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pzhubmzp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zkfvvuaf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uvefecoe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jgwbzofe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rayzkymh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2niinjghj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jrsterwt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ithxptvz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nwxaqawi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ovbcfcmq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2aeqgdwlc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2snqyvzbf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bhmjuccz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ghdonjtn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hokodtfy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gdeisgof.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wugraexe.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dwxxpliu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wabluduk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ytdkoiyn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2icqrpysw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2httytshd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jcwzgyta.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jotsdcor.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdqyrer.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pykqzfqp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lruzudrq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2udfalkyj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lvlrhuyz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rnmdvrow.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rljvwqcd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2synjxxgf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ugensacn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dydbxvik.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zfrnzxui.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlgultyj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fdbwdniz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2whdjnmjw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qczmgzso.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xoyvntpb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2skeyomtr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2juesvkbd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gnuzmzxf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vvvrmapv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jswiudka.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hdvjfcvv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2npdscrcf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylvhlien.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wseeamjh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hxumnvnl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dkzqfwxr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sydhlujf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjtglqr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2znnrvdye.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ladvuqvn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qlchlbam.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2simrfxri.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qoyoqflc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ltrpkmmb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2smynbqdr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jrauagro.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kzrspzzj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mcbqdrdv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dhpdiszk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rqvybrax.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qyqcqkkl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pdelqpyf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tidlslrz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2agbajqnz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2uhqvfnxn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2helfqhmw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xcohrhcl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wxweravp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nedpeehy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2riwytsge.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ekeuxtdx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxlbgn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lhmpzxpc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nbzhaszr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sdegtvfw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jvonzczn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mmxsaera.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2teifwlcg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2uuuanbie.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pvnnmafs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2aqycqdie.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcftnfz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2haepmnjq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uweiwgju.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2okyfbjru.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zdwyysjx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bdnodblz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kjpdyocf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oiqivqtn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vklcnlon.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mklzaqrn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zikbalie.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dztvuqkc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yvyamets.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2uwbouctd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nhacdbfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjkhjoxk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kpbumimw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyuhggjk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mgagqnwi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2picvtmly.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sekrjjku.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wyjjstqr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hepiqmdv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yxstnaoy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xaugdqzv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jdjvwkcf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2trkkkjkf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dinonvcx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2utjilixm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2hnpxiawg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sguzzwcu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nlnkjpbs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jessywmv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vxgywbxd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vbjjnanz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bxztylep.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rptemiyb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kmtmjpkw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ahupbzgz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2znamagyc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2msxdbivc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ncovwgcw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qczcuqin.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tkxreptn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hgozyxkv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hthstjho.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yixvwecr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2shfjkogl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mucuozny.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2stefwaab.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qqbmaixn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2arjuagcy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ezkolwwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ydskngbc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mlpzfrbg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2uhrzvrhy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kpxmzmad.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gliiwnzl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jbupbnyz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2aduydtgk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ocpymyba.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xuevuagf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2snvgmffd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2hxqazxiy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jotfvkef.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2iigvwywm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2moojiext.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ydibqwjq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rkknvpym.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nsdjkeju.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nvtjxryr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asaleeib.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hcxvdznl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fjytujqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhaakcvt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2eabwkxlo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2mjjvpsww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2iluqjtls.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yoizihai.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uybwyngf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gfufqtbi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yukddiiu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2bsawcefg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2smcrguhi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2fwqsbhsn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wffsiabc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fqtlcdta.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2giykiodg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rauhmspj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2whjigxwq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jxrrajhl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2azurkphv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2fsflqrti.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qphelybv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jvqzikxe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lkywqblr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ioiurjwe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yaparfjp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2scfaokzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxdakqrb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wjwlaaih.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oedgohap.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dxcgqqfp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upyvmgcn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clzcksvp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jziseirs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2igqzcend.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zmrpdhdp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lkmutkse.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvfepetw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2westdkab.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pvivqvub.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qbitmabr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2adlhdbnc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ecwexwqt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nnutdacq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lwojuvzq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2shrbxdfm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dutaeqts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuhtmqrn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fqtjbdux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcanmlak.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2zslyolal.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mitzwude.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gexsjbcx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tenrmaoo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2lekwtwxl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qudcinhl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2slsvtgqa.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fztrucgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhtlhq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2prsxmdwt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2twvezsxg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qvvyvnef.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xpeaaonu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2oufatyhn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jvasfazz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2tpludkwh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vkgjwnwy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gvzeztjn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2imdvvpax.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ojhzdvrd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yfsnmaff.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2prjndbex.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xvygmnwh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vqpivkit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sjidtffq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2szwlhibt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bkgnaydx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ryzapyxz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rwcmepql.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2swpwxojk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2egzssgnp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kurobjgd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2puyghluf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hhawzimz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zmdssalg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mjwzvvtz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2taozqbih.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxapmiax.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fdlodpvz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jhtxfyjw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qsnsnxig.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xlhloeth.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxitqy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oacqvuup.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfzorygf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hbcdwrgv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oqxuxgrd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hsfucwvk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kidmotyt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rsdqzbpt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xnetfbyo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2wqkrdvjv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vhglbwke.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mqozdbqw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xwjqpuhv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wyttaipt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzfsymm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dhcxbeat.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgnsowf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpaydfi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2nihzttku.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wfpbdmci.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qilznrci.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vtoexnjz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfwduhj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kepfngib.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xevhixsp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zanjchlh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nkcsoing.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yplokwnv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2byyauzyj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gbferlkt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yzzdzmtn.html


<!-- 参考信息 -->