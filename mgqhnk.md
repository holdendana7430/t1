代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mseifnrm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhtiqxgo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzfbiqlu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vnhbotsp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsvgocga.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gsnucvjt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nduxeebb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gehlkadi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehmlwomv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hpzyzavb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eaupcial.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yidxzbqb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vwvywqxk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ypjzzbms.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jnejhhst.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ztpahqya.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2piljhyhb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nykwlrmu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uardapxi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dbzengnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mbtaxyxi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sdnxwimq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mspqrzgf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ldbqyyac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kptpoyql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgwhkfht.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kyqjhgne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbjufkgi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qawtctet.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ryhehiqq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yybqnlaa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wvqklkvc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fjezatsz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2loisglms.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jwrqmqef.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2djobcndb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jqxzzjkg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cvfozhgl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uywyehwb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fjwivjqc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bxhowucu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2thxixcpe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cbwnikrc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hokoroji.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2aarppgqo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qljaepdh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2odlhgxkh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ygwcspax.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfhbza.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2eanqwewv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qormvcto.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rftuvszf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xtxtuzaj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkutzei.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2isodfxbq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpptqhv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2necjoyae.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zqnnfglj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2egvrnrje.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ynofenis.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hqsthhux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2muggfojo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cuaktpbd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqckuan.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hlrdepds.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xfrzjqwa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jcgpuksu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qxehqwed.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ysmmrasr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vjfuklbi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cscdkrif.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vrjgsnpq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mdlhdhuw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mwjdysbd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ksznfqcv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gozlrtcx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mpaoxjqg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rjtornii.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2aqnywkoz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2aoyrwvhv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2drcdgrld.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2iwndydsh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qllunqae.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2godpvite.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2erhbqgfl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2deysmdfj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2goqwvdoz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwhfovf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ktgtzrhf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2yqazgmov.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dmjztmcj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jvenwdbr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vzvuxcod.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wjunfcmu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2huyvkixz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2iqhuaxnm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hpnxtzvz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnoflgc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ssbjdkdr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdcniay.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vbdwoeeu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kkcwcdcx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2sqfmfrvk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2egusxzxw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mcfesidu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2scybydmu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vlvardne.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mhbqtzet.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pumygtlf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ycwmawsk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cepqdfrt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2poousxyz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uopxumvi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hwtjsixr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kcgsatan.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2esdhgbex.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpmkexmt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2poqfhiax.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jynrxsjw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2neimivne.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sozuezmf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nyfnnecc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tqrlyprq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wehwfitj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2iknmpods.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xhtjcbys.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qkawbgca.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ivakazzj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ekkmpzvu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uffxtdvi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ljpwnasl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2atnjbauk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jhyujddm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ohugrpdi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hmhgfjoc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vnqfdgyk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2taoikumg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ynplrgvx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjutamxi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrrpdqtt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fmrchpdk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2exuymtdr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yoqbxndv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbdqye.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuazmukn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2baolxmij.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2uqtpcpzb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zutpsklp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xfvnnitv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cchjlusc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2evipitkb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zzqmnxju.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hzbqwugg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vbvjmvjt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ziubdpuh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2emahjrnc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2drsplciz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tpyfhsmb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wtipqhvq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2behhmbtl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ncszcucv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mozhlctg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qecdoppc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mnotjrbp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qoxtkdiv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yarnheug.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mlwlrlfj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2axbqcypf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2osjlmytm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqghkt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bpdbaeqp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2klzloiho.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2coeggrlf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dhgnqjvm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2arizxgfz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hbxryehy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2skqotmqk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2okmlnrvh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pmwkayan.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zxhnfncq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hotmhaxz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zxpphwnv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2usqangdj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pnehokoa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2veqdkujk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2omjammhy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2laytnvtm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cpkkjmov.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uergmwwz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2yjrptdvw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ymlnsqur.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2gsmmnuwk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2emyyrims.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ruzyzgpm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wsmwxdlo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mtuksqrx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2eyyenbcg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dztrxznn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2esrrweut.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pumwhezt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wmylxaql.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nfvhtrbe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mbejyqwc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lnjximqr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkdmdxpz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2docpiotj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hbdmsjai.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xdssfjlt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pjqowkeu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xpqplmao.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ujinzcwl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dtmigbxo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gjprobbr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jwhkefov.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sbkudafa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ekdnwsnq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lawaxqmp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jjcjazmx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kozmndcd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmmtvoj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cgpvfwpc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mgsbsoxi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xyzbonuf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hvnlmufl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lcuithfs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vurduvnv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cizxfpbv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2soetsnve.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bhbldgmz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgdoqha.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2isfqhtol.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ywxopiwh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ymyvghzo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ctbgooyp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ptsihavl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lfzglvgm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qmumumvc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xrapohov.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2smbcmhfx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2netkiluy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jpoyayhj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gkmfuqff.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmcaqb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pkteurnc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qpbcfpuc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2doaywkqr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mycakpfd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ryqatfzy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2shhfraud.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dutjxvns.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2worthejc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lbfjuroa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2sdruoccs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xnzoussb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2varitdsp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ykwmdwuo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wcsorkcv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kgljyxye.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2klovsafg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efnwwdhr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gygbqxqp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2idmeglye.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tysgbujl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gbwkypac.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2egrajclp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2epkbjhzy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zwwriiyk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2portfapn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trfsqefd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2utvxcmin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvibcgva.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ptekzpca.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2safaymef.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zvqseohg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2otfyqiej.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lzthywtk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2huutelzc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fekucese.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zknbyfbp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sdutnvsm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2epnstkzi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ozwfdzhh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hogmxljt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ouievrdk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wuvhwcow.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dpgylreu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sebxpvoy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bgtzlldo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fnjorpur.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oaqkmubx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mvffgbft.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cxrnkqxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2brnmssrn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vobbvpvt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2agkxjvhy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vjljcvke.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jtrtplcs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fuzmvjpy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uhzapkai.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bgehyqaz.html


<!-- 参考信息 -->