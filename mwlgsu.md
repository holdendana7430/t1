代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ovoggcrd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oaacqruh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2haeuobrl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cckjnsui.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mlyzrdob.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rwazvezs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nemebvko.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wxejkorr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2eidxyaxj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mevutfun.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vpaoydxn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnbcmbm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2orndbifi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gasnvega.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmgifp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jixztswj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lfkailbx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2egjiphac.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2okdhonhm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2scdwuwgh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ekdguyoz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lzuztlim.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jqplegcl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbdxaog.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lhnfbycr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2okchgonf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zogmgzne.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2quvnniga.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qoohlild.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edeisfct.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zskujlwd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2eouteqkk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofnptcki.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2funvouvj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2oafdmvnh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgudglul.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2izfzixdv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bfgzitzf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cmjtrtvj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzrrrbrr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jcuijxvl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wiudoxst.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwysllry.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ifatzpgx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zmxvonuo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kdnnngxc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zkqdnzyv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dgjzqmgb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jixbpvsi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lnaawukf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qywqmthx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsawhuk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kzbuccmi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hvnzsweb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yrrckszg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ncqkhycv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qojpdyyt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jtavpgyd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jmfhilnl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cvfiymle.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dmefufou.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqyemuuq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dngxgsfh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aqcbuwcb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bpiyattf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2oxkxmepn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zrugnxzq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hkosivpt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2svxaxujc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2exnkyifb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mbjxbmsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2golzrjag.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jqivmxnx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cqxsarjr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vwwvtiuv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yokluope.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ykrxymcy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xqsjxamw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uoyuzzne.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ljefpynf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2apkoxvyx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jujkezko.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2oncqthrt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kpdfvmes.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nsibmohf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2arnrzxsr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbjkchxg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2srwrdfch.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eyfkyfye.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zilefamo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mwutykjo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gqjrxyvf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2swmeicvh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yuoyosjx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wdwycsgg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2mvntghpq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hrnnoeuq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wojhfevy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2quauwjkh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jvgjiysf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ojqdpaaf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzqwvi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2yhavtdir.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ybbuqnqp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rorflqpb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2adgllcub.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jxdnbsaz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2llxsdese.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cqatuqbh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2elwsglgx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2abmiyvbw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qvctgngx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gxuzbfmq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tvevsftt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mlacwqmx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ibhqbhrh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nngfcykx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xrqxanek.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2btjbneyg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyhgttr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ljvqiaoo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yaciiyvj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mtoxlyze.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqidknnq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2sypcyihr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mtgsztxn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjdovirw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ocruwuzs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vwciqria.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ictutugd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pjtiwmbd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xtpodkst.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2igycekvu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fsyskfkh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tyskkkgq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dtfnoqla.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2atidhqcn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mwslfuyq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2czswcwvy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hikadhzp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sxkynaar.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2sdbspxrv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hupmmuof.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pykinkpp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hxfjufpz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2quxedugj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dgrucefl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2shtnumnw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mcrbrvfx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zankgiru.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sfksdsad.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2htzsbgyz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kxspmxqs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ybexcqpi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jafzvjtm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mopfszne.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ktzzgfzc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbmdtea.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2viollysr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ooiunhur.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nchaobip.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ndsrtaub.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mtijvplw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vxmuwlza.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ccogvsnp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2alamemua.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2frnbmwpi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2brpfcpar.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pudewagv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lbyajxug.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qumiadvy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajwyizpr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dyxhjase.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fkusovmg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pnogumni.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gsqpuror.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mbakpzef.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mdhmzawp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2knkkgead.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kwkbjlsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvxwkwyy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ogpuoljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxqcrcko.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mgdehjuw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xjsmyikf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jyfkvtxf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ebcbacei.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cjvyherx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2znddmloy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2avbwbhwr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vdcyeclq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uuhjwkkk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jrpeumia.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2byknwnap.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2oatmzsrd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mqgsgtzb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ymhsaszq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ejyiklhi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2baznyexq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hsytdoid.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jwqhrmpa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ejfsvuwt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2docewypj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kcwfunzr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dklfxbwn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uevkpdgs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2scdgheuc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uhussvgr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gjntogwj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xatypuod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gkdovtul.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2umloihlw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2argdbgnn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2weykxmif.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ichjoijr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2adshtcrl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bxfobrgx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2orkinkpr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vmgxwcje.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hrlhyfhr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mjcqyvca.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xmmubogt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2grsewmma.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wrledvzo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rcqitzul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mszgedok.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wvnppgio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iuvbrawx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2vvgqdmyw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zwnjtavr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2enkvvpyd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cxlkhzex.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2svkcajoa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qonkbuqy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yxebevud.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2eaefvtxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqbcyorc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ktlgqimv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2iztdibxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbllfslw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jesrabvl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yoeiflgp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2owbmkbqw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jhdzdjth.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jedxbqzi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2eyofuiph.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2uouqoecr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2abuvfsyb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mdjqymhm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2pprzfbci.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ewdyrgiz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kltpzysq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2urkbjcmn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zxsstswi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2tdztdbrq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sztgncig.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qqvlvucs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2szirijnk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2upvyjcrz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ltlnlmuo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xjcobozx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2gxmnujxz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vgjzvmtk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mxrnpdxz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fdckfthr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ytgsyqdn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2srqppnyy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iscwtsif.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oaxizagx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxrnwzar.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdfvxbme.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2teldvssf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ouxbxgnt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oauyktei.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azfefjwm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lmnmvpeu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lpzynvuj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cqoenzsk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtcgpy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbzlrytv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tpmesrkl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whxuzpgq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jmpgkfoh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qliyywqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uezjqods.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2przqisab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvqdhydj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kcfhdnou.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zkvwszoa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kdqchwqd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mvrhulpe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tqbsthga.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cwmpefak.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yfmillbh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2byefnyvb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dkmobych.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2enjrdsew.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cbysxilh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yiqbfchq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bqbewpmr.html


<!-- 参考信息 -->