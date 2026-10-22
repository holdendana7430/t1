代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxrvrofg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xhizqayb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xgbwgurb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozhovbpc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vahmlldo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbtmjyv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tkkkeccm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nllfynue.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2byixtudg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ctpggzxl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dnlptnel.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lgunqpcb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cihdxcvu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kzrhxvud.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcczyc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oqhfjcco.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2grsjjwqb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pkyfzsyx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqhlkavc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qaofglto.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kiyolmyg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dajtonwi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vuhgfavj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nhakgdpe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jamtweps.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvpdtefb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2foztumnr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dbogsyrd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zpjgecij.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zcyeyphm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mnzuptcg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ocgrevuc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ykpcenld.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tsytcjyh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yxyebxbv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nxpjmzyp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vshinaao.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ltxefgyp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vzarstip.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgtrzjhb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bcgsxkox.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2evdwfeve.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cbtipfyg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eoikeizs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xykqjlss.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bftfjylj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vaealssj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmkmqkz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aqwbgczv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xuqbikpx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xxhnxjuw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2emmyyrjk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zvpizaja.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2twewrdyv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fmxephxo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2xzyvnyrb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qiqmxtmg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zfnwtuxe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vkseirjq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqwvsyfr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hspqpsqv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dbdizzvm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cdukhecw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zemkhrgw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2riyyaiod.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bxfwgoxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lileylqi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2obsciscz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xhypdypr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zcjilbyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cmulgvlm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fmgfsnet.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jmyeknin.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vujypzna.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfxknev.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fbboakzt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2acmdxewe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iewtiqtw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bomjneyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzovjtaw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zufpstut.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qhkqkbdn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hcbmmlme.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hdsmwixk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2foybcvcb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nswvjbxk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ktcivgdl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hkpovtfr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2csvmoxnh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uurvptra.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2doalrzgx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nipwbwmp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2eepivfbv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jgeflnzy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nkezxapl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tgmxlkll.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sbqmzhhw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2npuxpnsr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2keggwhvy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xahueman.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cdsrrjpq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2laqkvlml.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rxfuucmo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtyqpyc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tdqsiuck.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2plwtvnbx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2iladeugd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gqyhpbqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sricmint.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ncfxrueu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vvtriltc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2duvycpwx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ejxkkjpn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ndbfahks.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bjonkrkb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cqioemjk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ktzoryzz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cennpddf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qctdjvir.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsfettx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2buaofglu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yfcumolq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2srhhptjx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yaysxisx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2szcnlgwh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fnkbabry.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ttktazvb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nsvdlisz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uuuqwysx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fbuajqvm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xqaaperk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ezatjouv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2frbykvfg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zimxuybo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dhxsmsbl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vgagclun.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jskezbzl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cghrtxoy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rskdwacl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcvghdv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ncgfgsfa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2adslwvuk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2shlchjoa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nqzovjny.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xfqdslmz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jzqgzqfu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dkezocwt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ncksljky.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kkdsffpa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wmxtmhoz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2syllcasn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qbnlwghb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2idampymx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vrxxqqhf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kmuqftgc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2eplekzeo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jlafyrhy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xqzthoms.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rjnqoctn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnipjgcq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wqvayhfa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qcpafqph.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ebgwtgdt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayetyoyq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tfuokwnv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jqdmvope.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dipraebk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2szmdhnho.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxltyftf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qvfwumuq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nueomxgv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2intfoijb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aintuami.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hsqvqpmu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ucwklvev.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyttnvbw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vvnientv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2obgtmjhs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2obqubsiq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ygwfvkro.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sdavjdzg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wvtbpojf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cgvuoqmz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2slxosqsi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qpdghehk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bpqxxheu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hcpgjyej.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2metxyhwt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2spawrhbn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tguxjijb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jsucmfjr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkczcwz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mbkoargy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ytldtblq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2acvcqdla.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wtspowyz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mxptnzzb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ogspisbr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2elbunozb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aexlrdkn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jtivhyvo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwmikat.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kfzcbtwz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bcfwgnsb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2scyfebmj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cnaaeilk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gfynuolc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nndrtltx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vrzacebc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2waudtmbx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2eizkgyzn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbdpsr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gyohkmck.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ejnexdnt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pfmzhrmv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sfbfsqij.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fsgcafiw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzuuccig.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rdmsjjjr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wahayola.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rnsqcjyg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iajkxdje.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2flgdptzi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hdnthhip.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yiuegkzm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxuiwsn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxlnjmod.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2btyzmsii.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bpzlbmcc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xoypobwl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2prlqgzpj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tyzeyzvq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mocrdtbn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2eekaiccw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sbjwecki.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wnwgnnbf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbpegv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sgcvcjgu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vhemcuyx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lcmacijx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sefwgsiw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vllownar.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mhispdxc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bjyihayg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qkbuhhxy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xjebwoxo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2djepwuhd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kkwtklry.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uynbpcwx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cppipmui.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2srqmnigx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tftyiqya.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kxbllbrb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uxauzuwb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2vejcunbx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xnczrgfm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2iepyikob.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pxmwuuvx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2oydkeqiq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvkcfwp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovqblkwn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2psjwrbsa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2miciuxdl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ianxaoag.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ceqrrelz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qfnuzrfl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rpgcpicp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ldscnmbb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2smuiqbgs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hnicvcni.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vdnxwlqk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzlzzpbb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gokbnamh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xchlqfjk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2docinkkt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2luortcbq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dlqpalyt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulvojuzc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2igtwrhuw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qfyqtcas.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xytutpzt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lqpejhrs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ooeuhzim.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2oqcnmbvr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ucwzkejz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2awkubdww.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2msuftzkb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xjlchfji.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pniupsae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rdsxamfm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rekuqekw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vtdtmmxh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ecggdenm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vykvmxra.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ckmoxhqr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hsfmjbcn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ilachbsu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvnkmsx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vyorhzwl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xgeyxwvj.html


<!-- 参考信息 -->