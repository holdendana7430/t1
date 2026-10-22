代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tomookts.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jsmctcjz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2usjxovuu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lrtmcpdj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2olyvjtuf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nqrvaivg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qyamwzwq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bvdglzep.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vlhzjrvz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dnodpkxu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mjkoeuqu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fqqxscpg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2klgmxdwd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hchpgjvj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wncaaaqz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jonjynmq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2egqalsun.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmtfitkz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdhwlgwr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rxrfcczx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2uqkmeype.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ssacdcoa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eajiyuxq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2warorrgb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmkkuotc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2azigrbmz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lxcouvgr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tnblmpug.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2enoplkag.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nuivitnp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnavprgg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lrnorres.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ksuhnjoc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gqvaurfu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qxcbclfp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zibbjycb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aporvvyt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wjtgztax.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmzdddl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2coiemiiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2legtgbrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqtjik.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qwmvfwfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwkrvozb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qndufykk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2npxghtgn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zqhdnods.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qwmnnlzp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dtdahuev.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qmomgzsf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2trmlunre.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2glihoynn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rbewhjpv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfcapven.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dpuwlkhx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2erwchuul.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2njmktzpf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ztyzufdn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2tzcqusbd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mtherbib.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ucbhswnl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgosboe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uqdvbfcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kqkjadqs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cfdeuegd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlgdcod.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2iciodjui.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwqfhge.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cmivkthz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sdoramwj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tczuxcmu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zohovcdy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hvrvvyek.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tsejapjw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zvdgzsle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ozvvebcg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xmscuefd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gevfgiro.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gmluwmny.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gtuczytg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xmpxzxqb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zabghasb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wptpqimx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rcevxrjp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2iglcvqsd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qqsmodka.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qjgaiybv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xelslpeg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ghefvgkn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2affkeqxc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xpazfsnf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgiozfq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xbcioqzw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nfltgvxk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yfcqxmty.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2linibllc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2soouqptx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vzgmypin.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ppsandws.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wfpgehcy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uhrscqra.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2amhhmdke.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2owgpankk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2urwkhyya.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vyeydkvd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2djjtyqzp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2knkmsrjs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sjkykdko.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mswtbniw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dfhgvetc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hhmfydcf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdllkxb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sprvrlhs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cwvndnxr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ibfpntxy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rfncxkul.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2blcvbbxb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ijnlffkr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2viuangtt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qqcugsnt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nbzzsmyp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2orwvtdkm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2poyqxwzo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2okbpokrj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bpgzuybe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xacnrhdi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vxvndjnl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtmnrr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2erbsqzxx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2aofxatrm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2iwjfdxwl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fgjxpoun.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vdkfpxje.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2byaejjhi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kvqrfaye.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qbcvquxx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcfcdzem.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2enmlhpid.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qshtliaw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ranbjzkz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qlfjeati.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yimahdva.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tmrrijfw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omapwvhy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qiskihes.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2eubkqzxd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dmazhcfz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gsqdygma.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dpxytwat.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dxxdjnol.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zjjmedtn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2edjnnefr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zgxntlir.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bsjukjpw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iidqdlhb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iugwrwnr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mlwlbegj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmzqjilc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vuchrgfh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qufxyuti.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ikflynin.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2erhpilhf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lwuikokw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2madpuixv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vadesjlz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oqbveibk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kzggsscb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nxoqqson.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bfueqhmq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pehmfrgl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vhgfpjqp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2iszjkipl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tlteztxs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2muiyydkq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2doquoetf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mospiqgx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hmxviwzk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bxilfdpg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdlauhan.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ymdjfpau.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pvepvcnt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxydzxc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wqsjivzz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vuygpvoy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oillfzbe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nlstzvpa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bxhwyggw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uuexbllz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wasjhxmh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uvqyiuuk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wmmcsdpk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fpzxhugn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mqxiyuqi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gsgxfaik.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpyaxd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmjoksz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2frmdqgwj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xxxmvgre.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ngrfvkzl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2rzxudjtf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ygaaqpda.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nykjfmwl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zueehytt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kyorovfs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tvnefsge.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2nxmbwaim.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wkfecepm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2akhjvahj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xsqjjopu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iynvpxmv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zteozkhu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pgsojwad.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2digohhpu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yneiycri.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nmegtjyq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2iflyiofq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2keljfsfx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zgdwdzei.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2alqqzzir.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpooezoo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zjbdgicr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2twwnbnrn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzstbnbp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hguxqhpc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2avkdnkzj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zhbbqpzl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qndwcgii.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iekdabbx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rschxpzx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2nlolwdes.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nziuzdoy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2leiormbt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zpstvuhz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uiqijcew.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yytvklbd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zxtvuwrb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2shboxyvd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpvdspea.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2teftzosj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bqxbneku.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wtlkajel.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jnkdbmdq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2oycpkvdk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pjxbfnuc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgwrfw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kjyidaga.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2guvwyjyp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fniazupz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2llsiixxq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2iqphwula.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cxyqesid.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iqaavscp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tltitmki.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lqjfokkj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhrfvr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2uilzszdx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eeqbwikl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvapsei.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2uxhszwxl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jhsdnvhi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wcjyeuwh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cvzitfyr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lsnurbkg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ghrpvxfz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hgvjcxbp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2semarexy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hewfswxf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nvqsgmya.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2goajuwdz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yqycerfl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pikqeirh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2stbtnrai.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iqdaujuj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tbhthcea.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdafja.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlzpvkky.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vrgpqwjg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jplgsvxp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dzmeedfa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2uaxjcizt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2araxsytg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rnrimqlq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ohinrpjs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ltjbddsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcnwqsrg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ztgnrtem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plaepapi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wrbikbce.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dkbxlzgw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2toxuingf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mxisylpx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ntrmlpwl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fjooxrdz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2okohashn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pvftwjly.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mwjtplvo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tjbapmhj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dqishpyp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2poywsxck.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2prdbhebb.html


<!-- 参考信息 -->