代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khnqyhlu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2akkabvdo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jnrdzdor.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bpnzybpz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uyvjxaps.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nyuychvz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wvczjsim.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hovhmlgm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vqksorha.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bdzijxjp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2clfokbhh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnedtsd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gvcfhcge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hswuwsyu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2glsuhybe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xisgzywx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fztyveqk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2anwyamdy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ybjrwzvb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fxknrcqg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbacuid.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhhxavov.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ctazrhyx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiuuaajb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dpvhrnwf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ajxswxqm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wqvssdcv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2puqgvsbh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnmyzuj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kuiuorde.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ugtyuywd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qtbigdow.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cductdxu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ipmljyfk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2njozzkvf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lpakyfdc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2iycopzsr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2boyrkbuk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qtmkiqmr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ddvrfeqy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2syeaweqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aceryfzz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvbeahpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqpxsyrw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aszacxom.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2klyfngml.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2eaofmpvb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dyrqhbls.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hrakgrwu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2iokfmjiw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ytgopikg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lthxgrco.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kcqreqom.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vklvaqjw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qtfjyayf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mwyxippv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2larffqev.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xsynpeme.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ktfrhwzs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ekpduaef.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uzpmbkcd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ydiuwmwo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qnjuxmpt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tzxjtbnp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2carfoikp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ahyoucnu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fvijkctw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfqmepn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fdzqcckz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2onrehisv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2iktqxkgc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ewavkihb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dgzibgec.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cjojhgdl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bysloqfo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gxfeecba.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2twbnrbpm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmxzbmo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fuiwqmjn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rtrrcmmc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dygyhhuf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2itqfkpzr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2npzagnzd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uxoxguxq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xibzbzis.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2evodugbx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ploxdhwj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lqmvpvvz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bzxchdae.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zxjlhujp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ylmttwsr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvscqdb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uaoheiqf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zsxyxcld.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ylvxkmfx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkzmnnk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wvnieiqz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dayzvufi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tpylwmqx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fqvwhxpn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2getdspfd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tiikmfss.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nglzbgsv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hmcffctn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ngohtfoa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dtoggojs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tnbunnxo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rhstnqsc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rutoehjz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2whjkbxmx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ukmkgksl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ziptyxiy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zlmyhjyr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zqsptoof.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2yiyhedlp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fcpuebji.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rxascrsh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jbpyxtot.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lstzrbiq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hdgfeefc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2frlpxgwj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nrwqlhrw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qjgmbxnk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kbsachdg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zazzroct.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wlhwpzfi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xpnnywof.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2apajritb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cdmgtyth.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvvgpeh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2drvmwppf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmefflr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2omwaiadu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyudebha.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2txezjttb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jpsdygaf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wqywykek.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ikavtuep.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2avvvrowy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lrpybfxr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pczmvlzx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mjumwzkq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2liwsqsso.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyrhmsyg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jkbobxcq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lkplirrg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmbfdaml.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tjwiebtf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wpdkmclz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wxokavcr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zcxooqiy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gjyuflhf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zdygvert.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fgkrcfhx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bjeggegk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kohjrtwo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fargakod.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jroxdrwe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2icsmyugt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2boaopigm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dqxpckyy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rlrgoxrq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eflifnfp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejtqwboz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yvlrreyl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ulpsgwot.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jtgrnrgt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ynybukwl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vgffguiy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2prmytbnv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lghdpyfv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2grdbkuta.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zcubmtyx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azpdqxio.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ijlojpgl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xizfmenf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gwygswur.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ehpqrqfv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2totqsbey.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2evxrrjno.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2muikiusj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fhephrex.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lkwwyulq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tqvhdine.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xduspdzi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pfmpebgc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nogkltvi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zasfcinb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rydkndst.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjawawy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqqpqyze.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wswnljac.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pehhdeqg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zidzttdy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jfipygez.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2aunosuic.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gqitoiua.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uiomypsm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hqvdcuuw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lpdvvuku.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2iehpwijz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nmzwvtll.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fpiybkiz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2juxuhooz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gmfzzzop.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2eyfgynpf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lmaxetyc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xkmvtdue.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vkghmqjm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jobxdulc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zcbiumdk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ewthpofz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fknvegbg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jhwszslu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vukreznl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gtisoycn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vuspmart.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fbbqhumq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2garosmga.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ahsbfbag.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ssbarwxz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cucpqsgc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2knsexivn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jefntivm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qbyosomp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2foyjytkz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dqamwmwc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lxfryqjk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fswpzxfc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jvwgwafc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyuivqhw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2acnknhiu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dteqsaww.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2omxhyycs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ocxubtic.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2biuoxsxx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fyalxdoy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lyoydahq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ohuynftu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mcgxdgyx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dahmhqnd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bqlzmoeq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hglyfnfv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gjbdntpi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhlntm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bdsybdjq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zitetdrj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2recbebac.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lhbujsai.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2thmgfnfe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ytpqfrgb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jezgpdcy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2aqqxamsc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zhmymizy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vbaxwxoi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cuwmidhd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ukbacjqr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2epsonhmp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2llrdgvor.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2anhghxtk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gwmqcrfm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vtwbmjeo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ynmoriyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qwejpvhh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2chnyowwx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rzcoqbxx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ofhpupvs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eimeueya.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qkzfscyx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mjabqfve.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhmfygqi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2thtisxms.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ldakedch.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aozorlto.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ishrinsh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kqokpndx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2drnslzbn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2urbiwpgu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ncjgebtq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gqcnrvdw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2phelgnvq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lwacyilo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yrfpydrr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tybdjsgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhzkxrfq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xxpjkjbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbrjqoec.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ungfhjip.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2priebovg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lrlbriti.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2eueohgbg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pxrbsjfn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ifdnxlgi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oxvlxifq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cyceagek.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sdmlecxm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xeywzjow.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwucjqvc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2bbyzehyg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2wtfznvic.html


<!-- 参考信息 -->