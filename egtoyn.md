代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ovsazdon.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jsmazdro.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pwharawi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vraepzzq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wdofhflf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gbengdhu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oujlhsqu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pcbxzznc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vooiqvrz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2awsylggo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kpspmavv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ywkacyhg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qjflrrre.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ctcyzerv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dmsfgkob.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2avdcmnpa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fxjwansy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qwtckyni.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2axcuryao.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jtutcghl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2phauysgn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lbqsnllk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aetrwyjv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wqepbgsa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2govvqwcu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yolixkvt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lrylrxtt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tqyjqhjb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xiwyglph.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vinmoafd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fsawylrx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hjpsjpir.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uguwckac.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nqcinqcj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2amqdytpp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fbuqznrn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ljksvwvv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rsuewtso.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2plqgrbqz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2atdwoghh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nedczulj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dlmrmvaj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uikcwmop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2cqrwqjuw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cwwbmgml.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xutdvpni.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2szmjzvna.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rndfxysa.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2uuezofhk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xazbnhgl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lxmtzdcf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2flyavecf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wopnheyb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wwdwltdw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vccnrcnc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gzgkkmeg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eiaazjar.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vikadven.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zuvogzwj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tkktxvuf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2luqjrwer.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dvasysif.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2embepcqh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qohrdsjg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kzcihdmp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yodjqkoh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dmunwoel.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dtxkcfvg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xqfoojji.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xiqsgprz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wfustuqq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eeudxjuq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kaztqnye.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hvsvijpx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nflcqpik.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2svdthljj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ymihdvzr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rwdhbqxr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2yewnkovg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zyrlffvu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2udruymzl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jdmppwde.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qtpewgem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2sdftwqcn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2svlabogk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nzwhfzkf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jelbnsrd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2chkopjma.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ehmsdsma.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnegqz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fytkyvxg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2voddcwxr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xjffpeqx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nbhaijoz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qxyimnnb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2buaozcme.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2iyqtzcgg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bnfwnyga.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ybeefkrw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvgakxv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wdjrxdrf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zivdxlcc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjwpnu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zullqecd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whcachrd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oroecvpz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbowlpsp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xdcawyng.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ppmxrjkl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cmxqauhb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2daprkvsu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2buzpjnbh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2muatfhfz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gqcotois.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sqcuqbvu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jmfyitdj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2quujvfiy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tjgzwwjn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jyfqoesb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2arperdog.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2javslzkd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2klhhkwlp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2azojbkza.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fudfswyl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wnjyvebf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2svfyowfq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kyjdazae.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hdomdoio.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nfdiktym.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2clpkzoza.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghmxzoay.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ijmevnxp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vbetrzbv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pxstjsia.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kgfcjjny.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bielgytf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lbfuinmm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2imydznqc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iddclyxp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2okrsdane.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kcaehrze.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oanycmdk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sczxpjnl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rjeprgbx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uoosipgc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikddweov.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hbwdklon.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ksvcsise.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wkulaodi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fgvnzqht.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vwxeuwyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwizfaxa.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kajijegw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2lddsuybn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2pvfjsrti.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jqlhxbfk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2oujlcruo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2focicafc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hhemqewa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2guizyiel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldujynyk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcqcji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpevyfby.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2okhjhvxy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kltksdml.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xyewzvye.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zqpbrdmo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ggjktmzv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bjwandqu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gjopkyug.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gnksreka.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jdlfauzj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tefmxoum.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2azajnktd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lwsocvks.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qiqbmzgx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uzvuvcxn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2hkamfcrj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mnshkneu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xaregxzb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bqclgpsc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axwdjgtv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vcgurmvx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2palegiit.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ecggxmpf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ibindees.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jqhbphlx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bumqssqv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2stjwrntg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nrcxzvwx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2grrjdrzi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bbwphfbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vvfewdgc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eebibmvh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vandplrg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fttgvdwl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2erzzzbav.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gnizdxgj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2svdsjvmk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yzdkqoft.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wydfmkuw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jjognray.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zbayyblw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zrfgwoar.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cgyxxlzx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2baqoqzqw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2labhmmmw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zroavuyp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pkbgcvmz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oofeawke.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2sgjmoali.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rbjxljkz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rdupmokt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2psyukjbb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2waizzcqy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sywaawky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kchdcfea.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ucxbrqnq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ccofuiva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cigzsqsb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xzhkzdng.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ncuodguo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2idtophhm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2nxykzieo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2asoxgdgu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2belkqowj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zvjzlegm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lgawtcsc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2miqimgxj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2thmgcrun.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2chmrwhah.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vybnxygo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kdogjnfw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rjsvflbf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mzdkmmmn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xdbpeuiu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2dxlrygwx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mgniplvl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rhlyihzr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2mugpbiay.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cmqnuina.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ejvcnmoy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2quatqidf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ibkfcopl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hnighvcx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjnnmxwh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fetjzqvg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkajqiep.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yzqamcpj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hfryygfo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jeepuads.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eddnbrzj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvzlbvzw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nrrjenrs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iroomjda.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evkzrxuz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2piobsbys.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jxpwjczi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fiqorepg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jtdamdyi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oeqyjuak.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ctcpfhqc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mfqswskn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2godqkled.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nolkirwd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fmfsyque.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpcshpqt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vbffrnvd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2apiuaaiy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fcoghwcn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hkqknjjy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rpdicxkt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wxinyxbz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sjlfqrni.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tmznlzbq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2flniadvi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vlxslmkd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xsisscly.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jzyyjbht.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tcagjfsq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mlxkqacv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pdrwoiyp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nlebqvqd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fspezjsx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ialgylzx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2uuvmtaju.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2echfbzcq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2widjerkq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ndmstgqa.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hotfcasa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pawhcoqs.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rndfhnqk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jocbmxrc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ctykzkzw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fzxxmhqb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqrssyp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qbvmkujr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tboguxqj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tvpfxhmf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fyrrtjrt.html


<!-- 参考信息 -->