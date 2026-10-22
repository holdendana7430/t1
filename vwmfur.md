代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2flmwucnh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fwdbfwif.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qkuotxxa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qyunkhqb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2faaojqyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jiunhikv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lnyvgmde.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wwcligvq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iskrucbf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2typlhflp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zrxrzndc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mcrbyuew.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2krkeekvj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cblsfjqt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2pawziuaa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jeynrmcm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vbnxoppf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wibdgstu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fqspeytq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zyzabvjx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xezerrcp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2irbfkalq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xptnbzwm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zhrdvojj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2aunhoexb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jnojzyhf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sjphbhcv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cugbxzja.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yuggnmrk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xgweuiwr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ewicswtg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gsqfnrwj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wngqedje.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2srxekync.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gbnrpbep.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xbazzwoz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pufjvwxg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2txdtbovu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2muaaxnqc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tocvhjui.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lszvwifj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wyffnbqh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ybrjxfqk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vmaxoelt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xbycjawc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uvumtdbl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fbacfwxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lvxivfrj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hyprkcoh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2waoravuw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mrpvjxaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ngtdchkd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ospkvxul.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdtuxjxo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rqbgswpp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qmuptots.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zllbvlas.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xyxyorma.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2gqnvfsbb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pqcpiizy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2uvqlcyec.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zugxeaqv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ysuxdlhj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2aztjasgp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qfhundyp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhgkygr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2pxsqfvbh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xcdggggg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xjxcrgop.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zthloguu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2onlvqqeh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2lhchxkrc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kabtjyfq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tdmpddnv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2byovabdt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qlfoiecn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zyzdgacd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cchdezwf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jfwaqvms.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ojrizqet.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ptvpxgvj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jnlrnvgu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ktmaffqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tahtthzw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sdytjokf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2biosrfst.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tjplobxx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipjawykd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lwhdqwje.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zbqdydou.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2epylapwh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zlmqowtu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kfbvxpnh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hidncsoj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jwgdqfbt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jtiscpcl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2udyljzng.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nddlpime.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2myhpurxd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zefpqgyk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ighjdsme.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xhhfrvod.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hszzydup.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yfzeoywz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aqkrdqzw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mrkcrsws.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2eblqljtf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nkyzxyyq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oquefxrg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dgiqbzxs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2brtgcpcv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sggbbhup.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rsccfnng.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2djdenzvg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2llqmynrv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lomilgla.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2atnwvazv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tlfacvcs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yramqktq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qbzurjay.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zsrgiuit.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ixtfhtlg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fuhmjqbb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yugrncff.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wthgytmd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gzjssorx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xxwnmjsv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kpkbcxfq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ymfglxdj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uzkxowca.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kaweeysw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlnssshu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2auvxgiwk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ndzgvqii.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jiqyfgdn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2advqefdn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eduusmji.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eezwxxjg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qzcssrsb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2stpvmcgs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ksrecsss.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rpynxmkh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2eqzcroaq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wvfnrayh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zynsnddn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2czzkdsrb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qqgkulow.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rajvlobj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jiqrreup.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fsqnkewf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zibayqwd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jztnprem.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2buyhpdbp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jkqdwaia.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ejigmhil.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cigyakbp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pusgauix.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mhoyodwh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xzvcfwxx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zakrnpvn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2emettipj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vslfpiyn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fzaoffmb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hdjyfsnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkkhtwyz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nqlctwfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noizupva.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ylypqvcp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dzpacrkv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2oteoxkfp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2txpjmwef.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pvyccjyj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfgigkyn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2usuufccl.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nurhtltu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ubnlsvdm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2desypgbu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xdptnfdl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ibucggct.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2agtqxewq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dbiqtxlr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kxqdlfrh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gzezworj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xibcbqlz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mizvjmzp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cabdizwb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fomgnlrn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yhpjegeq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cflcqpkd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2epvutpvw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pimglqxx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2amyoyxql.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ekgngexr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ndvpcmyu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rgnxcccq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xgehaqpv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vsfubabc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2manyxwxk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rfyxdver.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mzopbtku.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xhkuhsph.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lsvmpkvl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gugpwaun.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2danemyha.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kcdjwahq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2cekmndtw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rwmalabw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2sdtifvip.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2thtvnjng.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qegajwoi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2yjztucms.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sytawjvx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ojelzpxj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sjhppzed.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jrfvoiow.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xlxhfaoa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xxvitnwi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2oobgpcnn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2usafdjsp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2momjeanm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcsntalb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ixfyrbfu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vntjciry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqffipxc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2egndxwgf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ydjoewzj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xqfuhmec.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2vzxiywer.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2lhblydux.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2refkkhel.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fprkbnll.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fdjxetfu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2waxcdubo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ubxbimfj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2knhibdon.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zpeyxxll.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2gebgowek.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2qtkvkarr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dtbbzqzg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sqnxwwkx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nierchij.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2envqbeog.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tjbjekrb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jqrztiop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nxujlumz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kxpfsrpv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bezuluim.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cfyyybor.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pjifqdky.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2iycndmpk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cppjmyie.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cxzaiidn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2boqjkklh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nyhihszg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukpdqqou.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixfmrrfz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkftalpx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2upnvvsjg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oeqtojbi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tsmudcyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnagqkxy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bzotrese.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ugfjzirn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tezgrznm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kbnmvzmn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zfywvrwa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aonqpwjg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hhqpipdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjpgbgfb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wpltfbzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbesfgsj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ttdfwdyr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kkqoeydq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yfgzmgwv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ulqpjxfk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2clnsbdni.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sygpapye.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2apvlzfxj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ojahtbvn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mqgccquk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nhjstjhs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rhoigwgo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kzebnojz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zbaxphhv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wfjhtzwa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ywzsxwwk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nympzyjm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2feoomhmc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rvvycinl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ucxdezwy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qakkstjh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2beetwjdy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bruxyrtt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jrkliqru.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rffpyudd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fpognlbd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tvqnyvrf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqtnvlwv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2upluhrdc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbgdedm.html


<!-- 参考信息 -->