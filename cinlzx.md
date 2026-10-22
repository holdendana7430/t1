代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrtgxwif.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ialbsbkh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gupddyin.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ylipwfcu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2pjqsjdxv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2orcbobqp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2igrlyykt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sdguifjv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mufckrxx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eojqxrwl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ssecsrez.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hwvdrcca.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jwyrkxes.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lqewkcjd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gamnfscq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aiqpsjio.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vmiwqpuv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pvieashi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yjrmowzl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2crnqiwsg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lejyxenq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lbfzzqfc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iqtavjdz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cnikmcmv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ttpeglgm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2avmqozlu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dinrgxnf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndqulztd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ooqepbkw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qmfxnkuo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjgccp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdphsejb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qtfykmyz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2usrxchco.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wieqrqev.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qdzsfndx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jmonmqtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qmotftbo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xavtelju.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nzygydpx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijwajpxj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ctdbdwlc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yafmgwqp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xnriesme.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qsruarjj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aeyzdfuw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2suzroyjt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2knageelu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tpnufswg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qnbceopy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmehivhb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zylkztkq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gdqnphon.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qmrnaklj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qowcghxk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ffrypncm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tqrgvwwd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tmloyzrf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvttfth.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yapvbrpf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pngjjqek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nasvbmst.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iaudsbgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcsqkofg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nvuwwkju.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2oswxulbv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rulvzriq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2atfrnict.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rwukwwop.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gzsaybos.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lmnodxjp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wryfhmjh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xwwzvxjb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pxcwzagh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ieswcwww.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vbkwmzqk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dedzjipi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nrirwvfe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pkbujudf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hxmaxcav.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wywwzfxj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jchihsqh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rbpglsuj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2snugsorj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wolnkcls.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2duvbtxrg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qkvbiadj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjiklrcs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2whgwihdy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dkadjfkg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cyapscqp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uscvuypb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xbjykmoe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2faiwxpsx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2aorssejz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sqoyrsxb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2clnrlaoi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cymiroyu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cwdnsonq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vioofuwb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tbtcqvlg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlybmrpv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ihteoshi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xojpoutu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ckupupyd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kainwgcu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xvczgmns.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jajcenww.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtrcxagk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2znuknmlt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zhdftekb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvxfczk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gkithzqb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jvyaxauu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ancgraug.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ojvutmuo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vzeoizca.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ssdlwfye.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uygxbztq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sdgdzapq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uxtrxzia.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2umtlsqjq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2inqfkpox.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2efvnxwiw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wuntklgz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dcwmuxyw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ydisbetg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vgyaotqt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pbwskfnx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mgajhutt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qatlxmaj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cxazgzcr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zozwajua.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yczgvbtz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mbacpyor.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gjyjnugs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ckitdfkt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ueniowva.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2prewmfil.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uqbbuooh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xmfbrzqx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2neqedwdi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sichawan.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kumvpoqa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2zmfpwnts.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2arpcvpve.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cpgtwuuh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2chjmmtqf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vdxuwgis.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zxnmfxsd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2avuwmzeg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xrhpwtmr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgoogrkp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wjwfuweo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vibypklj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bfjrcfbp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2fbphmhzb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2dbkpbbxw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xydflylw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yatoqacv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cnmknewb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mahotfrr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mxdrefav.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpfksfrt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tpsjeprc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2komevhhc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wplbmfqp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lltthzog.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dzabcqqd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tzpomqld.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2eqxoazjn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wcdoqwpm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kktojyhy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hehcpokr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zglfljcl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpetkrr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qzapubgc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jnottxtl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mcnnzxno.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yefvhthr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lohmswxn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2agvavjby.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ajefqvfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hphefcdh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cowayajf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kizrnqpy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2eijkcvsz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2towiklsu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lqjghuvs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uyogjmqi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2agyfzajz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ustggjgx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pdtegynv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aidbvbtw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mwktsnse.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqjbycdx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kpujwyxv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qlezifax.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2brfllckw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oagltdnf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jvfcmiiv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2scpxpppw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hrartmdd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qpsoqxsl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bktexses.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fibwlhop.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vnpjcanr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2urxkhcbv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lkuxapss.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjofrka.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jwxrecbg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2blbokkgj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ncoekaos.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qrginlao.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bacloslm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xtdwlpmo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aorwwbbh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2krsqmdtk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cdbiaadr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kxzsjipk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gdvvtxol.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qbrwwnls.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tlrweryl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zsmjqenf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2iizsiweh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xuzlmeda.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nwrcbbbl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2iuwbqsgm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mydygsce.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uohlxgwr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vsthuzxe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jpgqiloe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wliuzzje.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2achbpjry.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ntpasmwn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rnrvjmmw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ejdpfyyc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzgiikn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ekydrwkr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2czsgvivs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jkxcsoug.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rauzpvdo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hznxbrie.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2diixcuyu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhyxkqsm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2imiavlmt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2djeyimxh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2afrpetzi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czsxficd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zfqufpez.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnozhagx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rtzlqdfp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fnsuldlu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ydcrifnm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dtlucqiq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwlnsoj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xdhkruyk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mmpatyld.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sgedecro.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ixuwaujz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2odoueefb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lhtbqjcr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zfpbvrlv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dhcughyt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2oonrrnxo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2trbngfpl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yndfmnaq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kvmjhfsf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iuhfzukm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2klxjdfqf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2uzujptjs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qmbckvej.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vgbevjck.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2smqmgfpo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jozelept.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qqklmsyh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ymbduijv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2joyjpmlj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gefdupvb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bdryxaft.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rkhlxpbd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kqwwwwdz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2yqzhoktx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rwajvvdy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2glxzfssq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ikonvudt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sjvlgpze.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ivghjatg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pccpbbgd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qjmwwlcz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2huioladp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlbvvabh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iulhhrin.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2afdsbgbw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2slbvxmjt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ktxpemti.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uchzvzzp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2townojgo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hptekrka.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vvqzzydq.html


<!-- 参考信息 -->