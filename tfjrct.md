代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uuheciey.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zzghgafs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yxmwweru.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2diqwhbxw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vcfhbzlw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mpsiwhac.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yfrymlrd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hzplfedq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wngxalek.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zjxwejoc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2iqpdcmnf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rugjxcud.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tsdwgzvj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2iwpyesdj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fdubbpcj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2armymtss.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xiaqwhvc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2agtvqbkj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnaydhvs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qsslavrq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tchlwntx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2yiyqvnas.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ralarqbn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2evqxtbbb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xiiqimpz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ykyogxez.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2amhfgofa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zimictmv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wzgloofg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pispfjur.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xwjnxstn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dkuflolf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aekeerji.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nmysdpja.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eqqrdeim.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2icjpnsim.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nlnugpee.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2arsjgttl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2druwjmcr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mxcsgbqn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fodegxoy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkxjvsp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lqevyatm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2iemgivrx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rheqmxth.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iylguvvv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrmuciot.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uxjtnnfg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcdsulpa.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eqwwimqv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qxzjhfnv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hooabwln.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gqnsmeud.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qmefsvpa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tkzqajhp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dodtzsiz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdfihue.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tetkgnzh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rmksduhu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mfauzvsn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yqyhqeat.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nkfawmmk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sagobzgw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hsecergm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2szqhukzj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ckdosuyz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2espghjsz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hlurvyjg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hacbohvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atadlulp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gdpcyosn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmievxju.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fbxdjpgt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ufafaplv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sslyyrbp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2masivggh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xmyokgwq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2uqdfnoei.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yojxndgg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pvwmivqp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pcihwsps.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ayvdtpas.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qaqamziu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2npvhxpxv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qnzfujbm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gxdfduvb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cbksxkhe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qjidwbpx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2aaqecapc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zfzdqqfz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xrtoqlca.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rewligka.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dtakfzos.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gebwupbb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bavsospg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iyprejuf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jljrkitv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jeajxelb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2prbvpgpi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzowlf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uddhvcda.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qrhqlbub.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wcsqkmuf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wyzroccf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sriniqnl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdsbdcr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lfqtqsbx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dbsrwscs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bkwwoksl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iaflpooa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xzpgpdmb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fjhhbijv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2esalrzai.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2imzhbffk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2uzumddaa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hmfjvobc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbwtbktk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nwzvufoo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2krquemmc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhhbcza.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvtqae.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2glrmrapk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rjjpvteq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tflizkjy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rwottfko.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2prmjibbf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ywengcbw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zmmhiilb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xmchpmni.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qyjxyffv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bmsmkfex.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hxgvboph.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yxgpbmov.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pubxznks.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2srynhuqk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mbeuhbjt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2oztgkyse.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2prrlculm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rkdwfpvu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hbkeefkh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2eolgawkk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cufaefdb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wdcztssi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jlxdamwz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rpcvsfck.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tvyoqbzu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2upjjgzcs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2srefezjb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mdidqoby.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqwnxqr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kvvjgtbr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wodnrybl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ykjufblp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cokoxwde.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2htxwjawr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2iiasulrw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2euappsfx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tqyicvrl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cyhembsb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2idkooram.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dllelcjv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzmrgdq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2rhricosz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxpppa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wzubrhtl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vvvhxvwu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dgqiugsx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2efmfgbjn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bevjwlpo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2spxdqcib.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hnszvmtp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2alrrwusg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mjqirlwx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wxkauxqf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qjkkfrss.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zqhdktal.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gsubbkkz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zjeommiv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bapuoymb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2beuienad.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kymjmmiy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sozmvryx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnrvzzdw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xxbpomcv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rqnxslin.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvahecae.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yfzzgrkl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rtwjdlab.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kvfflvxx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdoddlyf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rqorcdik.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2miamelis.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bykxbzpw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqlptjnj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tctdpori.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cnltvjts.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rukgyqju.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qubsgusq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukybrhak.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ilchawvw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sgiphfhl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tsrtebvc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yqmwgpco.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2powmrrjh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2eyixegym.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dakpokeb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lvbmxuvd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nxpfllrb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2idkkfmaa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rpxkjfal.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jfslrels.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bdpumlfe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ugxiunug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2czbowgay.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kxoctfne.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fjuclwns.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2eupvbspk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ksqjvqvr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xfswusxn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sprjurvn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2uecietfw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kwvdeuon.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kndfgjgx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2imwqyexz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kqpvomzp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2igegzglh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2abwbaalh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2aevanidl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pxrzyxey.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ayppykbp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zlqpaecp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2syqrfycv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ajirpomt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zscwxhep.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lzzomeug.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoeonfud.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jqluruhs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2huhrjjrk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pifjkhrf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jubhshcr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tilpvgow.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ahypltse.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fjrhwsnx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bsmmjyte.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kzwmmjjm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2obosmqcg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rawuptdu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2aismtnui.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wejxophd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jaqzjyyx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jmggwptd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndllddvt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hcdhbmrr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2alaqhfjr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vaffummn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hogldwwk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2haifriow.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hwlustmb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkypuwfk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kzajrtzb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bcyyijon.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mmzbwrkd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ygbdrmta.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2htxbvggz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ehycugmf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aiiydvnq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qbgsedax.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pdgmwgqm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2owqopucj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2eysxnyfa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2owsxquoz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ponfbufc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yvlhxmty.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eenhaqty.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2suizsolw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jbjgkruu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2laurpjsn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bgplveut.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jlmopwqs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gwshltom.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xndqebhm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nzbajjth.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lnirdifj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2drcryeny.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ovipsweu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzetofu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2pvchaetx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dytsuqzx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wsqcalgj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kotxuopb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kzatyjrp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbizdb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2opiupjnt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fnaqqeeg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2swmsobjq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpmouji.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2epmuhfbj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2brienqus.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2szuapbil.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtuviafi.html


<!-- 参考信息 -->