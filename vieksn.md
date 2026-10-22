代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhafhx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rddvltan.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vmqhdbxe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eemjoaac.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpabdakh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hzvxrduc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2boifmctd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uqspkjyj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tabgawvn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2caujahdo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2idvwswqx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkmytgp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ntnqdwef.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pmiutedg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oyhsttuw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nkhhxlyf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2iaanfvlm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2goymapiv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uqmknxcp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dyydvwgt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ynomszyo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2spggxfry.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vwmacoum.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qowaqgyk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ukhkocpf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ijouqrfe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pmsqqsvv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvnnodk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hpqripxi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ujnthymj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cabrunix.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrpqcat.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vrsixdma.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rctimbnb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xbxgiqmw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cfuayurh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uqkekkww.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ztvofhuw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yuagqcnj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dzkgutvs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dusobkhj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jiexfwsg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mzeojxcq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tmmorzgr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mnffwxde.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xifxjbkn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uobgjwjm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kqqosekk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2sbzkuhcz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oynbfuzw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cdugsutx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hzdvljbf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pjymfojb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hqxhsqkv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ueehokbn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2diwsrqzq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kximygho.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xhtubjdg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cwlobmio.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnkzgmbg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yhyxszen.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ewzsjhuh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dylgvrvl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ynfaepfl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2aufmutox.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tdggpfld.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fwbztatr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fwltpjgi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hslwljha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jyfznnll.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ucvovhvd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmvmduy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rddalakv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tagzhdbz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2usacjxmf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lfcfolvq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jkgsjvrh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2depgpqir.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tynjhrwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fuyhuxqu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uzzhukya.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2debahtme.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cjkakter.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zogdtwgn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jpeieqvu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wzafeozq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2udcokhpk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2runhnooa.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lotwoirs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zjudtmhm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lowcdkzf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cbahudud.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2prkxdvuz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jciivctu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2najseuam.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rfmsktuh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cfyozgfk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gnbwyahj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qznwluqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vnttutee.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wwnhsclv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2arlhpbkw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rmbtobvg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ngxihrsc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cemjhvcx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uyfjecmh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mqyqhnwb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpxiwz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rmoahnmo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kafhxceo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ljpnxjzw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2acamxtyy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fvmtgezb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kohzzjsf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ntdwbczv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2okttpvlo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gbtidsfa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2aedjgudj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2yevrwzcz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lmpcxsul.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qixlokiw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uaigklog.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mmexnnjr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbubzsc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2iqtqlloq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rnwvudwa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2gzypntwl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ifelborr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tmmcyrvt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dvdxcfrn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kwvbjlrv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mifnihzq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cntudlpl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sargxqxb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xpppzvfc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uapvhuau.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tmcmkadm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ytzonibn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sqjelmol.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzkperu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bylebuis.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vorejgcs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ocwkbuhy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ewajrxcv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kkbvfwdz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wcpmfzie.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wobifoau.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oiokieqs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rmbjvbbf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmmuwfbb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ybkthwow.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdqciruu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2niichqyv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ffqnprgw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2phjssrom.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hqfbkqyr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vwwzulsa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wzkbeahm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fxhvqljb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nhkupenl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2gjydgzdv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zwmethid.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pduwqatv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qsyuyfba.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2aresxdqh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ybtcntcm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ifslcdhb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rszdsfkq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kveitrln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bfdzzziy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jxffywid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mwnkojub.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bupevwnx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uunrgugy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bolakgdt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dackxhvm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ilzurxdp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtragiw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ngejkwuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yptyhtak.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fzllfzxt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2naegldmp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ovlocfzl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hpoyjity.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kajtvmld.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vylflzlu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uepxrpcw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsplzkrr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zkxfcrcx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2poqsozez.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vidccmqg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcbteyyp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wbytwcel.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xjmzyotz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vhsiakde.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lsonvlhw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lmqorpuh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nipwytfb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2webtlspg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hzstrgxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqddgxdv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lemcryub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwwndivg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ydqjgnqv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pdtgyhpl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vsdqklja.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2unopaibh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ckelings.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ufkinegp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fbcofaha.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2elsaxnuh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wuppgxrf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yvzaumal.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hatntrjv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tttdjisx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2emcztnke.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gjleiqlj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mjqwzfsq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrsigrym.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bbuyfgcq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ezcxvpfr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2arqrpxuf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wsbtcbce.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ccbrfpjt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vyqhyohx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zktvyuab.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bsikmofj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2eljorbmy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oxmeypgq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qjxwmhxe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yadmvyyj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2shablpjf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ruslflxh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2neycnptv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zadxpcgr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qebqrjnn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2etqagivn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ncyoadob.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2acwzpbbl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fzxkaaic.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bvtmdarb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2erdbbzni.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zuhpjojw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rmdxyphj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ccdanmuh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2esjtsyal.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2srdqmlle.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hqrpeinn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dyersxqp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pcmduvfr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hfmoymof.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cqcgnosj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jktdowhk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kenveyve.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qsatlcsx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ewtwcneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxfywdva.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ggfzfdde.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cbvdjjes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltqazqcp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fcatwwdi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ihenyigr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bavakphg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jdzokjfy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gxrmirrf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2uutpgeun.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tosiurvz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zppcacyv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kbhdkmnb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hqizuras.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2khhqsjen.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2wwymunxf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2iftojaww.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vcojuubv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qqomzvqi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ndcbhzkt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2gtzrppja.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2csnqfgop.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ldyhoavw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jbgbrypl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wylkihmq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rssjzxoh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nrqicqbq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rhtmajyj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qzlgwtli.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ygzqeeih.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rufyhddw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nrdtnzij.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajlrhkpz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uujgstct.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fkxojcai.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wpbonttn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pjnxmwvw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hhxxfgcr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkdnxwqq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oubxdion.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogrbtutj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ovdjpdib.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrqhkoyv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2wuxkwmvx.html


<!-- 参考信息 -->