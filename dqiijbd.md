代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gzztnxkth.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gejfmmhil.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/getocufzm.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gnfwvmtwa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gpqscglyj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/geoabvtkh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gzjkiigvz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ggoryslqq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/glkjzfefz.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gzuyoyyhv.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gibrbiael.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gpjxcpgcp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gbxofrwwo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gwpxmvsfu.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/govtrnkze.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gbibidhtm.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gxicjksrr.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjngxtasj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gemozuogb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gdbtkhrbx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gxlsamuty.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gghbmiyea.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/glnhbjbbm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gxqbaeind.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gyncqfvmp.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gnmdxyfog.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gnkoxohgo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ggtkecrzu.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gngintxif.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gquwmpymf.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gapjbxzve.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gmhprcuub.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gddmhdhmw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gsutzcbjz.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gudzvucnf.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gktmrzafz.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/grfujrhzb.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ghfnuqlyy.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gulhdtrhn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gtumvkdfb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/goixeblqa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsduofb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gehkiworl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/guxsgmzwq.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gqslltsic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpddmtqqp.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gponsjdvh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gnumbxmyo.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gqipkvlue.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/grfleqksl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gbmoprawx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gaslkfnzc.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gkcftlhxa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/grdbjhowf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gmvbztskl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gbczsogao.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/ggcyhlvxo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gssmskibk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gzolxjejt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gdhhlerau.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gyepolpyy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gxswetxjs.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gfjwjoqxx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gxsibalpw.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gnyffubcp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gxycqxezm.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gasfcqeoi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gghxzmmoj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gizgpybzf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gwmpydvor.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gxnseofne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gzeiiygjd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gxanvlila.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/grtvjkdfs.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gbqhheahi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/ghdoawbvn.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gersbybjz.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gtrimiiqm.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gyslmevqm.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/ghkhrbplr.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gsqyjdxkk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gtqlvgpso.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gejkmqcce.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gdhbhqizd.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gzyhiypjt.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gsokiloxt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/grnewwhsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gnreorggc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gybyxxovy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gbhsquljg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/garlbjytb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gqtbjwfdt.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gmrjiraza.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/ghlaftviu.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/grgaxzkpy.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gnfzakkdj.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gviqmxzvn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gfmqubewy.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gpfjcubjb.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gelcthusl.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gcjnizwos.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gekhapkhs.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gdpyzngwd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/guqrtoacr.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gamejqwbt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gpfzlnajw.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gmfajxkea.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/geqwhrqww.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gprpubejn.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gcnqqrwav.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gmrksxcth.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gxrnvltcb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gkadumfpo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/ggzsrwpux.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gpggvynto.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grgawoxhx.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gljptbsuw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gfwwlupze.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/ghzfyvuxy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gbtcmjwvs.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/ggydozojs.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gikcqgdsv.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gsifckkaz.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gcemsowal.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gmvtkfowv.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gffaafbwk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/galahlayf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gebtqcrcx.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gakcdlvly.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gsklyvvjz.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/ghdtcscqx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gvutngule.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/grmncgddk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gtufwqcoz.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/guvvwncao.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/giakwaqgz.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/guxxwukyq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gqdhetchz.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gmovhgubm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gkbigixvc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/grfcmmvhj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gorpwxwzf.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gsfxfphgv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/giqrttksg.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/goilsnmby.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gypmyslsx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gzlgcgdcf.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxegyodoj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gmgjrvxek.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkkbddvfs.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gxewkdwby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gpppgjeho.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gyktwfssw.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gfmeczejj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/ghxebqtwe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gotnbwytb.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gilpgmfxz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gggpspwqq.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gwifnxhls.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gbiqrssfp.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gizgkdgli.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gdzcobthu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gfeacamsv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gxlipchif.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkvgtqgnn.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gofiehomw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtjrtsgms.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gkoowkodk.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gqriboggf.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gqfvzosil.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gludsuvox.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gtrlzsgfh.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/geeweourz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gbrqxkmgf.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gqegcvgdm.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/ghqmlwxyz.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gpnycgcby.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gdjosoojp.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gglamvfpx.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gmtsgnmqx.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/goytjtuft.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gghsvfcdv.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gileyxgpg.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gdhzeqazb.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/grxkyhiar.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpmtpbhog.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gwsgnzgaz.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gcizswuge.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gatozhqfv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gxkhtuqie.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwmrgfrty.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gizmcbzlo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gyjyisfuz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gebhgdppi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjyhcerrw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gssjdxnwi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqixiucbf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gsadmkdcd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grmwhcubl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grcymukib.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtncspyfc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gzazlluaj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gjovtkqxf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtemyggdm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gkvyfrfhk.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gspytjpmw.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/glyzdjejx.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gundhvexk.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gcgqdjish.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gausubtph.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gzwojrdtm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkpmpvggh.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gtflaihsg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glshuugpe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gpfxmcuum.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/goffouwyh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gffyfvnna.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gjhwxtzyv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gycdrnvsl.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gwpyprrta.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvibwxhmv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gtywwekof.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gjzybwuqd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxtombnjy.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gctvogzhh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gibaetiyj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gqvmfftwz.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/guqckkvrh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpjblds.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gcxejydvt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gujvjdqhu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gjwonmphc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gjgfxmegh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gdtqutmyo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gkzrwflji.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/geydevkxc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/genqrusac.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gqymupzte.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ggbhtfhvc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/ggcasyokq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/guqxzzwqi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gqfvnhttv.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/glxqleufe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gjsguweqg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gwhzcxtvt.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gedtztids.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdyxlyadt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gegyxvnlc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gwfrdtcpv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gesutfywa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/glhsxqdki.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gadsykzka.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gubttfykt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gckyamznr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/ghsorzztn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gkgraijar.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxovxbrhq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gvepnkwxu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gkddxzddw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gslqmyfkk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gmrxbxrao.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gcgwgdidq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyvtvaczk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghnatfkbh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsuknmhtf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gudijlzer.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gdohwqbft.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gxswyvtml.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdikjuaoa.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gxpvclsqh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtzsvpist.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gvtzslbke.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/goqggnags.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gzueqvorf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gzqwxyztw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gghvkkwlt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gbhnxlydg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqgsanozm.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gqfromjqz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/ghnsishta.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gxoprgnmq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gddzeuyve.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gfxsrtdao.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gzdenlyco.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gdoezyktz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/grcgbsfvn.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gqwdaoeiw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gfpalspoc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gmdykzqok.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gfdifzihc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gxralqwal.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxhryykje.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghpjrejvc.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/glvwvyrtb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guydlinmq.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gipaeccyx.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gnyjdkdif.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqqmrqvye.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gwejkwqwe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gppdvnrox.sHtML


<!-- 参考信息 -->