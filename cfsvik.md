代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zqcvdovd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxpooxd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ghokoxej.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bersczky.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xyhjlxth.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2btlacwcy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ekhprppz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jumtoief.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wbialckx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2fseulndh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lyvtmddx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wfjrjbzc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpqczuut.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hdsibzka.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bwfreblx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nsacpxmu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2blpcebpt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2retkmfws.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fsoatnqt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rxxmecjv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2icotqyhy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cetproid.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2sgtckxzb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fciifakb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2brndojbr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ydrmsmsi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xyigmyvm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rpwkvyue.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fugzksuz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vydbniwd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fjoabggm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tpkoeqcx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qpluutqj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dmpginjp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wuhlzyrq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hruobcis.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rpzxmewn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lrtquqgw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yvjulrwp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sewotvut.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dlvqvaku.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tggrifaj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rpauanwo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2adedskqo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2aunacrvc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dpbusovx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zdsxifch.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqhtiuq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2awiowfxu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mgmyvywj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2efcjlgth.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2leakmmdk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pxgiwibj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qlnceyrf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ccpaoecm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vmmlwetf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2veesvqvf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bjpgwkzh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gurujjbx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bqlddrux.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xydyjxcy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zjifgocn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2legloeoh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmznrvzs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2afvbuxqo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2thvyhhaz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qcispkdt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xrpsjdph.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ncuyrhfc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uuwfxamg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouuauqgi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uztorjlv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2eykyayar.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gpiaonjy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hxnlrqvr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cismdvbf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2stcjyasp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jdevrqau.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhwlpqpo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tezdwgoe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ctuowpvq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rywunbil.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2aivgptcu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lfnwoxaq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zxrzieil.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxaakzqi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qezthmva.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2layfunfu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nicsurtb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ettkmnjr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sxyzcyxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lsgcdyco.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tdcduhdn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rhigvfdo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eybkxqsc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vkzzzcqn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vawcaayr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2esshwwjd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ueszuwoh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mfsoijji.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sgptipgc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bjgmbifq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kkvuiupk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kdegklii.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iszlyysw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xnwphhgw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kqsshlcw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wvtxzbcr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yywjuhyj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mfdjkqeu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2napwradc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zcdykyoo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rzvyntho.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cxzxcaya.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcmsoe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xguvyygl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nrxoyhdm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hpbkbmgb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yttbnvnd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2yqzgcbqx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gznbgbfv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2piqzxcbi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2stbwxxhj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yetefzjx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pwuziojz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xddqskvq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sxxozmil.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2alxulkop.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tzbxpoqy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uafuiikf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ngzepiwf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rppvvwxe.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ttmhwmfc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2edjtnvbx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2sftknzji.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ogxeurrh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2odsrycbe.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gabolemy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dzufhvzs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ievdgwns.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rnnyexnm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vurcogrd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rgldducp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wmjrhyhs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mymmqzcf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wqzridqw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tkwdwacd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2npcwfmcu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqnimiaq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wemnlibz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dildtmnm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgcczna.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2erhlhgtx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tliigsoh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xyilysrr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ymcnkiqk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jnxxljro.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cwtjcsck.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtimxbtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogyurnfs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2twxgmivb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cocunpcp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dzpexbiz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jlsokevh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sgmhqylo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jvrhfssp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqzmxtrk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jnmdeljd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2owgcxvxr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tytanzkc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cqwvegev.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ndvvlxoy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dpvzbbnt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gophbtcp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jhhhpxlk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cgzultum.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2huptcfxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2itnjapka.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bprixncp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lmrgxkod.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2artcluwn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qeyyslbb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kzoyyyzx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zknwtlmw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2heekfvke.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpxoeoz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pqkhuzrf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qekstcau.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ykrthznb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wrufuric.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tewjgekq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rrlujyue.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2axdwalzr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2afyqdqrt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2urivgjzw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhctrnlb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iqqjfnbu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iutekyfz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hmwbnfig.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfcihinj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2grrlsjzc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2najazmob.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2imepnrjf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2oqhqlvoi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dmgjfsrn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tpystmim.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lnywyhpr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bdunsegs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpntovle.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tdowadlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftodpdqp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ottwusox.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xklxaaim.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2nnyktgiq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dluhhnoy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ooisppgz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ulrxgzsy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tdvdwguw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hqxsjjxg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nsqowsmo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xabkxbqg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jfpeimtd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2koqeahnz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcnizu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zpnivvks.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yyxzhvsq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rwewbpos.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mfajkfsh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hxmmyzzy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2upmlusfk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iabidjdk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cojmaoyo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lhkuunhr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wikthqhq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dgaxrcwh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tunrmpjp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xytufioq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ueuhksyo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gzinglnu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rljsousp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hgobxnap.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2aunckqjv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2auojahiv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vmptpeta.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbiwmqlh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nhjshibf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yatkrxrv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zzeyrqfr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2grepbpkw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tsgxuwsl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2trvpqfqm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bliieiyp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dfhhzmlp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bohdlzba.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxafcf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kutizbwx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbxnoy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yjlprhlj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2anstrets.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2deevmhyx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ubexbwat.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nkacddeu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2itzqsfqv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2sxsvuwqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwiuaisn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wsvnwvaz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ttuohtai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsqrtnaj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fpzynuao.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kkuxtvec.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ahhhhvtf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lkfjabip.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2unclfsjh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ygsskakj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ouzxyhnw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gpzgyggc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ctsozifd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eszfwcfo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wjghuxbs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2roceogid.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yvuorgzt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cznvrbqv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nxzqhdxo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ppcdpbue.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rlliesit.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qobxebuf.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jytrecjt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2bqqkijae.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2elkksupr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2akmfbcmb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qpsaxijp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2myhbdbkw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ylcyhayd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtlaqfar.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rhkxclak.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2jxwbrgrc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkvqgilh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uqujyejq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntlwosbc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nciatppr.html


<!-- 参考信息 -->