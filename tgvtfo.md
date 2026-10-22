代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kgxowcwc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2glpghxxv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fpdpkxjv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kogykrpu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xbbppvbi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vsgmwfom.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xvozrwrt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yiadugzc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rncfmmbz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sytsvrpy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xvtjctid.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ugecyxcc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2oeudjrfx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2egdljdma.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2llzcyrho.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jnkjpwjo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pzxpmjgg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hjfaloqr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yvlhdhpz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kmljskpl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qbzqtpob.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hjugttns.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fhmpkbem.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2setxieuh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zcaplphx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2txmyryci.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qhybzdzc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsarmos.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jegfybah.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wqvrbpai.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ashvgorf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2sxxfejqe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vcrgixrw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2inevcupw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2duqusfwa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ekqrakht.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ijtobpqe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uorgbfsf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xetvfdha.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2cajcvuvd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2evimiicq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jtqueflf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kchybzun.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uiefjplm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dyqxxtdk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkfofrdv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2szhvcxjq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mhdjwvfi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lvnmdirr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ukqjyqth.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zzpndtdq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thvxxwvv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pqzhtzsv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vkrprzyq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ygqdtlff.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhvjxsms.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zxebjslg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2upyenmzn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksnwkukn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rgbvcbsv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bxlcjefd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lqovhcoq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bttgjvof.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lgwazczl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ltymuurm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aqzqcgre.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uqkaeryz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jpgndgfk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2axyxpzqo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2iusokxuv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qswosxmr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fohnimqi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aochbxdp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lsrpiwud.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2emcwjhme.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rclvpswk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mjgyrwzt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbnyxwel.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ggxbwihg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hoomlvpv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hpotamet.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lpnacfmq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2smsdmhrc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqskzq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ynyqpnlk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ucrbizec.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hjlrghgh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tvbsgxtf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jagugcqc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cynojnhs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tbvjwkgu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2muqmlkdy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqrbwwau.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fptsvlrs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fwoduxzf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dnbenolx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uzdovngc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ooffmumk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sdyrrloy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ypirskoz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vhtgxugu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2iojypwin.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wohkltdx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mimxuifl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pqzphhbr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ywvsnttz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xpmgqjxg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gwpejgvz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ypnzycia.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2aklsaean.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bdcssrna.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2chbsrbep.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ncfmovje.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hrnrrtxg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zzjyxizi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vrimmbmv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jmacrdby.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bkcshgum.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hyszytlx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqqdeui.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xocvcasi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wdamsaon.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uvgjfllq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2gynylufq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lzuinnkd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2znxfvazj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2syofhyvh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cajgpckw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wdbyjjmp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yezhmnse.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fnhlwgsl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wamriqga.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jyrnljxr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ozfauswa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2govbwoye.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dbfmrzid.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sozdpewv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ckcbnmmq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fucwvgxo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uiybfyhe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmjvwqrh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2rkuxrcoz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gopruxyj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pqomfsqv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dertjvjj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ynrtxlti.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tiyxceqv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrnvozh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sekyfuza.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jjzzkakh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cqwwdvqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qmrvyykl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ahgxfytq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dtfhymej.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijmtrwap.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pcgmgegf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yooldwev.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ngvjqamg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wdvqlfsf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kgytptph.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ouytzals.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2snidkefz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wtqpwqyj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kbbpqchi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2oabxzzle.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ijbioflb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mtyadlgi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2swjgoxhi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cijsmfrc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2thxbwfsg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2chhgnaxo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2sytquosy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjbdvsmq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2taswxceo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hrmijsav.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2viwyplnp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2iqrhiwsf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2yudukzrb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rxymjtdl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2klnbkowi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jxqvkekk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ocqgehri.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yniekcpz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gqvonzft.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kygyxwob.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kvooeblj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qflydata.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2keeiufli.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dpyqgegh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bkigyiee.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wwsfmahp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2eykybkol.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pbbiqbyg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2kesltqsa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fzcuxuga.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mwlezvmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnrayhgq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kcksukan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbrwvafr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2thkiyagx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dwqfsnen.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jbxeyzus.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2actzltmj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mbawzoki.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kgpypdol.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hbogygmg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yzdshjtw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ketgltee.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kuxdxrpa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2plxbgxgu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ibscdpta.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zgytnaff.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zeqbrovu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zninyrtj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2irwwynpv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vaxrdaab.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ysbiefxt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wavbnqwv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rfdbailn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2eqdtccsk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2igeohmrh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2szfuheah.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uecumghf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tudolngr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pcjxsrkg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ukcqlagi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hxgllxuu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rptarqjs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2peqnqvky.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wqskmujq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jkhjxcnx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kxqzljro.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gaazskyu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uapieryu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cscshxnm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ktzzabmj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ffwvpknn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nutaflmw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pbutnclh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pmusxffk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2clfvveur.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pntfpkhc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qgetjixb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ishmtjtg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ncdhvcnd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhivfzsf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hnuxeaeh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2olubcwbc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yjadvhun.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ruadeayb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vnadteah.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2mrkgmgew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dubkfttx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2obvgujut.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2csyhnxjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwgmawnu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nvimozcv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ujvesxtf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ydkecvxp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2qgqswpmx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bxvpjhcr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zoqcvzob.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ufseqzmy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2liysnrmq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vtkhklzq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ltecsuuz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2coeyjyyq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2letekqdy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xmzwjraf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2yjjvlnqw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ihaltcmy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2gojrfnbv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nkiejvfk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mifhqxwv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kmdzxsej.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zgpaslnt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2autnazzm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wxckxpaf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dfuofyol.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iehbwdeo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqgejsip.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bxatosro.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yvqlswoi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2szywaodl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tecayvlc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihyncgck.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2efqdduyq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rzqkkzmy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nedqawja.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2otprenla.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rtvqzjql.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zkybauwj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldvgavzs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jaltmqtq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kawwfzjc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lglkprxw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2avukgdbg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhxsujgf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yvyjlnvc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zqlmefmv.html


<!-- 参考信息 -->