代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bgibssle.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nveuslcv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dsllcrrf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgegcep.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ihtphxhn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrvvddy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqtgkgyg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wygzqxav.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vqxgnrkd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdpfffh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kuurbpcb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cvnotbhc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2srzbtols.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yidjmmfo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2teyosmzi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zrnmqrty.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivvegpxz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ctcfbirq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ltkfrusn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecvtnodk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bjnmdovk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xiiffhkm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2spflakhb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2glnhbsnc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hskcjxfc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hlgqmtla.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2eizlpbwk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mbcpufwz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2htluqymr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vokazhdr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlmoacan.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njzmxjoz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ctijybyd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2asewpevb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zawdqbsw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lxarfydr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zlsbdlsy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhebqmcl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2chbdgwdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hmoxejuq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ygvgombz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lrlslpxf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pwmxktfx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2juoewmbj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dxvokppd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aksrhpjq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndlfabvu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yymqgvvn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gsslkfcv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qbwglxgn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pdgkkxmo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xgpjsxrq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fmwdvkyv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2urqlivbk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xrpdryon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kmbgxnmz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2olgehxcf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2iicqfmsl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2nxmrqhgb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gwedvzet.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2njlslqct.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tvkahnec.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zryedldj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xcbgbwsv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2npitpyho.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ocjkumop.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjqiwehl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bbtqsyfd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sjnbgcjw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2slngcdmu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mdsrctnk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jsiddzjg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wnemynmc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nirkqstj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfojfa.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gythjpza.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2azmsvoxe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2djsuxwbi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ostitmhf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xikjtqqx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fzurtalc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fduidtpc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wdppvjyc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuwgnqh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qzuwfvze.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dniivfnl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2iokuagmr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ppxxvpvk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nbhqkwgw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zoflkpyo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qkhtmcpp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tfhryget.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ftblcjzz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bkmgrdqt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bidhrvdx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bltfcdnv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tvwwoaqb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hcpxdfie.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qcwujgmo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jguqmpfz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgmrlpju.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2obekgrks.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2osezrqih.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ijydjmje.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svovlwqk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2naytamxt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2teekpguw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ybdyjrrf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vqyadypk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oqcbroid.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ajvhphsl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxanuucn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sktdjlsi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2btndcgfa.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2leehvqsr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wgxhsvdr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ehvqwgxj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pzbtbnjx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2onxqhamz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2brmihviz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ldjohwxj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jkspgnmc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qxfcpfwx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2txqkjysy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2iplfrljg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jolxvzcx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kvuzxneq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qpqcoetz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2epmcihnj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2frnqsyip.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wqdkqpip.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2iqbikdsp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iftotqij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ivytptth.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pnbvmans.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2orpsgtfk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nxayrlrk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aukqozkd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rmumtyvm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hdopymby.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2chyitfwy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2srccyhwz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2flroymyx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ekliqpod.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2mtwivfcs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ymwbqmil.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2delmrwgv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xuziiild.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lniajhez.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hzwyqdcw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2llrkyjiu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mzgjygxc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rsgetoyw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2eqfhvvkw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hlrhldpm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cbbjaoks.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2myquwsjq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2iblzeckv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ytpbxcct.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xxwbmhty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnrhhmog.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2roqoaxco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osncpkbs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ijwcbwyg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cvfdflbk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zbgzejej.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2pjdgtpcc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eyoyklzx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wjnmtiwc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ruuyrpyl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mfhacxvu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ssnbddgm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qswhoeeb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zunnwzbq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zjdrkarp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2dpfiducr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jxwdinod.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jsnhqgps.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zmpcccgx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2naemdfmx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fzeopkmb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kxeplznm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2akinfpvx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2vkucpmfk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2brmxqapg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qttiekiq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ddzyiyzn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kwhfwidb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2raexzgwk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2joetuygl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xroprfgx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tmftupbu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thaetdsh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ayqgzvkc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kpsmozhr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2grnpytuy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hxzebwoq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zgvwxjti.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ctsjzqca.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wzrodjxo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2lfvuvtax.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2odoeehcq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qpqebkeb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2drjazidk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lepvxequ.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kiubrrxi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2fprswofr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aopuebzu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bsakmtod.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xhdgweif.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lrwyopfk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fqxgqkbh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cxtzyvkc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jgukyzzj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yeemkdmr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cmcelqmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfkphzer.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zufyipze.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2sebgkmgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpkdpkni.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2aticddcj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2skjqhaeh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ckvxgknd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ilupqqqu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ohugopfm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bdlbnrql.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vkbpwsui.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2esyzyvtd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vaixdeud.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mrmoyjnw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nhxyjynw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2iachqjzx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xbyensnv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bbtbgkos.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2naagavlx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2oxfeenfv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xtuomzyk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mjmhfspr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2drnemcan.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ygazmiba.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2glhkzkbo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2mooyzzpp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2anxkvuuh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2syluxpke.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2apervvtp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgnscuyw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2unkiawcl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ngbtairk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vnvrpdzb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgobvley.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2spakyvll.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zksvjjsr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ljxsdmqu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2chqnklwr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxhpqspe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tktsbdze.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2izlwhret.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2vtdmssla.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwoezgsl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bbesqjmk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hheeacoy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgcrihsp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bgaxalch.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2piopjsyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvmcabyv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2njfdbwco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srqockfx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uosvhbqk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fffwibbn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zuerpvbd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gwbxdljp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nlnqheki.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zdifwmmb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dfywkmvp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tkbyqfzu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pztsrflx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2oralvatd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zfzruslp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sauunxdy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wetbibwn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bqmkvyfz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lmzxppfi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2onfnelhf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pvmqkclq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eicndhui.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2zjreewrk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2kuesazyh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kiqnnvii.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aamicwip.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2admznmjk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wghzurph.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2tzymvtnf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rpnvfcze.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xznhblzw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2piygruiu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hfhvgmck.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2miylcwzc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hrjhzycs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2raabrtqt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xdedimkx.html


<!-- 参考信息 -->