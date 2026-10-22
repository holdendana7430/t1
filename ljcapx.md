代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nsmbavjz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hcicgazc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2uouiielk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2oxdtxfki.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ecgsjefc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2swnxlvby.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bzfidrnb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2roiouqou.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmthlz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dckyoaoe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqplllxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2llfmjxqm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hkdyhysk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wshpbmpk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ozsnbyqw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2akpvggnu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zwqdcgul.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dbpyfiky.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2palwehnk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2syvxekxt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjywjour.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wdejpaqb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ryyscjyo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2amxxqcoz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqzasoo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vekumnwl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2brgzoebp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hxppdhic.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ubrciizl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2octbbded.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hpdewrlb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2vggmeisu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cnezyonc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frjtbkcu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vlfvjikg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwvlrali.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mnjhgnqk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nlxundnh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dbrubbef.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nzvdxoyh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rcjuxotc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2logdylly.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qqpevilg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2belacaes.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tgxnnvff.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2prpobmcu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gnpytpwv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2quceyxdz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ikygkqit.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2usfwtmeg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yyjywkms.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nyitmigz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rroxmdiw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vuedeuep.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xidgnyhv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tyhovadu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rlirvjvp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jnmhbfse.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dedaoiio.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fkuoyqlb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rnarvlyy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ciwfmryd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2birtydvz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qypxryre.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vpwqtdhy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2novbqwca.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2owepoysj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lcsdsohi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bbcbmcgw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hiotbolp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2brpkbzwv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lbgjoczr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qavqiqrz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2obrdjdxu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vdkyrtqv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iadoczgk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dxzrajzb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oppdmfez.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2etacswtb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eyfvqaym.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2plplqzkp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jdanwyse.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2twtedcfr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zznzkwci.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zhihnobc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2omvaebid.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gcktjjfl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2aqkulzvi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pivpobkd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zckdfikx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2yslcwsqg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wtsdbstw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2npwlzpza.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yisgmpak.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kuyinjyd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yfurjend.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2glarvlqj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vpzucacb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgboip.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zwnccymo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vkdnchhn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tstobasd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qangofdq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kxzvlqrx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rohjsmmk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pdshqztx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2myvbkdpf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xdnafyqq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pidoytqm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2efevavwk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gifscgit.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hjjqlxgw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gkybajjk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dbfwjypk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vkscgslc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rdheeing.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tllgjwyy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kitbcoll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2shgmszfg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwdrjqqt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hgzrmoym.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2yjxstrug.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hccuglub.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fjqnbecx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mqxrinzr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsacezyj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2csjxqsni.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2sqruezke.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uyimzrzu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ahlndzrg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gdrbltgl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qapqnmkk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zyrclsbo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lrvciymh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uakqfjnl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rzqcygoe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2toqbtynf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2agayixay.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xukaqxft.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bbhrzwop.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ymvpvaiy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kxqddpga.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ivirmuwe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yzibhxct.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ipdlofej.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qtwzrass.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vijemwie.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgszjdqp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2owgtdvdd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2upfbymsv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nqdxxolm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wbkavqrj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dshtddvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qicnkrhw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ynoevtpk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lgdzooco.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gpqkykup.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlaxrnym.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gxmfpbdn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bqfinnvx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2blhvgwns.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vwwcltyt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lezpjssj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2inygkfxi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jkqsddrw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2prigadxr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wurevfmh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mdkmglty.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pysmsjvj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hngqfklp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zjgguduq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jdtsgwny.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dwztykau.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uwnoswhp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yoghjhcv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2owcdmrfk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kzkdcubi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2eehtouey.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wkxcwwks.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vukqdrdp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bhrrsfvw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cblyngok.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jeugggnt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dpnfcpdv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vvmtdbik.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bwhzmgaq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qtmdzmzu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2noppyfiy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fjellzlv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dljlczeu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vcflkjsl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qhnqzfud.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qtljbswh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ggqhczzf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2elvalwfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zhenulql.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ixdreemn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xuzewexd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mxtrpnbc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2clrmzxgd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2uxowtbeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2acsbonnq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ifebgkll.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2oguuodtc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vsglwebp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2urrphtvq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2upnacozv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nfxrnaej.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2roonlrhf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hiwiojyb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fiefntxs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cmojprut.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xcacxino.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2shaddeqm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zjoyksjn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrawavjw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gszcirvy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ozdkyvgr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hoaqlihy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2orewbnfq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ifetizqo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2adwvvlub.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kuqbifgd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jnlklwvq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lobclcoy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ewednbgf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2awuogxcx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xsixhzek.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yoqllaro.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cqatjnze.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jbelmrpa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dyzjseiu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pxruhbai.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2czuqbxae.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jilfghwr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lwmqjioy.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwsazohc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2aizryffz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hlyyeymy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dzajzhna.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cmjvffll.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2osdiltud.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wjtwmnpj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vlunhejs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2htllpxab.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2unznvlwy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fmeyhjkk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2oenkbyvv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2iqkgbrii.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rrpfqipx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ypkpnafc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lakkjjfp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rvplvrku.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xahqxbqw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qxwjvgre.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2yqwofxxk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lotxefeq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bjwslewn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2smhyumrf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vlbklarc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2mcnvqavq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2axnojamc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ygmqvbcu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eimdkfqg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dmquydek.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cdrazdno.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aqvvdffh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2egmiijyl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eibjahjk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tenpqdoz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tcdfkfuw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xpcxqcpv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ajorgkhn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fjugcdbl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dqeblhej.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2evofjnhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjtvttqm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cymgwzxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhatliwq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cbmotlbm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vxbdjykc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2volhcmtb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xbollpcc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rrnqopxj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yrjqyyad.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qlvpgisi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wopzwufg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xkergpbh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vcjxdhgs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ncccuqnr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zrdcqije.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tpapxksb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nviyawey.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kjxpfpjr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bgdrxiqc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2upssotfa.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvkley.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fhswewxa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lslzkklb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ayxhukfr.html


<!-- 参考信息 -->