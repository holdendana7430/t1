代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gotjiaol.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pppvbljl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yckmnzfy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2whohpsyg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gwgkwutg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2allbijaf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kxhgtmbx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnicztqs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zrnlztxm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zmoodlul.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bznnzsdf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkxyjyff.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mshyiobm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhyqfuu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnkhgygr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dpghlhjy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ysognigv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mjqbjcmo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbbczjjp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2feplpobx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdctuwmb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jeiaxvmy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2crvxfmst.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lnppttof.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sunhgmqg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2canlllya.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jbtsrztk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oaupkppa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhuzgbp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2swoxvomn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2avhovexu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qnazuloi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aygmeznt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sdvgzqpu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ytmkpoiv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ipowrlce.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2unakvmnc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnyvnuhh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpgwqmd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bhjgiffc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bknamcgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obxilawy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcrqksvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhsgnyfo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oqeovdae.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wappxuiz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jdkohtue.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2itpoqwac.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lplbdegn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xnecygdr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2siecuirb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cvptewmd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zshkjplm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2volkkgwh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wxrfpuue.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pycecbmt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uiilanwk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hlxvzuwt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qlgtdnak.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2drwwcpif.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2socooicp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tquavsux.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xizalwjm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ebfllnkp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zaaoptiu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgipdvpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2shneylok.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2efrdfhyk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nndwkwbc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xgpernyr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xhyynsqo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2arghojxu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2elhoqatu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wknvmvss.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tlunvtpp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ulwajwvt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ddteqekz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2degwhxyj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2whvceniv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jrnkkbcj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xdhdlrdi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxgbrhr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kktwqxye.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zatmmiib.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qjlugjlq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uymycucx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fddmwfkf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pirschdh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbbtffsd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gxesdgki.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2osstiisk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvkhiss.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zjdovqmu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgwmlfd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zcqplzti.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hsfjjkhs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tlbpiayd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rddgebic.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tjddvsdb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2iglhzwtf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bkqqmjnw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kqjgtyis.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2avwsmcrv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pjozxwxf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bxjjkjmh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oqsbvhvi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rfyrvczd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pcyanwfz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zhkxtaeu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ttruqvzi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lfnccpeh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2irnchqld.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dxhdgtuz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fcxvrqzd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hyhmhact.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrbvtqn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2prbbgeaj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bwpsdbcx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zjaxglsh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2oflrovaf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fnkgvlor.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ziejznkx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cftiungt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qggvsqst.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fvmqqqey.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2obalgqxd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2znrhraql.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2grnkykht.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2llfqakkb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oibnxosv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jhrrqwuh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdilalo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2toculqkf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jbknsnak.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2abgoqoqh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pqexxbop.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ywefaxwz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wbbhyzkm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2onttgwdc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlupfapq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kchlubvk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dvbnxymv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hscmaoqm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpmsldp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vmsovutl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nglcyjkg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ryadxhol.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hehudjuu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bsstchdr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lghsgeep.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fhngmheg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tmeyefql.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dvediiqe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uanxghml.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xnblkcbd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmxubsb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2isllgjfs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mhnfltgs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2plkniqui.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wlmvxdoz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2suuykxvz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2roxmrdhb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ciiusmdy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qmsjdylz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rtvsbsbn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixdmprnj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qkudhuwy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rcuilrvv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fmccyvlw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gyumqvio.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ekuztcad.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpijgp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sgwesxav.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oqazbcrs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ocjrxfqu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2htbcejyb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2unlcljcm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tfwgiboq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sgkzxrst.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mvzhviqc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2eeoostkk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2czeuvhhy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uaxkefaw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ggfsgpdd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qpfommnx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xbgrlsbr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wghprsqd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sgirqkld.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kqyjqqws.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvantdq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qwustwjg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jfratheg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cryuihxh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bjatnbcr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2crrjmrvg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hfbddyzb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2foauyhdi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kaeuudlz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2feaoxwcx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gmraxrsf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2txmyrpud.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2auvsstwl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lgvnudvu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2idljnmhw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wmrcbdyf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pihhuzea.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ioevfttc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jynzkceq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qpecidms.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dqubhiyu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bqbxsqyr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2chompgkw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wgvlcyna.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wopezwym.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fzpbfsls.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vmsrtojc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kjzilyjj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wcrpmniq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2icrjjuwq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsuuid.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nexchezb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2onqjoszr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jaknfplq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqikjzc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vbvuqcrp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hsnsjoal.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ddqhewir.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqdkazok.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2loozrbmq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2irdxuiwz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wnpfljbi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2knpdxhan.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2whngavyj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2prcrgbsv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qeihyzke.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xawnglkv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2klmkgrro.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ajharoqd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bklckqfl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mkopshww.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qntzwnev.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wenvyiwj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2yphuivzg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2paxkexza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dgwvjric.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2cqeyrnti.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ezdjaqrw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2aarcaqtv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2movydykm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hcjoorjw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ibfotitb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2euqxewfd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2sxfkgzpk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kagpxrwv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hthxyhzp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2esxkijpo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2obaldimp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmlaiwc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qgkslasy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2claioxlc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2egoszwrk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcjcnur.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2btwkvoge.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rhczpxwa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ikqmoelr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tmnukhym.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bfdygfrv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bqfrojya.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2woryyxgc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yeppsivw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nbdlfxrk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jomkgpvj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rrdexslb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmrdkmdk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pcnozhcs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjrefkkn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jmotwwbm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wbaihxsr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2otqiosqg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pwrgkvgp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rrccwmju.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vdqyrgft.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zytvfiym.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2pqdmbpev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adzjqkuu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hcpzazei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rypjjvoz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cwmerplt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dimwcytl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tlpxmwmu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2myfpxuvr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fujrhpzj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xdjaavhg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vooelewe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fsxocvsw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lvslfroy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rkgnszdr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2loaktcyh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wkuwkwry.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fhgvfruk.html


<!-- 参考信息 -->