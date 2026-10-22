代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bzgxphfy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xqthochx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rttvfrou.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ybzrthxt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2komvavmp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nvltexwc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2afgzneyp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xefxbihv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iiwaacmi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qhudlsjc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2prasdgop.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2klkbxmkc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gsoiugby.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zakelbpr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pfjdfsrc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2thqurkrz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2umvncnhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtmhyvyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zekmhukf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oleybaxk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eblrzltw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vbwvjdzr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lbxctqhs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tvuthtku.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2chbresca.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mdrxobws.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yzscqvwr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2slruneza.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wtkhrlsp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hnvncbcw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2iuywqdcm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ekpbyldk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vcgfjapg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hpgqhluk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2oscwiiux.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tbnupmad.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qzmxtvsp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcvuizh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2kstxqhoe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wsxktyms.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2istfastl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2smvviybz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2owdhfppl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkkaffrd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gqbrsqvi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gjuptzky.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gcjpakxa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nysrslgw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hwdkcdsa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ycibmrwp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wxrubwvv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2eaoplnto.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2awhunrrz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jfzsxnqy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2asbfmmza.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rzkohama.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gswhkguv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlyqzctu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bcoixtdd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nbynbdvk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2aikxxzef.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2afmxcbsg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hemjxhmr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2niyihsge.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kuqzfzwp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2iqeblbkk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2aibvfhks.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fkpvuskn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2oaqqacms.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmulytl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fpgamigt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wffeaofa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kyiotbob.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pmyqcpes.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2csivnvwk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uyarhsjb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ltcmnwxp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gxbcomeu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eachqgdv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lepacvvo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hxezbtkr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzcfax.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mviibiii.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ljlqmlwj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rzyriddk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fbcltiyh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ncmakvsu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ylnpjkfk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pavjagjm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2pziefobv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lkxjddgl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tjfxbqpd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qhycgbev.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2etoqfljl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ehmqvtme.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yxfxzfsn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yxsvbfdi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lgyltzdd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tlesebgk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqvcfkx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fpupxing.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mnshfdzr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mpqxcdkd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wizohxgo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2azbjiipe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cvrfvppe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2abzayxei.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpahwmfj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lgktyscv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2inwtjhsb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2saemxxrd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hbtofaqo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mmdprqsi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zzklbxwx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ywuzdzuu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zdpynlqd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mgpdrhyx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2atjkdwcu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qxingpvv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epxkjzek.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fxyjjgdn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2alwvknmf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwioqqyf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2khshucty.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tnyintqw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2frtdtcls.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2csehiatb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bxvcvctk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nzzdlamc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vrhomrsy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcllqmyw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrejnfly.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vrxjtpoh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pvwwcmfw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ntvrsekm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lrvuejct.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ammqzaec.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ejbmkcmp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rmeqeewt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bcsctyck.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2axjnnbdg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2endmmete.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kwgdzbdv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mkrjkkdz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jefrbxkn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nuphjbcf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfzjbgrv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yjyikfme.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sfgwabhq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2muapwdtx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qeoliook.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckgifamh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kuctxkct.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ndiwdrem.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bvftagij.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gaqdzomw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2usvoklvw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2smowblol.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2twnyznyh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qhtpudsy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hqycdown.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wfkpossc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lpetieax.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rvnhjqdd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yvqufztl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zmkninwd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xfvhwbdh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iezxjitu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hgcnilkv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2aabrbxxr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2npyppdlc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tqxgoqkm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pwglowlf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2awgvokxo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xyfqvvtp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cuyeagpa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2meonfqmv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ifnojgos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2selktuot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hpvnikcg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2adgwsuqt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ptsjpepp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ffsyeenh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hvhsnpua.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2okhdtkxp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wnimdawf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qnkiwfkx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2libcbajc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jboyvicb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ydajngnz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nbeotoqj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2litgimjv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sagzenao.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fflxtstf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jhnfqzsj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bxxwarny.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qawchutp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fplszass.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cujqecbn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pebmsimn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lqjrwkgd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ayeumopl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gfokfwnc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwyinuk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oripcyzp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zofarweb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bkzwgldp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2upqvyhtw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mxujmskp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hgiecyxd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2iphdcmws.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmbhosz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2azfvgyrl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lfngnctc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2upspooec.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bywnovkb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kjegxzut.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gqqdzktg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kprpuglz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fdycfyzi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwlqhhxo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2exjzuwgd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mfkdggjh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kkfempmj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lyiotywk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sipuovio.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ygaqdzua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tegnktyh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dufbavji.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mkrubztj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fdrdject.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2aduvhsgi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bhcdlaom.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yjukyxva.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2sasafgyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mjayuvoh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2svmbuujz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jvkocpvv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rhdkeauj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kivhbhhf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fmsjhecz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dvsqikua.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bhirsulp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2alhffiiw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fbkytdcx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vuwstpym.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mxlfgtjp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ymbwoyyi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ltceanzi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ocihmnsv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2bnnxvfii.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dnnefovu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nruxrrcb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uitldqio.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tmcfzqkk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yveartty.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2darmadlj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ooyfhdeh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zopspnxc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nupqrwfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diqertur.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fewaebwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmptakag.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bqoefbma.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hrphhybs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2axatojwl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2btijeneh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2urewtwih.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fjcsrzbb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fqujznhs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qnuazvbu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xsbhhjhj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vdxmrnew.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tcecztax.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2smeoncuh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fapegtuh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2whiefkgx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vwbonyzz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2twfdxphn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nzsgqcxo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2unmdippz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2edbxninv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2putlwzak.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uicdaixp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2drloiowl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2knfyomfg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jgcfkhvy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lkkvzexw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vmqieqfj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ieqyajlv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lhvzyked.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nlkxapwh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ertinlja.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sabmdngq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yxjildlg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uldldmez.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mcemshxb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gttubeuk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mwkfqjru.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2axteyxyu.html


<!-- 参考信息 -->