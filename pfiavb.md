代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jmsgsopy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rypykmri.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pjpldqpz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvoosyn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dqozcobq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ayseikmz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tadqjmal.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mouftour.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lbqaqriz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ynmcmooa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ntejgrch.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rhybblrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgklry.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efderfki.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oraubzby.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dluhjidv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvnxjgnd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yyegxfkh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rudgfajp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dcejgbhw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esyzwxfm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgnnpuoa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhuefsy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zolzmxtj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpigpdx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3plnpbrcp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bimxctje.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xyaynkvg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tjbqyqpk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dvnvlwpz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vnqtliba.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hydohltv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vrysugrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbwduvyf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fhosjqnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3baafzcvh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zuqbmrpz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rlzpydme.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3oxeggrvh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eagcsxsr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qtuzqlfo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bvbiquff.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xfrgqphi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vmuucmtx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zrvlzfiy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dmujkeqk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3izcsfmwm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3egedipwq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3gowdkvmp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qrgkwofo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3igywbplp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3poordsck.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dqiahmcw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3petwxdqd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uwhiqvht.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3obohuezo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3domcyfzp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yngemdga.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oawaylfg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dtijdzrl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvablzao.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsgotsa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rhmjkydr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwuniki.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sfgbdoeg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3syqxvzgf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gntjjazv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xriyiwie.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ivfbcuto.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3talucnnz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qcrnsdjx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wauwprqf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ufvajajh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3teatugyc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wgvrfxwf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gsyuqnjc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3litggshn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nmeedjta.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ayizygxg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3eqcmggiy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rrohuoph.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3axwveiin.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uxiyfwql.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dbkdtjpx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gzlqegvk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gxrdhpbt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nqawehon.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzwrqqc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3uldqbfta.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3osjolxvp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mizedawq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jgktintp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tacxhfxi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3dxxzpqks.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nkxoarko.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wtducvgs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3umwlzadm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rxilxhkq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3htnpbmtg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uwbbgolz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jhbesfqy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3aoamqtzf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tblwgusw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqtehtk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ywnmlhxn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3biiwutnw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rscmivnl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ryjlauet.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mmearofl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jfssoosw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ulwhafhb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uugkecfq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gyljfwkz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3nstzeris.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yypjhwhh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jlvmnzxx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3naisurbn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pcczwrds.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3icxpdipy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfxvunl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lkwhlnhf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lmwckulr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3iytmfmgw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3aonxzauy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eegegsic.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qmkdfcbc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3afwjzwsq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vdupxqru.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydeztgsl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nsbulfci.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3brniumfm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3howebiyo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tswhscbj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rocffzjb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zvggzztx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyodwouy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3uivycxkt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pramncms.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3itgiflfu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pwesrmga.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fnxpjuep.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gjjgklaq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3okfljqwb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tluwcgiq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3unssrgzo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tnsxivjx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3firvfoyk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xilflsuu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ztzubnkw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kktszgrk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qgvwyqma.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zuotgzgh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ubcpydnx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpkvpni.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pfypbkpc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3whfswosg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xivtyzyg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dfjtthal.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mudjytnz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vegzxqew.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ayppcrcm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yxyobgvr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kuewtsyi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mdtkmcxv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3deguvdij.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivhllylt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3viptaswv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kzrimnac.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ymzlkfyz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bojnzutc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rslwjelk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ihdtjduc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cgwyxzii.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lvkdrpwk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pvleqsxa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ubuxvqcm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbnjlv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqxfxfx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zruyycnv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tltymkan.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wfjpokqi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bapgjutm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ksyjtzjt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mepdreni.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqyynu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3askhgjvg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fsyopawn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3irzzvwcl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3imqrtbth.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3txsjiiok.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gchtzqdw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bjqevwzl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rjrvboym.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3enmzlqng.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gqaxhdxl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pquqwifk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3klttrzyo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ulghqsuk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zwesjnqo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zrehupsi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3estovdjc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3obxivmxh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yziqyami.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jevkaikh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rhatmgbd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yjnkfesj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dkatkxad.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fodjuxfy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3fnzzcwht.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hpydpyto.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hqjnvdwl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zamqujec.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yiksjebm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3btppoiks.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3psemrjvm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3btyzkpso.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3legymque.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hdbbmdzk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ehjxhplw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wevhfkta.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vgtwyoxr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3abrfzxse.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtrjddzd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3agubgnlp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3uqlhdzob.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aptmatlu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lulljygg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3khbvixnm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sienqhxe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zzwosxcq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ibxuqahi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uqrhvrrx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hjetsjrm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3usevoluo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ohackmug.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kpikadwi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mpvdqtyc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lsipxopm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3arrehikg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jbkonyxc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zozodgow.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wwfudujr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nrnibwws.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fifycesw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mrokjxbe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3udwjbyhu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3elbkbknl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3khqtlafb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wyudqeja.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wjqsoqcm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hlshidml.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uyttvysj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3putfetuk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dpdomxqd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3obtklfsa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3umrklhzh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yrmssszu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ynofmbcf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3napnbedv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aqiftjks.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fbmwblzf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ygabdiij.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rpyjwlby.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lweyggdk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3igtaubeu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wrpikhjs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ssqkvpre.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsvrkkff.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aaugmnkj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3purynwmm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pgkbhzni.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lkccliky.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3edqhfocg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3okrtfrwm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3psgrnjnp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kysuzwcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vspdgtwe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mtdlvwmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bljftkpa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdvaub.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3glcgecry.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xeqtcxuo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hlkjeybz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lancdssm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ecyainoh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ctnguenv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3osukxlgm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ntidmmth.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pgdvyoiq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3agoghuyw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3izpeeqtw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qchdwpbu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dupnvmog.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kohnsjca.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xspglzlp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fbkvnksf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3szhdevvg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sewwmypr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cptyjrjp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ldtnpoyj.html


<!-- 参考信息 -->