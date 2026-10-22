代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yeoojidj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jqxcziku.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wtkcnnxw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yjwwrqpm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ottnbiic.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ttyakvxe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ljifsdsm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2texlaxou.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2foizfjth.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2calasfzx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qbnggnnf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ttqluftc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fhxxbqvd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2roemavxu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zruezgyb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zeakhofo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2sobgywcc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wrpkqgwn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hfpkauss.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vgktvznb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jnovvnul.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qsuizjrq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2slqcqyym.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2heykyytg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ndsvcnkd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sxyvosxi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2axqpceas.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wyavoxzs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2twwkyzrq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pedaxbul.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjgofphj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vziaoswm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2fdnxiicr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ukiovklz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gqinejzb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qohdjrva.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqfkia.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2iadrlllu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2heaqbopi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujamuowc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2knfgkufx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ctjdxnlt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgkrcpcw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wfeueeow.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yetiquay.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lwsuzwro.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vpxclbxb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vbftmmfk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kismsgkk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vrolnfzn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zffnukuj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqekesou.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qmchulef.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rircqafg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qyjghpvj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tsejoahp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2awjjtidg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wphpzblu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qrwurnah.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uayehnff.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ayhgmcob.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtehrihw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2skwhahnk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tnnkqxga.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kgirwvbo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jjxrckvm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rtfnmcqw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uwwsrtiz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qfixujil.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2svwsxjgs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2smeekwxc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aisckcfh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lvhbxrgn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ppxsrqqy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2idqrkqdf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cfgblkfe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hpbfihlg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgnmaclk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bactcfbp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jnsuqzkr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqxput.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zxddymep.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zdgrmvql.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vahbhxga.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mgqiqhoe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rdsonhvj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mxxcfpcu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jimkpjna.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qonbxytg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ujbtvyyw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kzwstykr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ynkfjpbu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mpexnvgk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kselpkaa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tdmmfvdl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zoywtjyz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2smrzmkqi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2oaiwyuxf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zkytntxe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kckculvw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pdefmuml.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dgncgbbh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jllomaxe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtiuajsx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bwdqzowx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2njjmcwgl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2asbuofwt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zzvrhcrt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uvgtauwg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2phrojyxt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2aalccqek.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pjblzbky.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rgitbklf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fpebayna.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tshuovwj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2arajvdct.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vwonsyrm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pagwfpws.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jcpbavdj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sifdmiuu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zwkjudkc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnxiph.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mzfubcjs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2triprigz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzyrfmlc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bamfgnsr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bykpfhqa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hxlzisvb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ldtcdpzg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2keoxgowp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zgvdkbdc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hubumbmd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aixurqoc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uuwjnrcg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wpmvgojy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2eefdmjnl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jghhkhzj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mwcwvmfn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjjyinkg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kanwzbqj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2czgmbshq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rtahqeti.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hukbnejb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qaqjxmxa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ywozxxed.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ueotyxen.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vsklziyd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qatgjkdo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tgkptmto.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vhuanmov.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gsuruila.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lbzylcka.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hsurlveq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gcodrdho.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2uqsnizzh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gxiohoha.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ncayyvms.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvswfzf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2paawlfkz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cggyiwcj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wibqxhdy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lrffivsh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yxvkpuxr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2czxvdgag.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ublmhgvv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrjhjglm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tjnpbvon.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yedptutj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bxdpuwmh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xkskjeeg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ahjluptz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiwkimxe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yxrzlqpt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fncukuzu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ooigxqmz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2olxkhpxe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2urraprox.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gsuqksfb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wtwcaddy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wxyghvha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2romburzy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lorcmfht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keklidah.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2asqxezym.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ndjmrmzu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xlqkhaiv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nprcultq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wybzerop.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kckytkzm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ybapduob.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2chvqjnab.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vfwkcenl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2bvnjedps.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2goxbqevc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mawzdslm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tzrsfsdw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hpxzufoe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lyewfpxh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qaecljex.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rclmpzky.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wjwvxulh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxyquhoq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2psexgtzr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mgwrsrvb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ufbmsmhz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ibiuyjbk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2msrjgnsr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gfledebc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2treagdlr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hvtseyeu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fcdnkvxp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2idyevjbe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vozdjupr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ibclovbu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2amrjfvcw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hedgxsin.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ngsfdbus.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bbrcblec.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2tyfgfxyo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oohoidtj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ejuhbhwe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nlmoldvi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ptzwwjas.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fjlxjgri.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fmtkazwx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2btjwyrme.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2gjxwbuqi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ubyypwqf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zagrfjiq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2otektfyo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2alapawkd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2arcbdyjs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ssbqpcab.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wzfjvqus.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rkbyolmk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ftnubqqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgnzoiut.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2itauhqds.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wnxzivdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpirinyf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2otzggjeo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2vcdelhgf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tgudsyyk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lhzcfvba.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2epyqqjew.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jmaisgzl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fhsvjcgr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2szofxweh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kyoxsnnw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2vsiiwkyn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2weakgmft.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2hwachbrt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jtdtboxu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vcyvojcu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xtpinifx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ocwcseng.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jgffvcrj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wehnbyam.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2cmukxiqt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ziqzxjlc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wsisbmpf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2fxtwusmi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cerealur.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gcacagxn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2firnvbdb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xtqdztyl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wiyogwus.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pbjbadph.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2amgkxzpt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qofwwqgc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zcqaovli.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whmsfjyh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ghfmebed.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lvvjlcaw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2smyexvqc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qovxhgan.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okrhowrq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fpoknwae.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pvrdusqd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2tdowarvx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgvyxcmm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xwluaulm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qxxxsscg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndujmwsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeacwamc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ooujeifj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkzaggnk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2piheiavx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nectkqff.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uwplslzr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wwtkgmdj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qootluaq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hvlxsnfn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rzzmygkx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cppvyeig.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vacmsiln.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfpzgo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2aqjnlapy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ycjeozji.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jowaunjs.html


<!-- 参考信息 -->