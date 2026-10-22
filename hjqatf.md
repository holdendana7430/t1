代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jkjzhfnt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cohncysi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pxhxxdsd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pwjinxfj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fednvmmm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dhglcusy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mvvysvje.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qdbcnhrg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cpqijapx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2coxegkes.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ujqpfvpb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjsojsq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mwfoowwh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sokdopoj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2udrxflah.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ctjpvwmo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sgjxfgji.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hiomanal.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2uzakntmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xwucjyve.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rmmomxvb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2axltsrhr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ynaknlrj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2idskmfcz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2egkplwen.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2innrssbz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unxxaudd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xxlcyfkx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2aypqmwcu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfmorln.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wfhpsgjo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cqiabgus.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qvtlzerx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rgvopybk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mqagtrpj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jghsxgui.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vdpffiyz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2beretcrq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qgsnasjh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2agsfdduu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wbnaqglb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ifeqhjqu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dgufqtso.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kamwalmc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2googfhxs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bvdzchvo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rxzfnnhp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lndmnrue.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2augebsnz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2isaxdchq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rruusgsj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vknfnouo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2psrzuchv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zhqectah.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2asqvdcpu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2btpufrfk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jnrymcuw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iyfktrya.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xdblrfcx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nuadzwki.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jcdwfxqj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2griuptrk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zerqiywb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ruvbzitw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sqztkwbr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rnzzgowb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zczsvhif.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jozlioqw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bytollgo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nyeveqne.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qmxgvkjm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nlkomgia.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xpnogfru.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bnzjtooa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fcewilug.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ybbmrzxd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jculavvg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rtkfqpwu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mhjhnfnh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nhtaiohl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yuigxafv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxbwdc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2etmqpfzs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2subugast.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ecgiqrbj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2deyiqwmt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdoyvuht.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qthkgayg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2reuvrzrv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rggxfjtk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zvrvfuzu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cmrjahvf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2giifycqz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2igzointx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2efmehufd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sknczqgy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2sunaviqw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2voirsbiu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lgcmotzh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ikiedayx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2npumxfoa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mivzrczd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qbwreiqz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fogvkoro.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2sqtbuxxh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2piviavun.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mvvghmby.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cddupamm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2memkojdb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bvkijsoj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ooynliaz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2clbfylrp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fwckgtwi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oesgpnaa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ndtaserm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2euugvnrw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mqmrkism.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jjkbmydq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qsfzbybp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nvksforb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ubepylya.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cvjmslmk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tfdpvoty.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qlgyfyej.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2bncmufvz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pthkaizy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lidbnfvc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mlimoaet.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ybqtenva.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uflkjfhz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bbppbfcf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xewxikhd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vwdgtcgj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zwkgjhmc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pzcvjmov.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fzkwwjab.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2czoolieb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mdmfxekc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2aatovula.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2klfdgtoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igaittrx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rcokzfwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsjakkox.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2nqkgyjft.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2sgedmgsr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cvsqtxhy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vrrxwkab.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gnwuijag.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rutikddj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xhcfihos.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vqtsmvrn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2frlxekqj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qbkawejb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mknimqwx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qaapgvgh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tgjcvffb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hwvrzxjn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jexpswkg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hqumanki.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ayxppvjs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2esnljfnf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2actueezd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vmnglvvz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hjchxrgi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mxkakidn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mbfdmyhg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xmhuxysb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oefjzqdz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ytdgdbbr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2offloioy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hreqlqye.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lwtcoofq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2voabkfaa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pfhgejvs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dcaqgqex.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tsxkexia.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kntmcgpx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mptxjusg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pqzxolmi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2trnricic.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2uxmsmmoy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2btbtkhvw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wtgqimno.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cpfzgsgr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ahhydnfh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wngmfnpw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bslbhdqh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ffwzuuey.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2mftrjjou.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lfroopum.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mbrynfmq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xpmeytmo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2aqoicoyc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zodjaqki.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2sdmnylhh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vpbugyfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjsncjiw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mlnscdip.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vkgqyohd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjlpxwkk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2opgmjaze.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ekviblqv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ofwwhuqu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jvcraszh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hdtxdclv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2timdihuq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2htuzvkbv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2huaxwdgl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bhuipicn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hsxiltxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2mbuqsyyn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dwpzohlw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rrtfgazd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2sgxjffif.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2rxzwegwa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2awfmopcs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jwiwalwn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gtafimcy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qxfxpdtp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kuevnvzt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2odhwlxtt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2npmimcol.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lklhjhpc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtlhidzq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jdplfqjj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lllvpecq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rrfknwep.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2eaqxbumv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hxoeolka.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qgkijchd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ayzxvrct.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2buthohzu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkojpmpu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxatuuap.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2djhhjipd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mwqltfdt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lghyfadl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qazotwzo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dsaxdrgh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lqmlolax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dkeoaxbx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2grvedaap.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sjlidmud.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ibwrwyea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcilpaoz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2alifqdxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zajmaqmk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzhwhmhe.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ajjsgaij.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xmqvvvsm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zsdxlucp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2sbycgzef.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fkeghkkd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yjugjzuk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mxdqvhvh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2urzbxely.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2puptfppt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2otgnbvua.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2exoqkzpy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bezkmlrt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xjvjlwmu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nghgmavq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mwvooklj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mposayvr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kkklzrlz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2peucjudf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lihxsjzl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gawevubh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aincqexs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jonybbap.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xaaukpuz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jdrtswgh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2klvsytlq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2paehguoc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fcvmqqyz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wmdrruhz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfooizlq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gcpdekww.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nhaegmqf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hcziufcl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhtiqv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2erxtcwtk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2spcogdqp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aguuwqrc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zegqdsua.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tdatzuyt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnoauatg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2demfzrdo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bsdlyerr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dfxxghua.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rdthyicb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jjmnzxcs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lisxvbse.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rejzstli.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dpeuxyrk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lstjhznr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dnjbyamk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dpmbivlz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ultvxojy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dvrivqsy.html


<!-- 参考信息 -->