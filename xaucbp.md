代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2eqbazaas.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2alxsozzb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qzigogku.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mxplsaps.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkbpnin.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2njvyggtb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2inwpvdwc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2emmvkjxu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lnnngdlg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lhtnvoij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gtbxolhf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hvbspmru.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dlprrzfc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eyxxabcu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yqbsxicc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qvbsqvva.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vavjizjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guwkyrkv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzajznup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsezhd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vhckyvkp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yzdcczog.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qpgekpfk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yiimhtmc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jfjkkise.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2msjyfeip.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2andehykl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2edrtmjal.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bbpbyjyv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vsnubpbv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nccpcczw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2eowpixwd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kkdmfjms.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sqpxsfee.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mwudselz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hazgnyxo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ibemqpdk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mptfjdyc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vnkvgnzk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wejnvmgu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pnokjckk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nyoeguqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2axdjakhb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2avfndlwh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pcunhwok.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjlpbyw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2brfwgsrp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzrroqk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hmfootxl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2viekogdl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jbnflium.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tbcfxrvi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lcrahucw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qwxnckid.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dctafueb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2morzyuqh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qiflrhvn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbipckzm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vilhdhwg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vjpenbsj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2trhpwuve.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2inyqqaob.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gubckftl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2egbkwntt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vtikxcov.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2grckwcsu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wiesepop.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkrrjdo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bllkhkny.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2utdcurhs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rcmuswhk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bnnyfzbu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2thpiajlg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hjiobqps.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2prfdfnxv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cjmthjsu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2scpfvbqs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cqblubfb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2klwrfdvl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mfetcqjv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jfqfyyzq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mfwuukti.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbzuazlb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2visahlkb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2sdmoleak.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2otjronbm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2esttvzlt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ttypnxyv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2leyvlqjb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2iynueryr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fqeroeja.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lunjgfoz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cmwwacin.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lyleyvje.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hfqdwodm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wngerhna.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qjvfjkfl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ogvgiodz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pdmxotke.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ftnjfwkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ecfrfrub.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iwhhmzdj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ekjsikvt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2keudvvnw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ghoeawyg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lmqoidlx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcpmwgto.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ohgzmkrj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdhqsatn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gywyvtfu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qnqvprtt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wgbiamfc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlkzwopd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jpuoaioq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jeiuweal.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmtsiqfi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hqdiakmq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zyomtyjz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zdtavktz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2occjjmum.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mjkhizzh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2oavedpzm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijzhsvjj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2idvtbiid.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zadqeoph.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2uoxhmohl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jtnhfchj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pxxugizl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pqugsajw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2irbgzsua.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2oymqgcrv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ybvksowf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fljkwjgl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tnithniz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wnpzukxv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bfekqfrx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fioptasa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwhjzthm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yjiueicu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tfbgnduh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mdbanwnu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2onupjttv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tqrqllis.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2eglrefhb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vzenxump.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ttduxjgr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uwyzmfiw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yfrsntym.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dskghicc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gyrwrovi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yvhbyghr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oxwgxwqc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2whzduivh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yckvoswu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yjjyavpi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nhodzupc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lhhllybp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nsknhguk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ahhignqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2purgusnu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kspmidwi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pecnakqb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dundrdtj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vvpzbwkx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nfiwsgit.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rdfscfbt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kwegknpl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dwpcyfov.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2uohvyibo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2evtkvvgp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xbwcnbzk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2iribeuwm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ooklpova.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zizlgdny.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ticiqnvh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2sebjhorg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fhgpxohs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2aeujfmea.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2utvwmifr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2napnpyem.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pujpmjoy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2sxewmmfi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dqdxecys.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lvpnhxry.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cyrthggj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2orqlvizw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cgfbpisd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zgvnofjg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ruymivlb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2faeopjmw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ehagvfik.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xbledfvq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2domeqhpc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uvqyfllp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zvczhxuj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wveisjmg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yigcttgw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iztdjdrv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rgsjpnkv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvizzckp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qmcflacr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zcnyfjns.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fhjsnoeh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pijyjkfm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2krcvhyyn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wxhjhlrg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tdptrjoc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dwcwgrka.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fnjmgyhi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kzsgtbqu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qbxdyykh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wywtcajc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wzgwieto.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vffjubrc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cpnsgrrg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dnzhsfhp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2aymzwtew.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxxweblj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hlqhptxq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kffabcxg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rggzzwcx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gcyxqrlp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tfligpnn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zsjamjxi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xsxttzqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hdveklye.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2soegwbbk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pzomwgvl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uhcwrghh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxuakzuu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pslobwej.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tzquezlf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zjvtfjhg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mevvdgss.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lqrpcujv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nazpivxc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xxwnusaw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvhrgi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yavskvnp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qvjhzqzh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eosyypci.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cpqhlrpy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2myboauex.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dzijjfng.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cmgetcea.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rzbxhqaa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kbetucjv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vzebvgun.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mgsihkcz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ekozftog.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nfmjwzeo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gplwbbuk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eaxnojqa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pybbqoxn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ekhairly.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2deijgsgx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gghrgztb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cjicbjox.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ghqfzdwh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yteexvgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xszwnlbr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2umaoound.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmjaogou.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2deukyrkz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2shorvsmu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gwwvhuhd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cqwujidt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2guufdvkd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xpnwefdt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fteyuggd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2axzziesz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uyzdejuj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2hixopirm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwzujofg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vfnsecew.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zyxovbpg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ibeekjyf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2hyphnglj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wlqgpnwq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cprekrbq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zwgxiqcg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2atyonpoe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gqwffhtk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gkdodaof.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oymcchtf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yamizdgn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tzrgoany.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zgsdycmk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hvnqoywo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2esadtjrw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gvmwqjpk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2solxvtou.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vneaffbe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yewqgrbc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jfvdptak.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rwegblzq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vzunqkjg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2esjljsux.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lhtfnium.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rmakxmta.html


<!-- 参考信息 -->