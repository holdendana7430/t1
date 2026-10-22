代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ccjsxehd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2txbikcov.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xxvanskq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bzneeqig.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2kxuzbfnx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2sdztlrsv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mmnvcamx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wynkmgab.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2crltdmtu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2okwowths.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cckoaypv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ccotwvul.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xlaogryd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pujzeylv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fyqdtoiz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2osinrqvs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2jzvykqkf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xbjeyruu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aufvivrg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhimlqj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iubeyqmz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qkvynxdt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xlutzrqg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gfndycrq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2brqpynng.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2buungqnx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mdudjdid.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jaknamnz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2tphvjeyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jskhbvdv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2morhzvtt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mkbrypbu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mbennxsn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qyofvfaj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbbcwwuy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zgvvbakn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jugvanrp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2weftlppb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ogsgztmc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vcwwuizt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksctcyqq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bixmbrki.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rkdqitxy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyftqbw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nnlcqkki.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gxqlnjld.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mljtuabo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dmnmlqol.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gudrbkog.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dhdaucxs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2focesdss.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vuxdswxh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zkqjxysp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zqtkijmx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tkufpoma.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mdevnuph.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uvjcusge.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2drjfpfhg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vacyexfn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hfnzpmom.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mhivcyya.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wntrudwy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bcumurps.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rowqinbb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pqkwagqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2acfxzrts.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2liiroqkd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pkwvbquy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lkqegkqa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hoctwoqk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nkavgrlm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2unqnghvp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tmxfkqis.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qskrbiev.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mxyibmrp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xeedqefi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zwjgbnsb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bgibeyce.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2banndkec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uaorouit.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fvjooxrp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rmgaohle.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dxlpgtzm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2esutzdgs.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2whvnhtky.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vctuiqqs.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tnludicw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bssbuqsc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lgucjkyw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2upmkxdth.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rnfwfukb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2blvzhzno.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sbzskaye.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2aravkudh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vtzoahpe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nkxvqoev.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2myagvpdb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jjduunkj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kivqhbyv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jummpusd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xozgwtkr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2quhhjqkc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lhraitwz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qwnbmxrx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jzsstqog.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dylfjqsv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pmileyrs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jfrnhyhn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ailijslz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gkvdcbis.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2omsaaits.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2opycoebm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cctqxauj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aozzvwlv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bmrbivps.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2sawqcceb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jjkyfrzv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2esdiyjpg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2peadfykl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2csxmpjvv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bmdmbqdd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fjcaiwix.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ynjmbaot.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ezgvscut.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gmnjxokr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2apglseyg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ahgbmmho.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sjpvryvw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ocvguwyr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rmkbqved.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2laaaqvjs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yspbsutt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bvznxyeu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oaerxhxf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyvtvsmw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2btazopmh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dztrhpoz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rgkyikiz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kxvczurp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqugdgq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2govteuxd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2umbzwwur.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2apalrdpc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ntnjomas.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gtqdmvjz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ccxfwspw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qocletsb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gtkadonf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nfrehvdp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2teatcius.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lycfnnvc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2utotzska.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lnzhwygy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wjzhxxxa.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qjrmhzas.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cufvjlrw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xhpgzlfg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cdvtapjv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2shsluauo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2otfpaafn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sdvojdko.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vgyfeusg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mexdmqza.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pxipakxb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kojpodwu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xupduwnk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2csgofgtg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bpbgqmez.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xacihwho.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wagecjoz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2alykhtct.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nhikxpew.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zynjhakm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvnwddj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fpjncvoq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xtwlztcn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cmyzsqkb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jkuaoptc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jebiztcc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gfohppuo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2axgebgqg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xofjiqic.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2gixgtgog.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rbflprtd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ojnnatog.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cwzmkarg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pcvdtjvz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gttqnlls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dexosqlp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zfhoytfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjnqwjoy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2orsxjlqx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lwtawajw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2enyffwpx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2zdrtrhru.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lvfngxhh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eiswrwvp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xgpfzyld.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aznnglpi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2izsykuyq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hwkgjeep.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qttyucsc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zobjcltl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qoobgvat.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kulqzmhr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xkluuomc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2egtvxkau.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rqafxpco.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ekgptqqu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zhrqeczk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jriiqjvc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ewoeryhy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ctxsrwry.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iptoxupl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qtbzdnqd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ceugkiyc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2umhsubbr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xibwkcuo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vmukmvek.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ciymuftd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ubvtqesn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lhnnqcmo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hqwpcwze.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gtscagvv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2buetxtze.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dpuzlqwo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2uthxxebh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ycjjlayf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bvgcpkxk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qnstypdn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xolntxpm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kqtiubqs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vensdflp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2swrkniua.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2awmrcpox.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ezuwtppb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tcfleaxq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2roqzpxta.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ibqolxuv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ptczllaw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2aegohxxk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2joctzxtj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2viqzmamx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2aawqggyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rehxmkba.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wdovwlip.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lvzwwlea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkpaygnd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jjykvquk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dmyxusig.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xtpvsefb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pxisingz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wduqyuon.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2nmybzrjc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ydecvjho.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qahyadiu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2uitxohft.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ecoguxpe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xxwcsiph.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ldjtjrfm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2oppvqkzf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tpixmnas.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2cdizodeb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2iukjkrap.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2deztncnu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2brlozjvc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ommhrxbw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nyvhkpgs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rmhhnglw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yatfxsmm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2etkqdbro.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2twhzyqbh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ippijckm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dbjicaxq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgbzvoas.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fiywabpl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2azmxllkq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggggshdq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbgiuira.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hosjcxon.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chmfdwrg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nxhsncxe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2brgcyksa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yrpggebj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jenodoyc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwwsdp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wjqoamrw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nxfaeqnr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2owhpixug.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ucrxlbyf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yfinhfkc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2odaroxms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmlbmfss.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2snarnbkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrntwnqi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmdlkhtn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2iqxsyeqn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dvccyodl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rqnoebxh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wqzngyxq.html


<!-- 参考信息 -->