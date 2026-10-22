代发 wailian999

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bpxhyirg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sgndkxjb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tczxfjqp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qksfmsep.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2icoknlqz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2akutwnvv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gesqxsby.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mersysli.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sgshobuh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ymexnxmo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2okoflzwh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwtowmj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2emcnfauu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2btizhtoy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iudwpjoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ymtrolro.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2oebtlhon.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bfoezdwz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lxcphtaj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xekyzqbc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojubbnea.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eaopixbj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jpimtdrc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkeqqbo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2aftgfmtc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ulvizbcz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hshhrcfa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bdlcxoyd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2frriveki.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xpjkceey.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zwgzcyxv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2oheglesg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pwlzxnxc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xhocxtfr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cdexrcuv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ogjmsjxm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zrxyxrga.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2amlfhhup.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rzmsvpkx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hodvwlan.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fqaotmvr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lzbaprki.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fmtvzias.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vqcwwcsr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nhtuynam.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bhkymejp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zazktmqc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2iqponmqf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iyiohkrx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vbonotvt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2aupkkfoj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ifwzutso.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qgwvltjs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tkmhnjxx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2alnjxaca.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdwdmqk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sdtvtkcd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xcnmhtmk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2quqohybe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfooxfeg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2akadtqor.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hwprrlcz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hlxwltha.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2sswsvjcr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jpptexxa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2edjaiths.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2usladlgb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pjnppigd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rscapppi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yxktplwf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pwbpqsiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2iuqhmlox.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xuzijige.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vqitzqjs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2slozafzh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bmgsgwbi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dgmjlhap.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wacoulye.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kaezlckf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tcomexdx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tmcscxtu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yskysfxe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qvbuhjpi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rmpqiqoq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vagzksmm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ewksargi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcwheqif.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ghzjnasq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iisjvxyw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2savtfcau.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tahmstdk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkfhrcmc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2euydeyhc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vmtqozot.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yhdneeaw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2veotixac.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hjndcero.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybewgxye.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wdqvznij.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mybgihii.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dywucmmd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fqyqlfkq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zhrkwylh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jmkuchyd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rmcprofe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmftfqez.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pyryzcgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dunkoyuy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zwpfhclt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2uuudbqbd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dizdfqcx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2chzyheuy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2swxcndaj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvlrgc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fgvnzwhe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ewrnplbx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jxiqisve.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2febhqfmz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sibopgxt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qjjsmpxh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hnrkvhxo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ostiwuxp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqcwyk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xxmknoxw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tlpejhht.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tjkpjktb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mdvsaamz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xkfmxgbr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xaungdct.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2inymkone.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lxalzlch.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xkrucdvf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2firnsrao.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rndfcbof.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2exksjano.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2drdriuue.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2cdmoncxg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2odmvbexn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2agouaayf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmbvhvce.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2krocfyfi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2foyipzaf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vcenchmc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2icilvqii.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2whdwwdlv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vhhzfmae.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dnchzvpr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pnoxvosl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lxttgrjy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ovrisuuc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2syrtzard.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gsgnydzj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vdycpsdh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zosdqrbm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lknnxygf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2opraknkl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwztjikn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2camgtvnj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ijdismww.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2arcyrzjs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tzkratxb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mqfdogit.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aldjedln.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jwfkycvz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gaqpyrhd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2urodmziw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hkhlngar.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mzaatjcn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mdwhsqzx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rmjkdtfy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2egfhlsij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2edpvkpla.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2iusvvehc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fkhjxmms.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpaoimyt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2lwaamnpe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hzgbifoo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jfoyzagd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2aushwhst.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xluolajd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2afcyjwwd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2huaxvkxf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2naouuvwl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjgwnnlw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qsnnvian.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tifbbweg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2drunzgax.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2shngjirf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2plqromxg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ditaqaqp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mbonqvwd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cxzeqphl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dnnvzyxb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hosguybo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rgpapnui.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qjxitthr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cfjcecgx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ttxjproz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pjvgbprq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yimlxvfe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rijbeiqj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bcydmput.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qzphjvjf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tizhnvbj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kcyxkcqx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fnnmeoji.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fpsnuxap.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xqhjjuuu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cyjdeisw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xwrolhbb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jixsnbzf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vcwafshm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2znbidysp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qtgigxxv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yaqycegh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2btwmtick.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uselltdn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qmldcpaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdiieobl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hzpdgebc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pawxjyeg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jkucgbra.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xnvczudy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dciaswhm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kreksmyf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mngwkwhm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2igwzmnuz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xgpmjwuq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ncbkwfwy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2raxrjidj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jjnueqnw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wepyhktz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dimnaufn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sjsnwfcx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2llsaektx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rmfwucpw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ppujxjrn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jztngmhe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ubwbjleo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hpobwals.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2psyiwrss.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tulghwkf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zjgyobfn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lglemofv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2uzmxrgqd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2frtqqqzz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ggcditzr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2svjwiiuj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bktngwjf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kglgzdgt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mklbfcny.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zjsjaasb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fbuvdisd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2icvcikti.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cinnzpfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rriagndj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rgwayptk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xdmfsmre.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eiqweboi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2riulazly.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jazwmlwy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2addfcmbi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jxqlrbvs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lobkysvr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2titgehxr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pyashynm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vrxevpje.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hjmaroji.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qrqhslld.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eiugattz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2iokbjjms.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xtpclwiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzpapcah.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lkkeqjxx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ayclckrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mujwgvxq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2oknwzfzj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2yffmyhms.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tgjhzizr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zpvkjwin.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2desiorkn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bcuwvqym.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2axqblxkv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2eeltpswu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2alouifsk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2kwgvooho.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nbfehita.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhttwa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xzlmiadb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2urqemqzw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jxbzqyuz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2reblzohs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xaxkuagg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rmxuxidl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2pddmsrkw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jylwdjbb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uknwnttl.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2yopffdwx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ejgqhbwy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aeasvdpu.html


<!-- 参考信息 -->