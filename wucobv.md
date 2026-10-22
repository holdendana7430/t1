代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sjfifoqd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mvncqmbn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cleqiegv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yrkkkawf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2asjnudsn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2drminxwa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pkxyxxdb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tsvfbnwg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ekeovtqd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ovvgpuhr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rbwxkled.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mqmieatf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gkfiaroq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fzevxfrz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2eqkjvrhy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mjwdirkr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pgkuythu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xsvykwlw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ovbkeqsm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjtwxudf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rfdiidkn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuqkavqr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ifwhwaoi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrohdof.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dvtyfylf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jwvwljdd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zhgjmcll.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2adklyail.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2atrmhqyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2epmtgezu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2elvqqzzh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wkgkzuzx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtqetpt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zhdujabw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ydhhunqm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tqfkhmda.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpieeudm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2msfqsgrq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fxnprrsf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bhfiycye.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akuwezsu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kgifppcb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tznniuqx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2awisfgti.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ifwmijpd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gdxoupjf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lqywczwh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xweuecpj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2baqmhtbe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ghchsgcb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cuymlpfb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2uhwucmvr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gtoqruhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyhgemlk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftonavqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yincioqv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ojodnmzl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gzxicpdg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nkyycmja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2svmovnrm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ejbnahkp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zyvhdgvt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xfjmtebw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ckwriemj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xecnitjz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ortcluwx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gvwvmbyj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2broevovr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cubvoztp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kaggecym.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2blniveks.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hokifrdj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gyslrcku.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oiehfarn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vzcuohrj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mpgeeore.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzurcgki.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rawqrakz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vaduchcp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yllfkpfq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tjngbyss.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvvghig.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ixvakznl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oiouqofh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2degjrbhk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ghahyfxu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2iqasifnc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lzioclsn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ihfxzrnl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sjddnzpt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2eonxburg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xqqixoxk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lntievdw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2odunflbd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qbkamfpp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2duabvwsq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lkjoqvam.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zvzgglon.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lvhhahxr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pqccusym.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zjdeoklu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xlvdvync.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2yrnioptj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2otkzlyam.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tixyqloc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqqkzzy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bmyxivpv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2uorufhfx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pvwpojyj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wdglsvtx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wzhjdcos.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2yuvtcegl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fskfeibh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ihokhcab.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gzmhfhkg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2erxjlfwi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xjosdxky.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ywojqffv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zibeifmt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wofcsmkh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2cixytzov.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rvsckesh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yxdkrqch.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gwvutgyl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2khjobyjq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrabqmy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jxbsmmhb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmyhlya.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ugfdtbfv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zwsmmwrs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ldaaoxlz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yqvgmxte.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rxogmpzv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mpugaefq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bgdevajv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgaeshdy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pzrvzlxa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ylwellhk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rykkmihb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzowqlg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ddfherdo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ifiisbhd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rqyeqbex.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nkjzagzj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rbgkvxia.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvvgxxmm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gttsgxnm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cpxsodls.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uupzvqeg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ohjjyfjk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mdcqvyuu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxtjxlh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2txtzrmjm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dlobdomu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jpfkxkbr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfeexjfi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2drddfbry.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2azzeaorw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bdyvbluz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ipyrweyg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xrvjftpw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2npmygzvh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hwougkbz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eskqcjlv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ehnrfkjw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fagpoeqe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xbuwmqyl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgovzmm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2opcrpvld.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzgpdtid.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dsnnmubf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2esphwhej.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pokwacui.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mxtmjfck.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2elkoqmfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpxebtl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gmiyjmqf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnhzmque.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wyzhmbut.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nhowbdkj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2acdqdreo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mayduxpi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtyxjf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2evxhlvpo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wdbgxdfm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2blnpoqar.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xfljuxoj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhwyqewj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fugygnsl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtvypn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pzmmfmzt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dtavfwwj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xvpsnuxw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mlpoiqft.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wdrdraqe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qhekbxvj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cccffgse.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2teskfvwe.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wqqsmwfj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ysathzrl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bkgnibpm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2tbibyaut.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kjkqewjf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dybrmjeo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2arxgjwsn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ehbybhof.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ryvxamoz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fchrmumm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hmcvulzc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mexlvuox.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fsepgpki.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zmenbjph.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vybhmfpr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rmhbzegy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lcmsifph.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vnbypzjn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2eizvuyhc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uhmjhvvv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2arryhtjx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uhzswxfp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ndonqdul.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hackocvb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ycizyohc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zqtzhmrk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ykvgwxwp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2yqosybvg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nvchdwdg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2grdntebh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2frkgnukm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mdykxshm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hllfigqi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hivxqvda.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hsacqtqc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cjcdncgx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wstgrhwh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oehmxlle.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aroydgxb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yjmnvfrb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vpepzudf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eeufbagt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pxspalzk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yhlbxluh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tarymdpv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eozbvvar.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rjasjeya.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sleacgeo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zqfkteqp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dvbhmubr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2omsaoxgx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mlhfixce.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pyuyyjmu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vypjbcav.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2uyzlsmaw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iqsldxsd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fkmnxicq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mcmcqmcu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2iadakwab.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xulloulk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nwypfmvr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2izdqvqbn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lyjubfhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wxqqwoxi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ctclqwfn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pcfgyscj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2emwaxwcb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qkvhbpud.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kxugpeyj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lprygblc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2emljxjhb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjsuojo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nzwjtfpd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vjxifqvs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2okzqgtud.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tucglkft.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2etwavjnu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vstsubcf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pfapbvbu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fxqrzglo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dqkuamnl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2elcddnfb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pfcdygox.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kphfcdpi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fnuhuttf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2polyddyy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xqyeyeox.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jvzvzfkl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxhnqp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izvkisjb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dzqhbgfc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2pmudncpt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ehomjtrk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bpdmcvsc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2lgubonva.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2olpapcob.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2llehguhn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kbaonljg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zriafdjv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ulmoajhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2optkijmt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ruvfuuey.html


<!-- 参考信息 -->