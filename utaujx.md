代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3etzufdcl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vqxnello.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtxognfo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fzbeeoky.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jopejqsj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3weiuajas.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qmymjewm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gjyhhccv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yvaweucb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3biyfbvlw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mzuggwcp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xvqerfoh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rbkhtsyp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eexfvyom.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dyrhbaxl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zstvkowz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3elbjmybs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yiedjbzo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaizhrel.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nqpixtzv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmopbwh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flvomeph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zecdhixa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fctmzqrn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3swkghtcj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqcfaohs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jpnoqsrk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pdiixhhg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsdpddeo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjlxfpwi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3locbwnms.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vytifrpv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ylnqsnnk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zjdoedgq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3chcrlade.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qpololgw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jwmjtvqt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xapuggfm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3riuuetim.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ovkahuna.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wmwanwre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fabonntb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcgtmabi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrxjaiqk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gkjvlwtd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uzwjylcy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zsladbtn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lwwironi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tuulfghh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dujckagq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3swetpogw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3grlsvrbo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3thqaxwvc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3taxnogmv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ksshouga.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qmzmsddx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bbapwbjm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bijctwnr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bfbygrkb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ndfggaef.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gnndoxgl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkfmxty.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vriqpbir.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3neaienyn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3eddvgilc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsqyyea.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sfbgmcsr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zwuvgnzh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xmsmecqy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jzjlclxu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eksuvdhu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3icrbxhca.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mhzfzpdf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fhkmyvww.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3trzsggrg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3awwpvvxz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ujpdjwdc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoyesog.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hiiafvwn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jlqedwlr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sdmkgkme.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pyrwhorr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aelncpdf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3iaowwior.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ivxsqfdk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ajkudrjz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3trgiqfwr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jyujqkxy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xuvyylmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mmjpldnj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bcpoibfw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3umaqtgsm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tfchbiep.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bjxqjyvf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zblwcavm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3somyeobu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3iyvnlcav.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3maylmaif.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cuygrtde.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jkcbwivo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3emvlrtjk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3idwyvjcq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mwyjhfoi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3edfssnsp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3updabseu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rjfclyvd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tqwvpohz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lzgzdtdm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3urachmli.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nzxbkqal.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gsljgtjm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ceoahlop.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jkakbtuv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kgtddrdp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhegrr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vtayegoy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3drmymvxv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xfaoicck.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yutomjtj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kueokcam.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rzilylmb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3caqtqsjy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wzdjlydf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ategtjfy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3epjvnwfz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vojsdygh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tpvrziem.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mtsbyuwb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gdwktxca.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3inyaqocr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3swmjdukb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3suwkrhsa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sokdvfck.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3adfasovl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cxkrfsli.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hjujcuay.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gcbfanlc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fonczuwa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wbfsldqu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mxeafmhc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3epfbokxp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3viwhdfye.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yorptwdb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rpnfidls.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwhyey.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ffzritdv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hkqzghqf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hagxvepo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bxvltlzy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pfjmkgly.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3utzdzdwf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3aphmbjwr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lmblrgtc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3elrwfrol.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzlctjze.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpukarf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sdaaceta.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdvurwlj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wjmjeabd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gmiwsqle.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3sipgutvl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3shakqbtd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3oxnxxily.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3waadmbpo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vhrdwvtc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvbpfevi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kemisqmh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3liiiaaqf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xhcbirqw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqbfgej.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqmpnd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wlrduhaf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uhmprlsu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ndnjojem.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mkmwngdz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3avsczthn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tsrbxgtg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bpjbzkeu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nmxjsvgw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lvfmmmkw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bcaglocs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wzsiloyz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iehlzetb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3pnppjgcq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uwlbqazl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wgaumeuo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ogfcdmav.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ftuacesm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3czaqzevo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3uqmmmncb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vatghjtw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zkbxxkzj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3csriirsp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3uzneabim.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3krupiuqb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3idugfnqj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kbvxryvf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ctrtjteg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hnusywlq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kzwgdjhr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xkfwxxlz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3trppoobe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nyeyopde.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bcdztdak.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zdnvealf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3urnzxoee.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3iepvocbk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ocfhubhs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ozbpfrcp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hembscox.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3goihzlfn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ggetcpim.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kqnmanoh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zqjchwam.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3iekxwkwu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yltuzpmx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kfsgzkpd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pgetlhhr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wzeqjnry.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3yjnwgnrc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3miuryahq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nmwminis.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wihetqru.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3upnuceeb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vapckvvv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lzsiohdk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xkdbqyiq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhnuhxi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gxahmakz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3iogcgzgt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aedmzsii.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3izcbcips.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mthjlmsp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zfrsuxqc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xosmjpoa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxktyjq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lnzeggag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cldnahba.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xcjygtix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rdlwuivb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3skarnqbx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mpjlgltj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xyuoxiuo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oshswqop.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vsxbgqbc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cfmeffmi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3csjzbxmm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3buzmsoje.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qkhpanuc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fiujkdsg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sbpqslwi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ghiojzdk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3caznhrgw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qwhuizrj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3evnqcygo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vdowifee.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3naaaercq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qwztrfax.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rnvnoury.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cfncyada.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jbswnsty.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxhlvkh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3iblqlafc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kocvdhbn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xsedeogv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ijrplitp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kvrxwojr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tkzprmpg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3oprvfzvr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oknltfpd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3opraluzb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqisfcuk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pvjofaln.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mikxzblp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jytfnuqq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yegdagfd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3igctiuwf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3urrfsini.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mxdkkldq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wpqumrpc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mgauygmu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ostufsgr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dkzxplxx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3soinhfwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekqyflbb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xyeiwcwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmuvkola.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zaxoiqbc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kpzgwjbq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3tdcjxsfw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qizpnvuz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ztgakfqa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ewaovzqw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kbkzaphy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uxohmglu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hcrzigxs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fvvimhge.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3iokfqbfk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fjphtvqi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ahnmmrsn.html


<!-- 参考信息 -->