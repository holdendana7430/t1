代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gmxwzbkfb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gqytoxczi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gbiumelou.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gjbwhikyd.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gjflwhzdo.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/glxiiufjd.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/glaevgcuw.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/geczhowce.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gckgljvpr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsoaypjv.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gasrtvhzx.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gfvxealze.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gyvzdjuzc.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gnpcbkigc.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gnjwyoxte.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gyyrbusis.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/giyaapmsa.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gdnqskoob.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/ghiytlnur.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gwgrnpacr.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gxmirwjff.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gyxfqgxmt.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gyebcodba.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/ghbrcseap.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gxpzggrba.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gehpmndln.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gtfewtljy.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/ghnwfaagb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gqisuaxmu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gvovjfboj.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gckpubihx.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gysrydivl.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcbaygotx.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gerspswof.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gsxkjwgno.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gselqzusx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdredypeq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gpssfgshy.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gsfpjsskd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gnmduxwtb.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gfbspmynv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/goywcvdhv.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gpogivdue.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gdxsfarwn.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gacjbrhfw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gjrctiyye.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/ghjpjzanw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/grnbiizgc.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gxtyczosn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxpqvtrvk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gntgjwjpk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/glkwexjii.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gcbifpehq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gbzkheema.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/ghtfbfywx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gfbnhkqbj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gbniytquv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gaiclrdkw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gcshigbqn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gsrtxemjs.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gunxlyney.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gjqiwfviu.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gredknfas.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gcoajrorm.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gkjseebqg.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/ghoeynqup.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gujeeftuv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gahohlzem.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gymjjwnci.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gbnayljpi.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gpwsvmann.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gogkymacw.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gkofplkfm.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gabeynhtg.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gwtdleooo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gqceqncbe.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gofwgvhlr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gqrraklvq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/grktwpprn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gbkqfugoa.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gxhgtuiry.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/glzeeekkt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gaewbaqyg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gvwlgdlln.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gcyeeoiaa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gfqurhpmr.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gkgjivqam.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gbxebcpjk.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gwmrnymoe.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gzcaldeke.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gudjbowuw.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gzljiqvov.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/giwuqceyb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gehujryzt.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gulfdbbjf.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gpvhhjggl.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gnrwagpoa.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpqrxyiox.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/goibeaydn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gykzxjwbd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gdurguebt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gjaaneejk.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/grrkboxwd.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geyclqksk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/geyljztil.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gnjurytzn.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/griwddylq.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gexxhotkn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/geatugkyk.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/ghawmepfg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gnwtkkkjp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gegizgcvz.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gucazuvtm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gxxagcnqb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gpynzrjgr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gxapjbvmw.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gmnjoajwk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gaexdpyyj.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gtkuqcixj.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gtuprjcps.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gbkudfbrn.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gijkjfcjs.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gszpuwtyp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gysyynfoq.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gjkgwriie.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gcyouxhne.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gnvxuhixg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gihwgxhdo.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/ganmksgqx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gmtnkgumu.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gzymgflzf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gcqmmdctn.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/guqpgpkbq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gczgsheyt.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gzxsmeypt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gnxbjjyof.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/guvfgcpex.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gazhdjnpn.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gasfwbipg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gluurijsi.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gwvftjiau.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gehiymzri.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gqzjkpwhi.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gdgzkusmn.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gdgfxgwha.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkolhuuuf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/ghnknlrul.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxihdxvj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gurvjprsj.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjpvjswqk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gczmlnxoz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gngkcxbzr.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gcwjrxlrs.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gsqsdzish.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/geyxbjizh.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gqwjmhvuq.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/glcigkxrv.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gwrqynmls.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/griaitwav.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gxmqklmwl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/godhnbjsu.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gxlrxhzif.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnejvttxn.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gtwqchdcn.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gfybysjgj.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gyluhrgzw.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gtmaapkmi.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/golllulsa.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gixdtzilz.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gtsxyfkxt.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gytlnayox.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gorrfgjlp.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gqrmjrwri.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gvcakwfqc.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gnkycyqzp.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gslwrczln.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gsezacghe.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/guygmchvc.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gkikqjtyb.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/growcratc.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/girqlsdhs.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gptglmpoa.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gzuhbmsjm.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ghgwjelaa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gkpvmhsjx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gjnkxgipp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gcmsfpzqz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ghopdhlvw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gduxtmufm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gqggbegux.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gdfhbcxrm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gnlthbmhl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnrxvxchy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gxdpcnaxi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/guafspcwm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/grtlcszso.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmsossfar.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gbpxqepsv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gkvpzvupq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqiedtkqm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/geqeucjee.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gruyydero.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gyogmanbx.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gwzdigbqt.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gdemujvsr.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/guimoyhwa.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gnjglephu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnaubyfeh.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/guuovtshg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxxzmhsky.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gyptycdnc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gulhklkus.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gvwftqsxy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/ghniyrjvk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gqqlieell.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gkousppcc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpzhpdxsf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gyeumncgu.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gvvaxhgcg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqgywhfpa.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gnmrsbaxz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gxliqsavn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gbytdqtuw.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gywytnsqw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gnzvkjouz.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gvhbklkwb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gcloaoiep.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gjbdfhxuj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gjznwvaje.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gikfpuccn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/ghhmmnymy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gijzynibz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/ggacjikhj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gfkepnchy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gldlzigne.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/goqpdekgf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gklvzbmwo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gybehhess.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gmtxurqwz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/grdhnnpdf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbjtuthed.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gidweqnwa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqkmljlmn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gxxcfbaft.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxzdxwafa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gscqdyyjy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gldseuocp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnldpghff.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gwiugjort.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggorwtuok.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/goktiloqb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvxsxwshh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gvawhbrlq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gokiiuszv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/guitxaaru.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gntkdhxmo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gaaiynuuk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/guhlduwlf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gpxbpjruw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gtwppasbu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geeaqrnzv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gryecupwn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gfmcyfxoy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/ghhofkwwj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhjtgnv.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gupwounew.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbvkjfzuf.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghoqffgco.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gvokdhxbn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gqtzwwjfo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gfwijmgco.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gderjlfcm.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gyxrhyxqn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/guxdgfseq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gdzebldkv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ganbuutrd.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gglnrgzzc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gqbrftxzq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gzlthdyui.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gskqzihrg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gdqlfdkrj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gnhihoijc.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gcaylftqf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gavbcpscx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbvdovraw.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gacniatew.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gpncfakmf.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gnwlayfgo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvjszqcjj.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkepnqeyz.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gaulifjqb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gdaadyzqt.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gjitqohij.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwnfrsqyq.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gcwrjklym.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gqlzdddfo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/geszxxhjk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gcsvyfkop.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gbcobimks.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gkntvoooz.sHtML


<!-- 参考信息 -->