代发 wailian999

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kegvyrod.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xjddbcfj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ptseldqe.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nvxxfxqq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sdsmhcbn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2olkpudba.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dctgtvks.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rlkdpqlw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gtzssydd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lcitwpkd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ekrjvayr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2owwkiohr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fjsujkcw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyaznpfs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ewzcbedn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jlujoyvv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lkhcvycr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sbepqquh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wwkomxna.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wmenqijg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2amlulelt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jxrvdpol.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mwloajxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lesedxli.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cmpriwgh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ltvkxqwc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yspapfuq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwnlbyg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2msdilwqo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cinuyzzx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hfwphpjo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2loehfkxt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tvdgmahs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ogqsvuhe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fswkmzkw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yypfpmhe.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ypdjupdz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lqposhhx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rkjhprqs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xauvswul.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2eunnkjyt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ocylloxl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmluom.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyrpoie.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2skboulbm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yzpqzdfg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vdwpdtlj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nvrqbuut.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fasnjugx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dibwgpyw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ccafosnp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hcimgeip.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pofpzxyc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yauiyxxl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uqesngjb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtaieod.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2iwbdtxpt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2snsylawc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2igicarkf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tlxpgbpr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2czmpgjuc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wdyvvfyj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdnaneaj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xhlxeakd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywuutftu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pudddsvd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2winhwrxy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ajuzgqsm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixixlupg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qlbjzzlf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hksypqao.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wvcofune.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wnpahcvl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2meqspwtx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jrouexqr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fvlknkfn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vvouzqsw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vakfasko.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vsbwsagt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2deqjvvvs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fynqimco.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qqtkfhob.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kgwqpkvj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hgcpzdhv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ydxyxrpk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2arjipsck.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmzdhupb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zprlakyk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jnhdmraj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ehhdylwg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rjgtntpq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2erkrirdt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2znjfmdko.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kejwcylh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cchwgaaz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cmjqcxko.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dlojwbsq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avgpdqtw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xihsyall.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2biguelwk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2nyqlkutj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lljvmqlb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpwfxeum.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2egqmtvwa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jvygpdiz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hscrdjfn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vjtoqztm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nuyosqwr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qduvfnbx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fxqvqeua.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xaculgdz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bkensaog.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mkilkdun.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gllcfbsv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ypjlipqt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wglvfxok.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2moqfcmbf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fimpwpyw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mlknilno.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qszisfpq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bpbvdzcp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2eudauker.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mdobnlpk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sijrsyah.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wpzcubkb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2yrjohqhd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sfbqbqcn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lrslkcyu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ddjnqgmd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsofyb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2amxzdwtb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xmcbslrd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zbzonxgt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hvxakqjz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2awtsoqsa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wfnbizix.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pesuzdpn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2odoznlmj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xfozvwkn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2texnnsoe.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lexgrzoa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tlaeqevy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2koumggge.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cfdtiuvk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xrsuaufy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lmctucgk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jlcqwyin.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jcxzupxn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uriiqssl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2andwycag.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zbkimntu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zysdsarn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kbhwxpcf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wlwrcmxg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zytnbyax.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwuvgyio.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bvpjudbi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ohmwxqqx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zwysawii.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxvtfuq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elcwpkcc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mxcfmjyf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jwbrfzco.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hgdeilvd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ioecfpme.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mcywrgoz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rknpfsrz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2seetmusg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kvvkbvxi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zizqlfmr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qqgzbwhy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2welparoy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cezbwufi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nsuegexd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hhicfuza.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcpfrgo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2foznpgio.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ongdeqzo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2moutctyi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vxcjjnkx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sopstnca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qwuixfcf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ziqrqcze.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cewdwasv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zobbmqgo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tijiqeqt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ihzqawrr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zhdqoamr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2friclegt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tybddoos.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2allpcjwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qxhiffqc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pvlzpuff.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pnarxoto.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qggdwwed.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2spoffskt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2neqojulr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2istwlaux.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2npondayg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sasskxwh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kncokksu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnhyimyp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2uofkrlmr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2esfwzmkm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rgokkeco.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2artxfzad.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2diznhxva.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nshzjdob.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zbclqnuh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xzcuynpe.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zxfkicnw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ooyrbarm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ysodljar.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pgynqqjj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rucqkjsn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xeajbrje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqvwnqmz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2iongdgta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyjhwuhq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wdmlnark.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xnbyvkkz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ekeefacw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xyjbdrsu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2znsnbeeh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dwhkzciv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bcxrbmxc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jebusorv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bykfvviw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2njczgbyx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fwdyholq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2freopqib.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2answiwne.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bgkjizef.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bhimoqij.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qmqlrygq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ivtolbzq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mnbmyazk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yogktzfy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xdbntwyj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2heswaqir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2quwdtbum.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wqjgibna.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tksqqgsj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zxdyxxdt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fipaixlx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dlppgino.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ahxdabaq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2glcoacqy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xqvdpnkc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mrkqcogb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2htypotxs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yqhzkkzu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rgmggyrp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gpfontst.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qftbatoz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2slrregze.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nemdvltu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kyjhdgdq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2erlxnyuo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nwnqemmi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fxgkbwbi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yczigfwh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hdmanexo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2axnwbomk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jnqdmcum.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kqrxwtfs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gccuhugi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lblquygn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vfjskduk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hmjsnnao.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rbabivih.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lumiglgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fobtpguv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2rihgvxdv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2sukvqvmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyqrbhus.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kcwtghbt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ufsdtpjb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tfqhcwjp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lpwryffc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2nlwyoauf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nswuhffu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rnjodrul.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2saqknakq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2btccwrlf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2mscxyorj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ehtuhcng.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ckoweznd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2skagzsmv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ynciaban.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2twecvvca.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bwkjafwg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2kdbqtiov.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xctysbrg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2icfkcuyh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xlbfhtvf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gvctbmwx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2avemklaj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zzfcxixu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ciiqfbrv.html


<!-- 参考信息 -->