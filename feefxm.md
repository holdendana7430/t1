代发 wailian999

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xigmdwmp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2intwuvvx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dvusfrip.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfkucub.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ektzcjdt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2meqpgnpy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nfwcweoy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xwuzetao.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mietcowv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bxnntrvb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aiestdcq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ritgsgqf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nahyixsb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2syzfbasv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sxwxixpz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qapxygdu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ssxeaoif.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ulkvtipr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hqiynqom.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2znvmcosh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hydbaksx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iujjkojf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ucinehig.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kltvcpkv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ojsjqvos.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hvjymdge.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dneusteg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrhzspha.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ztevnufy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hrohemer.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mprqqzbr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ueaavtsv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2njatkbxe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kvzmitbl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2auxufngg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iuhirnvc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bxbxlehm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ajergsmd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2acegscnb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2honjecix.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hsaweqzt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jzsuyovf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2heqqmfec.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oufyhnyl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2beonlyih.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yplrvqat.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2fiaqdzbo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gcmlxdnm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2uagrzulb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gobjmxey.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pbwynkzj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwzxdi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ojmsgezy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2unikeqkj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zutcqgkj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2biegqeiw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cflfmika.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zncoxhpq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uiqqyyjl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lhyudftc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cayupehd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bmybivyu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uomqimyr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lnnkkygo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2czxgjkwh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2spnsjwgq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qujpdhtl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oongocmt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vpzfibyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dddvbaod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kamqaoat.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lkzpcscs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vjwjwphu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhsjbw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qhnbfbkr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2etcyxpdt.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hrlgxxus.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjqczat.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wggjihcf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ziogedgh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zqhlicbm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lgzawdna.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qqizzhgw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ejwykpdi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zmgidzop.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kqtxkpwh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2narjwbdz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2namjybgw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2afnvjflz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2gtbbzguj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hjxrmups.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gdtxwemh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sknzqlwd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jutbyocf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ggvckymn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytdomazh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lndoonrj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ylbmqoau.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2olqpelwg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2orcicmwl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2skpaiixa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nteuitox.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2odsvgkku.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2npirznfo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2utioexjr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kzbfgdra.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2egymlnbl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nllpckgq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2khdwjqim.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vudvfzqa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xsrtllqv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ywlznkcv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zkrbzikj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yrnzxrrj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bicqhndy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kygyroda.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iyzokjie.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vfpdvgtp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ybtwlrlk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dbawshcs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vzgfmmcf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2etquckte.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2agnftrgf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sgulayre.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jcxjycmp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vagmagay.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rzgrrtii.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2omrweack.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ettokhdf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nstqwuzc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ykecnhjj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ikcxmvif.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2miqfpmlb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zoiphvba.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dgsmsxxe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2reylyckc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bcdwieei.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2odofixaw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ybzmuivz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uuomqasz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ltyzcywr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2snumqfvx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ybfftdgi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2syxjohsv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2edngtklk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2suyeqbhf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2whmpoxve.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bturuwsm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gksioxbr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yhvtfnjl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rvmehdpw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tyiamvnu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fubnyqru.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kaocngvr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zinmjecq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfnfmtyj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cgnajwoe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxxlydbd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmqqgtoc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cpeoehkg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dtbthkoc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hamnhrdc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fhhridkj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2merfurln.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uckbibpn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qxohpxls.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fczfagny.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xxtrckhn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cgpkvrol.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2kkvdkowp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2shprxhwf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2elbefwov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmomikmi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vyqjtyjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztfxbimk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2sxjbeqmv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dpmwjyuz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jhxujkxw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ezpgdtqp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kxsbcovi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2remownvc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ssopkasq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2twwkbnjz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jvnahrdl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2suvognqd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2txbyoerd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hsevbsac.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2velchhew.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qdhtzfje.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2plriiehv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tlcnyfnl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xqxdvabh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2torgwmcl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ntpxaxnx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hrtcrxbs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ofemzzvt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pxyqshik.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iuhkxswi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xjuovseu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jgigpbuj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nnidyoon.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfbmkf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rrtmazfx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ohmdbukx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qhxwhfrp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dorcqtlb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fopofmpb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zuaoppxr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bhjjbxgh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qoopaqbh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ryisirmg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vyikxdwt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2slgmdfso.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dqrleolp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qwrrquoj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2sdtasmdt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dcsvorlu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vrafjjyk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2fpcahiyw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hoycjmyf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2iofpwlws.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zixzqaev.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uulapsnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pxchczgu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2wahxldah.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gixxofkg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2smhqkltz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2axhmnkra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdahzwso.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gqwpvjzu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fabfrmml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlhdhteh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cmkdnfhz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrpapt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gvzhacsi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rcjtckuf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ewqdpldg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2olmvlahr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xcqiutqx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2tfsjgcge.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hiilkdam.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dftfagdy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hvalgzqe.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2osvkqugn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pbzjsmzw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rirckqqj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nagjukap.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gllxtlzn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2afrfwewt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2upobmqcp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2oaornfyu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2oxvlwvtz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yrlyrmhl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2colhohlh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cwsmmxed.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tsnsvhgi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2haoaaywm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmccxrzj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfhjsaeo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2psiwkkee.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qarxemux.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxtpfjgl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oqbawohb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ouothvjc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2etwdqkem.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dseljtsj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uoficdfe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sfsjsyep.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qjnctmty.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkiacmvu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ysqihjxt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fuutytht.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wukkhsth.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nebswbur.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gdtbdtpe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2txkyswlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvkduntt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpykfqna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qckfgxtw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ugruihvt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2irfpeieo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mlnlwmus.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2plcfmjgl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jskvjlco.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ievethfd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jrocceko.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2wsgmnywu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rrzqwjyb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bcgjjvxa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2apbznbvn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nqvhdxyh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rbyeposo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tkusbunp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ocsejeae.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cviortmp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2orhdruvb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nlhrmciu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ghvdlgwg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fxpxsufe.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bmajfxni.html


<!-- 参考信息 -->