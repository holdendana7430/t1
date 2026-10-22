代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2apokjiip.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pufqqoxq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ezjapoaa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gaxxpxpn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ucyykjbl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xuarflgj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kddunznk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2reojekec.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dqbirmgu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2avhnpceg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2geoitjxm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meacxeno.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2olddhvla.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2usdprjkg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2beaspzcs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2diyrompb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2phmucdmn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gflmlkja.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2svpiaves.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2klxqfthm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2biurysuh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gztzkdbh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mhrnrfyx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2etzgyzuc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gkbjfdss.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ruqurape.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uuareqzb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2larrcwmu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtpvqzpj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vejxfynp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzhmbnmw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nkgeebfh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bnmwvhus.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sakhkzve.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zkgwnghk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ncpcvhji.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wtzplymw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyrynqdc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sevpbfbn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lmiqplao.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvnxwcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abooevim.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qawjeknh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpqldddi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qjeudaqg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2amfxqwjf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sakergxo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbpmlf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uibpwobh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pdxezbws.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qdlvjsuv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bjbryrzb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sbrhzrim.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bgkpdtnx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jyaxkymt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sehbqbej.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jxnhelnl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jbdmhwzv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lwxurzgq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zsqpovrw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgyryr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iauzijmg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezhjetzb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bjwpgros.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ouhpophc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2iahvrkxf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2grbeccxp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vvxwywwc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gceqdsuj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjquvyi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ddusqeig.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gbienxxu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rucpiudi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2btxapslv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ykkxitig.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ivzamumk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qrstwxzo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jibvmcff.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbwgpjga.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eoysukyp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2omqnepfq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oplwjaps.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ayrujhui.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2btwextpc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uobcrhgz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wxaxennb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nlkbzyge.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2uwexmgii.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2aaqzunoa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hprrntfv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mijicfnq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hgxzwwhx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2atcwzipb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2glusequc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2skorerxg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rxyeroqt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wnnsgviy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2demuvwfi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fwkuilze.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mxisgidu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rfwgnafd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2skkpbnfk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tpmavhbj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qwmrhneb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bwweomyy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zvgnroxn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gatmtwoj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ogjwuonx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cdpqpxzd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2oxluqiex.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kngntgid.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2visturjl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2eazircfb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ohbzoqdy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pvyiehvl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkcxang.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nthkgffv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qpltrfgh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2moyhwcap.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hddufkcf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uvjbfngz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vifxnvza.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ikguxbyd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rubzrjdu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2novuhcjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mvqcowja.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2aaauppjw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fugcqzvx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xuqdbtcs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xejoapgs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugxrlfxp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eurchxty.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rniecpqt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfseqtqm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jiiglnpz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aqgwtxhx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2voozyjhh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sqqffreb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2oyvublku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2amoqzlyn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qemzktjx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cufmdrcf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ecsttilh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xtztlwvn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dimemqnz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lyxfydmb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2emiwgunx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkvcixx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2njffydbq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2spxdsosy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mutzuenj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pbldoqqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2alkiwdaz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pznkdqjd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ttnafide.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pogtkslz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wfquoqht.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmjcwnvi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qotjgesl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hopmooro.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qgkiacos.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2crjtwykm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bkqwlabs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yjabyxvz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vvvukpoq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2antffsbu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fosstwzb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qtlzkhig.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sqaynrte.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mlocwahx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ahasrgrr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kupxlued.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zelrmwuk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tdbexlgx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2sofezkmq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2daoatvtg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yipzxvxr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lmvuzgzj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrqhkfbs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xgitcgnu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pbkxjxpa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ztzvrgml.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rkhwndyx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fqrpxhcz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uboifwrh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bhjscbdd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cinuzbuq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2njgjidie.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rxljyupg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtoouko.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wpfrgpda.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sqakxgbf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lbnhqtts.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zhctnxid.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2puexyhpc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yclvgdty.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fnxdoxre.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dforhxoi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ernxvggr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kdxvpepe.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kyzfwncn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hxdjbwwr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dmtwvqbg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ijdjbrrf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zisxphew.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qfaqhxjk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pikfdydg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pwttuwpq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vgwwjnbd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sxmjfbda.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lxxrrush.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mustrlmx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cyboaejm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iecbhlvl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gvkvstcw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2anvvuqim.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2taiyoluq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2sjurnefp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rklddfam.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ybfeewrv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vottrxuo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eilsjfqf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rvolrnnp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vnlvunfn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2srbaqvzt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ohdfpmok.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ffhmqwpl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzoirmru.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bmdlklwc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mzklhuzh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtbxsm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kedqkldo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dgvqsugo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vijvrfol.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bugkldms.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xfhebxpu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kkzywyzn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2myaonqeu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2biechtez.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jqtjcsht.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2omvekqiw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kyuoilmg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fqcpkrse.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pmhoqzjt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cvfjbmmf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2prygejcs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gypysblr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cenpjsgz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2uraqtlln.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mtpdifee.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lexqvqsb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgpwfzbw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vyosgpqn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gtjpfjvv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irztlngq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jswmfxau.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2laybkift.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vzrieqve.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vjdwhyyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ggsnsplj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uxdnopzt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jgyrzacd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dopszypu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nikrsags.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mqzyxzrs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nfhkruux.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dzlrwizl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iygcooxj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pntedjqi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2egzzqvqy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zyqapvnh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfosjstb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kmuvrcdy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ctfxffyq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gpmczkuc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeafancf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lhussrbs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qkedppoi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2cjrvzgao.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sfggssds.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zxqkxzuv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ewnyfstf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mgueqcvd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rngczeri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apmsowoo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jwwnfkhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gitleifi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2uhddilsp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2eogqentl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2puhwlntn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pdzwlxnj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qnvcpzls.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pinxezqn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwkwuthg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ntjwajyd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jgpimxdm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ywvqbant.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwimoxhi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2srsbjgqi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ffoiybuz.html


<!-- 参考信息 -->