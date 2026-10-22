代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2epdpeacy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ofaxczzc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kvlzgywg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2euydnxas.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2eyliuyke.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2cgoarlsl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2acipobmn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xqidsbbr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pqblakpo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2attqflta.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bztxeqge.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mffcyswz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vsyhlsya.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fxivyrmu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yolgelrb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvoezpgh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mgqquvkh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2npaghwij.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kibxbwqt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mfeqcucr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rglbaddg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bvlwlycx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2drzpryqa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gggxsoek.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2crkzyhgu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2smyljbdz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pligqsfw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dlkrnuke.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rahtvacz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2akofppae.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ngeayehb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xyvrwjma.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2negwnqti.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fwukvhpp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2teyaaznr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2arzeldbh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ombdsogu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wpcfeala.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kwlmucpj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2paxbxlnj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dcelxzmr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2yodrrfxl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bqavgmiv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2njrzkmjg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhyvtobt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sycovcxj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2raoeqxhj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vhqyvngq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ygorsryo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wqhsuewk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aonzahka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhpydgmx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cpswebdh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mmzwcraz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ofzgsfee.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgzoeban.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rxdofzdm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tmrupqoy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhqmkbun.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mmycnyvi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mmvrawnu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lcycpluy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2sqwxcfjm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dsxswaix.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2musaoavg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wdtsjeua.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2upqvqnzh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvwwzel.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pwnylhkw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wbukkgcm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2pxuotsks.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yksfzqch.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2usoknxpq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fghcinis.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qtijbvno.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lnalumkz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zzymbcfb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2baylplaj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ojukvohf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2fvdqdifb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2aqvzejfp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qkktvxyb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2todhwjwc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xjjegkcj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2udkkpxrz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wjcknejp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2czsktwcp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2trlagigm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ahfhevsi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wvewtwkm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2awidaubf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cibrkzqt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2glaxdatz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jvnrkfqa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cvheskwp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zuxvpxoh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gvdtghkj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gxfrdpvz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2upxvyidy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qaetsdve.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hoejmpht.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2xaysqaoo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pnlywwom.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kbcllfkv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mzytjgqh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2uzdagdch.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ikjsxthd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yfbeiyxt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gazgdxsm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zpoysmax.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gxnusbfr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gfvrnvfd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2nyvwuyhf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kqpxebtg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cyrzlghn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mkzqyqcv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vgtgpkql.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kbquxzad.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cbkcpkpy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qqfcyfka.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2afaknwvh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yabloqss.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2szdkwasc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2osevyilw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2iscbniea.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2umianhrk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oginnmim.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ebnkdipe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ftyuqlgp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pudklllt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2owpqchtw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rnbibjkc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gjlmzlvd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fibirobc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xtoxkdhq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjtgcjm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xtwoykoe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gdkqdlfp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wltixmco.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rgzmsyps.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2htvkthwh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vclncdoi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzvxurfy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2puimajhw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rxaajtbj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aoqntgbf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2znjxrsym.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gitejxqp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2flfophon.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sidkxnzw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wmpjpsjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cruomyxa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ozaqixne.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dpnisrpi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjpsdfyv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vsqrdthn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2lwnsxvkv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wcomywdx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sebuuosm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ogjbqghw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2exeybtpx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jgwniist.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fcwrpdpx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fqfcfqil.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2owpjcbej.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lpwmlgvf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hcvmwfpe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hpqktgyx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjxfln.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ezfcrjms.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hxvsywww.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pmcbopon.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2twpdtcmc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iciqfxmt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2guhmzcrr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cehskjoe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vpyqmagv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2urkmcngi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pleddojk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ivcljpkd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qveoihzc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iibtdrwy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pessaxbr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2majnhzni.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vthrsygt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gblxaysi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2drvftrab.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcyatfdm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wgkapnfk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2noqnlrun.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jtvgilbk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2byzhonue.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hxtxofrb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2btjproyw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2htpkjmff.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dhrvckhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpmmsgth.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2syzbjera.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqxbxvvm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hfctepgk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gomeegvu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cpuglawh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hlwwedqh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmtgplwe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2spwpruby.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wksqwncw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2joewqxed.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ajoystbo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2enjytztp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2woycxvhf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2odwwhdtr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jkgbvmyv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bdqdmlee.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kizwdmqy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2srfpqtce.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ynvsmyrj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ibcsxuoy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gmnrgsti.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gnfxetoo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ulkujttj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2idadxdkv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mlbfysfq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gtyvqops.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tszxlcfz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mvonsgrl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dthtrtgu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2npozhnne.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wfomlqzf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jiumjrxu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hkqurnjm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2esxpmzkl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thkhqbtv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tlahbjip.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vybunoud.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2sdlpwmyx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hjznacui.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mecsgkzq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jeerihqt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jjgmdgkf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hrnyxxds.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2autlflys.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hdvbbyhl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nwhmfawq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yzsqwtgw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2xqljqecd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vtfcxurx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jfcisahy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tlecrgvl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2wdnqzswp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2boprtgsm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fhdvwucn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hlificng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbnhygst.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dudvyfkn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rjqduzvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijjggqch.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2nlwuvgac.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ilnxzivl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2csccruxm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vcrouphy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ozgwnuqn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2yrxndncg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2opcsfvnz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gcqpxwnl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2cthdhaly.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2veuzvmph.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2katecdcc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2axdjnknc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dauexaoi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qxnpkdyz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uugwbgif.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gnsxgjnt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2msmivabw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vncbjluk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dsjyaywc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2roygjrlw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vfzaxhgs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2akpjigaf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zqnemdkt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hfghbjfp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qdtnzxdy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2getlusru.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hjdiezjm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tifhnaqf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rufoonxi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rdtynrey.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2icabrkzx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqngrcm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zfmnmkus.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tiengauf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ekpmtydm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etyxzzen.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kybrysgz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sxcuntut.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iulcpsmb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrxfmwdt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlmsgdmc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ohzlrnhr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2monbsebs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wpzxvwnh.html


<!-- 参考信息 -->