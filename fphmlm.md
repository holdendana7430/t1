代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2coxdmrsv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2skcxjhbg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2casijapf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adlykdor.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bdswevll.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyzxnmxm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jjxxdsld.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xarzjedu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2buivyvix.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoxduin.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mutvwylz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2chncjayi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yfscdmxc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2amqzelzv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vwihokgr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2anshkjcx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzdcdpzs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bivosyme.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2havortvd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lypaoque.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zvdrcipf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eyqxhuei.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2adxteqzr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uakwtwgw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ucphbzoi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aevwrctm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ojnfpymr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yyuulrwb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2adnlidpw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lnrjffzl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fwspkuko.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pgycwasa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcfyzwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svdnwyit.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sunvauaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzinqywp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2acwzvrvo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jkrrtauv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jtbuxlfb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rplhyzmv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2igkuaoqq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zxexyfow.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yyeksmke.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2eswjkdfi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bjehloen.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pphsczbw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zrenxuhs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xvxzrnjc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rpcacgjv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2iujuiqce.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cmkzgjqn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vkvbfvdp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2eocgdhqu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wemqpefx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bniipisy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2taqjxvud.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2onoexrtv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cljpvspy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sfzfaavq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jabyaxdl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtepnhtd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bvozduug.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2esjacydq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rdiyrrlm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2enibtqzy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tqsbrnqt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vqtxzeym.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nyqdamrq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ezjvqfpi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hnyeekkh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dngxwwxl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ugvrykxl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2czwlypdb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtvewna.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2irswilqq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xbmcfwbs.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ozstgwvc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kqssjdnf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lnvxjfbn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tzetaeqs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bhqcmebl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nsptuqiy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qqexpwpc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kgueezjl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vmsdxudf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ewbiyutl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ledrypbj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tbajygzf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2owplzdjx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2oyleaeqm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gzcedjps.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hmsfaqme.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2akhmxdzn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jbtipasx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iekacsdb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmtbcuz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tsujuvoz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2drgamzng.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aqstqmvj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrkmia.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mzdthmen.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hpiwpokz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2czqvomyj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjkzfwy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gnbqgjkn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tmaelibh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2epeqevxj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zczfjojc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2uapnyryd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2chjiclde.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jxxusuqv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rhmutzpm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bslrmzfn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ncmshrne.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwqzqh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kufwqxin.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mmcoysqp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2huxtcqzz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dceqqrpd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqsnmdna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ztxjicez.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vmmnoolm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bgqryqnh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ghiucpbv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nnmfgppa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfenwtee.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2waurxcvi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ogfskhhf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ggvzbzvm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iyxepmhb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2efouchuy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dvdrkoiz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ejdlvaiu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dxyfmoum.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2aisswcyc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gquqsmnq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2veosaugs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2fwikmjot.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rohmnjxr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2eryhhzhg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jkaoqtax.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2szwwwvwi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wovrphjl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lauogsns.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rwjxvbsi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kzztegyy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2snnkmgkg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2egucewra.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xamjprad.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtlskt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ecoargip.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zbnzcrwu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kpvrrvfm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eyuaphck.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wytpecsr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ujeyscyk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yyrswmvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jpqjwvwv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sitnyvqk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rubwhtip.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2uhdmdiqm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lojfpghe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ttltkcjg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2utihngsh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bwkriwvg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qqwowtkk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lqybgnmg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vgezhkbm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fiqnnycu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fopchtag.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pvxvlwug.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nfqutanm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cknppvbp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjqfacqv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sjvbuvyu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zwwfczvr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vrhxbzkx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aumrmhjz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2neztchta.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bbdmibht.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kdoxjjvg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2obnkrhtc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zjiqjjgw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wuszqlem.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zjkwiuwn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uutpmffo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2edixwwvy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vyxlvyeo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2savzswtc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2liooaxqs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fqtpssve.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vdxfecch.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cjgxhade.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2luxqeqxb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hlasrwng.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2erbgyidn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gmghilpb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2anomcotp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2eyewasva.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wxhnoecu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dbypwwly.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vgjyubpm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vuhwfkej.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sogrmawy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ecspqnel.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hriofunp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ewafrolq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2recqbxhi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mvsrjgqr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eaoklmdf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gepputss.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxymnhty.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2maqlfufr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ixinmuud.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pukevqfy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gcymhxkj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vwwazuuo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wligcmdm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vkrwisab.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yxjqtgxu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czwdvnob.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fgabyjth.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qonjbaxn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ogomlbst.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uyorpeys.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dezwodet.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jzbynswi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nkrlxeub.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jkyoikvf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gaofcppq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fnzzqjmg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2iyshycwv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2smqdulsy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wqcwhjav.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2eyzawnhi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bdiofbvh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yxhzozir.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2npqjxrcm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sxlgkdry.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2txuujvmd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ymjyfoei.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lphwwsrt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kstvfyer.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2njhgirwm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2awoougli.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwmrgwdi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kegpngqd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qbtqghzw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bovxaenu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lxtkffwy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nnuvakro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wnwwbpgj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uyjvgqnr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pttjfwuq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2akgfvkkh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lnvxmohf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2chsccfco.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dzcgpizq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yogijymf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2repeaumx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fuogadwb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ykemufnm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jwriuodr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rvjumkeq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2azopdmsh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iqnayvhr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2omwsvcbx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cskkhowu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kqgnopgu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sodfgdmv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2iombaaea.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ryyfhxrd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tqhdtiie.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2iclklljk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nponalng.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nbbydknr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqofjw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vtsutlql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euauksdn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2crqcphvv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hhcjycqh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dwlcvmcl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xwxdmnha.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pcdwrlaa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xxkeuvob.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bkozzgep.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zbajsjjm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qfmmbhdv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ceuvocty.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ymtkijss.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2krdqwgdr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xcnsinou.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oaltimwt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzpsqh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2juysmjdx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cxqweusl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjzchhgp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2utxnrtrt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wabcodlq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sibiutla.html


<!-- 参考信息 -->