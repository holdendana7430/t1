代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkrqjk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gnrkwkip.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxjekdia.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tbkknhkb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2soovzjxq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nprqiryh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2itbsqbqp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yjhelvtb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dkrbnsyy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wylxskyi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2muxgedxd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdrsdpza.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qtdhxzmx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2loxttbwc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvihwetj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fyqhoety.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mreijrfc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgadlmtk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sykazrzx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ezbxtskj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fkcdttfv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dvwsojlw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gstliwxr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ewzqcjvd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktlkuvcc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ybtumfzr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sffrtmlw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qmvtwhmx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kszsjtlx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gsomxhhm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngzebyaa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2byexalee.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bqzgxyqj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sgwwymrq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2beojzvme.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2adbhqeip.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ifapyjhy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wntkvtnv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nvuuhcjr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2firreayv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfbayj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kskpnuue.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejporggh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iinecsbr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vpdrfygm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2podzdcek.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mqmgcapq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ylqxslfa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ogjeyqhn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2smyyzypu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vorpydcd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rdrnxpsc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ciddijjm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vvniwbtq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ewqimwut.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hrqjatgp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hqhouobl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jsnlqpsp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zyogafsv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ovmyirsf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2owkcadkm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2behwvuji.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tndfdjwd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zbsqqtru.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zrbzslje.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rskovkky.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2khncypve.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyzzwin.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqxxpovb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2nncamnut.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bozpobsm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2blmqtiet.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nqqdkyhl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2enrppsgd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mgdybuoa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nwwlcegc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2snrbulmm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfjztjd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dnqhsynw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lhuaogjt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mileywpk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vutriqqh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fkksgihs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nwjhpijc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wbqcbmsi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2aumlfnrr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tpthttrq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rdmaakio.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xnrlvqax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2tfvkngqr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vjohzaux.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zvolcobi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ezmtekso.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gbnyqewe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rqokmshz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pqysnhco.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xzfibhdx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2okjhsuba.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kmucvmpa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vekksojw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wzyyyarv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pvjgvmbv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nkcvjrhe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqunnef.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eqhqjmrz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gzurlfbp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vycamfcz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vmhecqwf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hlvnrkdw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2chghglgx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ngvejzcd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nyaxxcqr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sqjxdgsg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2abfytdep.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kkqaabcj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hupdvkmy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kitdiywb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xbffuuey.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2walrnwbx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ptsefjva.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pximzfrr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bjigyshh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2awgrlpgz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2smdrqiev.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2egkbtmyx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xawrisbt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tspxirah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gewxtrxg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vwctgysr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iotpddwz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2thvvwkkq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2weropdya.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ziqvytpg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxukmqxe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gjhcejmx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cgeaeiwe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cyvxewej.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hhyyjcza.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rncvskhd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myrghzsd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kncmbepe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jevpujxi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nuyxzlla.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rnxiprqf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rzviewsg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fouytppu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2teezobsr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ipecvobi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dnohezbk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rupjtbnv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jukncinf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pztrvilp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rhbqbzjl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bwxgbflr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yrupmzpp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxidmlq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gepujngb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfftczor.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zkhrhoys.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2purqygcc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2heyhmprw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2onafwoif.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2itucobib.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pmfxjasv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2njvxdkrg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwstfbcm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ebyfgmxp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dhnlwlhq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ydfrgqgq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ukqzgdsm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2usodapzq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fchmyrke.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2psqqzqiw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lkqoaotg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2whhqoiel.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tljnjdyf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nkjrlnmr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wlrrqmdn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrwkoiis.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yermozvc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vjzdifgc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ubphsvfb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ahcvplih.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lpnatdbm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2craqzgrg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnctgot.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2frajvsgz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jnmfqfqb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ayjcoiti.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ijakoksq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rpvlqchn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2parwlckw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dkhdvvfr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nlzanpfb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ynzikhvt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pvsthtzb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bombygvh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xhdnpdxu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2shxeidwg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jaaosoln.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2etijicwm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2aqlepmcv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yvrhcihg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gsqjvhmh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cxahpdmn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zflmbhyu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qtvizurd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkreenaf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cmhhvvqi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jmtpzkzn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zlrzbjuj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mdyoiplg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fbfinmzt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bgvlxkbh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lwjofwzh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hvnkfgif.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jdhhvatc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dflaagvn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ikvprdig.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rietrbcl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xteaelae.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zedanekl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kriavoej.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fpfcdwxa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sruejjjy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ofbaksak.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jhkqutew.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yccepwbu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgagzpry.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fmkuwaiu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zwhskdxq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ppakjdoh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2eqfohkou.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2admzogje.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rpqrzmyp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mvlwflie.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zwbtzjes.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bgimudnc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bcnigtpz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qrnhmhvd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2edivtyxv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mdocovlf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lriwhxaq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2geskxzfe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbzhtqxb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2utzqiyxv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jhwruqvk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zkqnsezz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tsgyqpkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bupqbiqy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ywytmiqc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aynqrvyw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2chlnpigb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xwiyrual.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zbcgpvto.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ijubjbib.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eslsjvux.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2grcskqzc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2iruqszvb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bselqfii.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2nvrdqabq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qeovoizv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iutuiiwq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qvpjfxjq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mwjhpbay.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2npfeiukj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rwrcektb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iseorvgl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vaeysjbv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fmsaugix.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ujpojdne.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hqairhyr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ccsyviuy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qviranue.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pisleath.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mmwqmbwn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jmmqcdzr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lmoamuaz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sghnxdnh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lfvysbgd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dfnslvcl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ovxiwryb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tlwbfrwe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2otkmimhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjrkkrky.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2luvbbxao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asjqefkq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kekjhlyf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2akerljyi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qpolpbgv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tsqpsyxs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hgsqchnl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2umxdqsjm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2psnvwnvn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vcgijnih.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gxiuijxn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xnwlxcvh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lqknvtsu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2spvnekhi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2abhxetdo.html


<!-- 参考信息 -->