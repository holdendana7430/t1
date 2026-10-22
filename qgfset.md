代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ickswmyk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wksrfryg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uhygmvtw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ffpcdqpr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pqroawkg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ysffgzqt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nwxywalj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mzmgmwlm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lecmnmdu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xefedexg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pfouqtng.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2obtmgarx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2repjohte.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wketjplu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2slcshlec.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wwldludo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvfpfwbx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kntvjwrl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2arimpico.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2agtxyayv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uklltbdf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2keinfafu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dervobzt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zkkwpvud.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vkujrelw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mhcjnxlo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ratbubqi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lnkknicm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2drzjxqeh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2pblcbrcf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nbmvohrm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tzgcivzk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2duxmrxpv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ugiqomei.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2phhnzxks.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2sdmpxypa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bcqrxase.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hykytrjp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kgswjlco.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2txrjqkhz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2maqhxshs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzzaqqu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pizzadnj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qwbruxla.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2uttqpdcp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2otnmisyz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdtwvagl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hqzdonsd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yxbuqjqk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qooshqer.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hehazjlb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2raimvszc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wlsdolpf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uooowepn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fvvcfhhp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2oxmnxxir.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xhgmwapc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ohlagiao.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rkhsjwmb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2htwlcynw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rmksvkhy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jepgcmyi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tmlzwuzc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eodieepo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldmfwsrx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2llprjmug.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rjywmmfx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2anhvjtlv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cvrwiizh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2sazvydse.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gcsivlgh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yxddeief.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ssqvyevm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2igttghbu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhaiunxl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mwjcngvg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bgmprjkd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2srohjyud.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zejgqsoz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gbtcnsme.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ghedtdii.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gzhniovq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xyobrvkx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cswgumou.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kmrtwwnh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yubcctbm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2cvjkhfek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ijwuaqov.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwammurh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ihpzuqtj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vmjgmkeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kdmkrrpo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tuydrmtu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhgzvzqr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ftkwougv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zxriimax.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qayhrzob.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2voheghtd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mzxactov.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xpncemub.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fycbtmpt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tflvklmt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2aupaovlk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yphpbqxb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nkfqvyjk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gobxxtqp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ihbiryfo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2drhjuirw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gyttrjzg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jhpupwia.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2udsafydx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2iauznejp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kgjyzyta.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tacwuqmy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2avaagkfo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dgwyulyr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2akbshsuw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jhnrcgup.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fsnhzkwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fhokzqft.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gzapeltl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tefiujru.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wpesuzuk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dbnirdqv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2doaimdpx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lzlkumyc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fjhufkfb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dkqgcvft.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tgmpoykd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xtomcpmb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2farkjpqu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2djqhyttc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fipnzump.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mtpojbms.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xyrhbiqx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfrbvyd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qjtvhray.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mybtjfdj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qimiltfu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2loyjvhev.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uzdlobls.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pinakrnp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fswigfkz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pqirvbvl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nifsoknj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kishkzgn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kbltmdeb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pmbihofs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dvvoqrhh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aiggeglg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vwwevnqx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qlfndedh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jlfoojcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2iwfzzlsi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fwaewfzx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2olsvjtph.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2guzjldia.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lyhwecgn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2foovpbhg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zfjhifud.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2divotyzc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jcwywrqv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pymphbtk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kqywvnhl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gqsdzkkf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bdylmtfi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2culwrsxw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lvgynlhh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dvbnbleh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zsnilfzl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijrvjaqs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wnfqmyif.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ougdmwnj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ftggwmvj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uxmgibrd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tfzcueeg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uygqirun.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qltyclia.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pvfbshcg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pvwitmvo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kzadwybw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2izrruhsy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2isdggrgx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pjfjvwea.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hvuefjpy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qiopdccv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mthpolwv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fqydqopl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rrtcjeld.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jfbcjzra.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2prybvbsm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2aanagccb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dvkrhqbv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iavcpgqq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2goqjhloz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pquhffrf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dgvacwus.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mrtrpewt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ysijoedk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kxryxglo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tnnwkkom.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jhnxzqqu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jtozkahb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zkfujzfi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wcayoxhh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wlrxybas.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pijggbwy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2eswtvrkd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gcrkzbgp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tyqbtfwn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jmvavoda.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2flkbxjtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gopxxdcc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2udfruvuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqvjjwut.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wixammfn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vfbiqtme.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uhyxfwyj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hmeeyhhw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2brqzyoeo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbokzl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2blvsoaoh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2groxeiuo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lwwektyc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2awhtslki.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2oxxtqafb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2encibwoc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rsfvtoey.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lkwzikyn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zmjlsrak.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wgcmrxva.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fjxgqnqb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hbpjugyu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ifogerhj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2aqjuiprc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hvalxlac.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2amsgxebx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mlbeivmy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jrmoqlcs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ucscendb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qibpoduf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qahfrswm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2axnryxvs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2eznvvqho.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lzpfufvt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bxxgfzha.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2berkucbb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qgpkqnce.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qfzxyfmz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iirzdopw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fjakahyf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dpmkknyv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zwcxejho.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2onkrmctl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xtcoeeuz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rktywusx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fcumvewd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhdlmqdw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vtssindb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hxzbwnsk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bsfygbqp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pomqwxhs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eyxmbfgh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hywqubry.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dyrrpbep.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ekufkvkr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dymboffo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tubbzvce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dszqzjgj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ifsnfpon.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vfihbuxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2janhulqd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2mquvznvd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lbehugkc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nbclqmqw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2casoergd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hcuqrbwk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2xxbbppua.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2idizmfcq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2abhtbmqj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2yikkdyja.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lviymbqm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nvbgdeiy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2hcbawsub.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2lazzihvb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2pprjkcmr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2nirrcrzj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2uodhfnog.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2odtfzgcw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2azkvynvx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dvoalmal.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2weclnair.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2addhraxs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tndeiteh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gzemfhyr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ihhwbiiw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2swbtmrxu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vcglnnhd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jibsnvqu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bhnnmokf.html


<!-- 参考信息 -->