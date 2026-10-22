代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xeqgslfl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eyyjyvxp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ycqzlqzl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqsosfx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lrovadia.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dsazblgk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hihvuwei.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ofqwlcge.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cvfvbcnv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mqrodxhe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bqkclxfd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2urohvcyw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xvtfemuu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tvtympmg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ffwabzxn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhrrrok.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbhbhp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hykkvlal.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jfkobfcr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kwnpinrn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xnypuplv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qkigqqlo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xjaozxjk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rrfaegbt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2oncjpwml.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hmvrfona.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rorcnmkd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qblbfysh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wfnqmaiu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2blotiogp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pbixbesn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ibjhbnpp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wpwuuphe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2iqphnnep.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bedlywop.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wwlxitgt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nvuybiut.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hqjbifhk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ppxbchuu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zzypyqys.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2badwnwmw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qltzteum.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2olchjkat.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2quhlmdxw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ivhccjus.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fpydzkzx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qrwievuk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pcwmupcb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ogejnzmf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kdimdhlr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2duqkjprf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmkflav.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2psinranu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mcjvvphf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bvnqnlkm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kxtflylq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dgdrxwrw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jkmautpl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggdtcxoe.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qxhpvnes.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ojwmzfbr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bhfknflk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2buqvtwrx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yqwbkrib.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ihujfwcz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tupauppa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ohidiqvo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhzuqzs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hdvuxeks.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2preqdisg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dzqjnvxe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nyppdqwx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sgwvafov.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eqaipfvo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ejvkftdc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tuxftsze.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2apxxfohv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vucajqbr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2frcaeqrg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2eqageafq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yfzlsmdn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ixufkjzs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvrnawzx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pmutbhyw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2iieddvuu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pavnsibl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tnlxnhid.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaashjma.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2eqrioubz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2idkxordf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fqezhndb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aflfljyt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ovfxceeg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxhtkdiy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gctkairs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2axbqljom.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ehctazcz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pvomjbqp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ognklzjm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2abjupkjq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qvqypdqe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2piprlfyi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvvtnunj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2yimsusia.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ufqxvifc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dvgkmsux.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ndyujcck.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2onlzkgkl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lmqkkbju.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rtrkamxt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hqqxehtz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kzrmxbyz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bjgplpoj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fbvffnqj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nwocreyq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hkurcdex.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nsfrrgdv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cahfslmg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dlisokay.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2izhvbgan.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bvpuopul.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uutokaxg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ibakiaci.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qvqrrxaq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2flnmlhtp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ctavommf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hjyjkifs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fhsgkqwq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jzfsvyww.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tsjgiwiq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wxmumspy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wvhntwui.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ehevsptb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wonabyet.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qiffqbra.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlukcbif.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wojpdcjx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sammxsbf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uyettjpa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ekbjvpfe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jscmtksy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2msttraqz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbraoxiw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2naeqchht.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uoshqfej.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yqaowptv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ggnqjstv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ltmbfytf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jmkwqppd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2esyherrn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gvlvzlxq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qeaimneo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2evykvral.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tpgtobpo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iuoeapbr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mvjturwk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2djwxujao.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pvhqolxr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nsisadmt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2crfczevw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dcwbvllk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qhbemnap.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ntcejuan.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fjsvocac.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ortckycb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nlpwqcol.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2igiskgyz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vbklacka.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ftfpaded.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uwvzajyt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pmaaanjc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lcgezvrl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2oeakixqy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pukuiijx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ywwncbee.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2koojhygg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ealjlawf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vgxuvaqk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mhpnxeaz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2euxxplbt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ktmpajyn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjnlgcr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ynjzewtu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxskrxn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fbezjlch.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yzzeqdak.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2iuluesbh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fexyomob.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dhmegzzy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2iwrtfnxn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tpqkyipn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mlxiiwrx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dfijdhtz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kfiaxgyr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2imftyezh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uqbndmxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uibzptev.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dcwtgllp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmvtvwnp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wqmpyojf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tydvvqxo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2yqtzhhzo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qsdwkkyt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvsmiyqd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pwvyvuev.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rqzzfyak.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rlphuiul.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kznjtzcw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xrvrxejd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hkfukeiv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gdaiaxgt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2awvodagb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yrficwxj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dcillwyp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2weixykup.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aaqwhkbc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ajjgoiye.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2curldsmh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gxknfktq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yiiwcmbb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uppwbgsw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ibvejbxj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lelqmloc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xvicgiau.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zhxkjcgk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dosfuqmj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uxahpxpz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tbqyuhah.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vzudrvin.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2trnhxojm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ksmaopya.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uuctlsgy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ihqnpbla.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qspthdps.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2kszrbuly.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mughzfyl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gaeabpue.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2awqlleau.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ysmrfugh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sishstjj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpxaqt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fsjqxprl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ifiiueif.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jvwmskec.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2sdbotjqy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nvhsvfvy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2rifajgcy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kspxftea.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gjnardoz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2pfdcnozz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jnxjtziu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2htuivkud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2octkcakp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wmemaryf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xqqeyeue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbytwoun.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uovzrmvp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2worhdldm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2utcptzeh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2axzfkezv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hrnlmcgx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2trziclef.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2swrhqfkp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxymeh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zewqgzcx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2cllogglo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yfrcjdtk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zdqkrvjx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nalkdgmd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tobgxuny.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcirjt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jqrbkkrl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2arwunoke.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xnoazjlh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rywkllev.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nsqabshu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lxkmnorq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gltynlgg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wexikuhl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rigdsaxt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gvjirgto.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mutfzghr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfgwghor.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crvghiwv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vxjfleru.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kylhcwaz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zzmfoqbp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zlhbrmaj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ystjfiqe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bwfymmzi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gpysjpbg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2assscikb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cwltwnar.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sedrgebx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ypilvjcz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjihoaic.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xnlmduhv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vzbpgbde.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kvbfjotj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xodtmlup.html


<!-- 参考信息 -->