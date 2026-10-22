代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzinoplu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2axunwevk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2adtxdvgv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kvzkaukc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gbcfkwjs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kdtqgvlt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pzdgmapd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2irkumqwj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uxyvnsrp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2trtjgrbl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fenzmxfv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cerdpgfo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rustsdem.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ysxmpkoz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgjipzxb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zgoibfoi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fnhdowbr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vchloesu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ldtfcckl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2trwoumwo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ihzahftx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hyohgacg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jpebekgs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nybcdlgp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ufwhejqj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ltduuwld.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kbqmapal.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pvcdseyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rioouetd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oevfoqwf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtkhpzw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ovequojm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ltgtglkp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kodcassq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tluiayks.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jwijdxeb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2roqmvalm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2drmdfprf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2udrjjqkm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zcohstog.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmisajk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ombrbpqr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rnejftuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkcsrzww.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2blzrrpdd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qanmfxih.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2borbkujc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lqnbnyhp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zgffcdxo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pmorlxmo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zdkfysyh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fmqchqza.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yoeyqvbr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2haqwlzmb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dpmmiayf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mjgrjjmb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nqcozsvk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2biahvjql.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pwgjdoau.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2atfyhlpn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lsmgzbir.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ueabcdnp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cjhqzgzj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2trethckb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2szzouumh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrrtywp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2trrighol.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ufmlzcdv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hhuqqlem.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pbehviua.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mundyoqe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cjcacgws.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ntbdwsen.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qtmmciyq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bwcnlvpp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yokqqwyi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jhdsqmpf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcimuct.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pnehigdx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iuamwxxn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gawdbqhg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2thmqjpfl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xjtidmsr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhqtkty.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xjzetygu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ckcsiwtp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bxyfhlcx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rmypavvj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qpjnsbdd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zpmffmug.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dinzvydr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qgohglpi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xyjgovwi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bvifvlzz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tgekkytc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnlsztc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kpelmaez.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nfzqpqmg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zlifkqlv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zoofwpfe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cihlxple.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mqddtwjw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rxptobye.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kgvkidyc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cgnfurcy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vmrkcqab.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ytpylmde.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bkjtgmwt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2culkckgt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bxezmgtt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cxkroohr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2admlodcm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2njlgzwct.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2orcqzzir.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2apzjousd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zpkoyuvj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2opfgzjcp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uneyerbi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xntyxkkv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hyknntny.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xzfallpm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xlsdgnwz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2owrvupws.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxmdsfd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yfnpqefn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jzdycgqw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2euxqumuf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pifepgvj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dthkdzbo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oregalau.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2sayqnjkn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdpitody.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iusxrcyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlovnvwd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jttfvwmh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wlruryfq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hczzbbsb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2trxlnxok.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2soxivchl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gwchouzt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2gzbfhais.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uvumkvfx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ddxxtejo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gskywkaw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mewaybep.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wigzgvoc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mtgsnspe.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dthumlzc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qdxihjet.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qryradet.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ztkrqvoj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vrexyixg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2unfblgip.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rylgbhse.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhhxxjyk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jbyvyvwq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nmzkathz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ykefvxui.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2drvhqzyv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvxucwjm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kpbsemrs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dkdwvgxb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bxkutkcq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wfdqrwrt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mlkjlqcs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tccmijcv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vnuyidds.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tfckwdgg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jcldeihs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxnfbma.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2clzypjpn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sxokqaln.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nohspqse.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xttbowul.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2btnjaadl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2eqmvuocs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2usqmbqsy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2iciqztje.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2isjcgbtu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gtrmoznh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wnqkfufj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hdxhyimc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dphwmcjc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2frdmvrvp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yfpapvnn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ubeotydd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rahlqgov.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jnjjkiai.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2flitxuls.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mitusxxj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ixpohzzx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ltdbubqy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pvukzjsu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nkorqqjr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2sasdlsww.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vojyzkzm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zlskmkag.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zmqcexuu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2civrjupa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2iucoancm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qlzuwhns.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2byfmiiaf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lwbcetcd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mceestfl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2slffgxqa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gusyyrus.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vqmatqym.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jzowozzq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gxfsupaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fetpcfrb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qlvqpbkv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tgqdjcom.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ozjsdgta.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2uaazjfiv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tebtdjlr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2psvuclkz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gcjgjthf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mzaoexkq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rgfbphlp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dqaktusk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ovqfkrir.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nlllwdfn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2prxdgseg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2undkpznq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2aokrfpey.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lggucfsb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lglfklap.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmuoknyy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2iubiifmc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vegfmjrq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fvhfvdql.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uejnrbjy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hbtmmuca.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fmwjgjmd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ynayobnk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2prddrkpg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hfbilqzz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjrfkrve.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wmoradpq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xgzmsrgi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2scnxsjyc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zhktluxm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vxxiyphe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zbvvrmgs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2bmuhbzgd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2toimusgb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bvanozln.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fdrtnxze.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vjapabqr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2plhycvcd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bciyznbf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jsqtqtbk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2anjhgftb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cueinbeh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ksnucwwu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2seqlcibb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nbfgyqrm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gfkaaryy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2noreixao.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tisoetid.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2folcbluj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bfksnkqe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yyqkuzyo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iorfozqg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xflbnelv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2uvlqstdx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ojqjgeoy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2csnqbtib.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xcpxbgij.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2smbmkfbx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yxuhhzsz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zjqdggne.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gjzbyrsf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxtaky.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rtqbkidv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enkvkncw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ymnncaoa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2upzlltot.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zwozmpks.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jytyzruu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ctgxkvje.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oclcbqxw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sbzqsasu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dkymdqkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2virxheln.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ddhguczz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpmkgxep.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kcucbjor.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ukadllys.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gmzfgirm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tyomadpl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2szwarzxa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qtolxcfl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dldkagha.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yasdbueo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lwbvvxkz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tpswewsq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xdvwhnlx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jvetqeyb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jgvwuaxn.html


<!-- 参考信息 -->