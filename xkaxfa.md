代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pzwwjamh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dtswwlrh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bvqzpodh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2sziyerqz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ufdgxnep.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rapnatfc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nudahily.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wsealnud.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uwaltbbe.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2aslrrdnf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lzqewfsx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2exgkyqoo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ocngbcwk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uakerfti.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ssvrieux.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2faarwuvp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oeiymgag.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ghjxmcjp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dcslpwgu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pkyrmtyd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2onphohxh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cenpowel.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tahrddis.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2twxuvryr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rsjsehmb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2upuadgcm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dawkucjn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wqgcflet.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iqvmgsmy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zauktnda.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pmlrvxab.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqawhydq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tfkjemix.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xruadtky.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qqynmjqo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xdyhhbly.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hnepppuu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qdggwvwx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dsbrkhou.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bzschkfu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jrsfqkxp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qhvwrdiv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kbhcqidk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eepnhvff.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aveqpzlt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dqipgjkb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2upqilotd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yhoqtuys.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdsdgfng.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxtcfk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zdqhuodb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pfxasirp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kyraaxfi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jjroanbs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wofcekjf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qhacjqen.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sxkwytwj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qiqeqtns.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ofpizaod.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhztsxy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jqpdifjr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2skgkjxfu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ebldpbbi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bcvwfhus.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjpliein.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vutconvs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2facbtvmf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lpfkjgkz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlivgtz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rgjitkeb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cygwynut.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gdsazxbw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nybxouhv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eidjlpwp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2igysntko.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jxpybmqe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wowqbesl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vacjsbug.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmuwofpn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tbnumlsu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgbvkuy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zickosts.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sznztqrf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ymsfvhmy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nyejobti.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2egflvsnm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xopceihv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ahuznwtq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ittyfwnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhulghhf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2omqgrkhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cusqepev.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lukmzyxs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rmgbbtnn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kismcvjf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zpmzhnqu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xsegmeat.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ifaqkell.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qlkygxje.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2odxxjgjb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mvdnssij.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2txujoeqb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jaavieml.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xznvphis.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ylgxxaau.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eftfgkrv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cecbldld.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rpvpdzzn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hjbfkiyo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqqhtgt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yhqqpcod.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cmfsdsok.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ysjpucil.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nawbciqp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hkgqqyea.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dakfedbg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2llvoyvzl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bbetlthp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2oqxwmjav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wlhtzshk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2brynfmef.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jtcvbtox.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2juwvnxpp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dbfzxcex.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2olgjpjry.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnrdrpi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qwcxhjuo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2esmxkreo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zskryfcs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tvkoubkx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2majzakdn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gzkyeuka.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2igxalixd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2imvykfcx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nzjchxtd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yaqcamyl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cnugklia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ziglabcv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2atewzvvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfteako.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2einadaif.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ermzqugp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2crwlsxyb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbvvcbg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2elpvtbgg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bhoyylwz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mxkkutyu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2iidkgnae.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2novuleyh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2cedlmcrk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oxtjbwwj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2miybzjwf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eeidfwlp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kcwodvzf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2syembjas.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xvhhegdj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lcqvlddc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dfjreoal.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sqtttgqr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jjhamncr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2iujexaob.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dgtmqlwf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zebtacwj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kyqwseyi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2acyfupgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2oboafwpt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ccgbgtdt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ncdosfwj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qfrscmng.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2krjwpmgy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bwtwinqc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tmsbgumt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pkdziger.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bkmduhio.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2brjbkvmk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2imkxltcc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jvsrurkt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dztjzlrk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tffiluxl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vidhnthn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2reklukps.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2krbmlacv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2npwcvrdv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2asdamumq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2guyyhshq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bfoxrnkf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yvthkctd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ybexjlmj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rlkhahcr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dmkeaknk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hcwnzujx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekaawvvs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2duzymhiu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jwcpmhuw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zymxhrcm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uunknbvm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ggiznhar.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dqxwoboa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uaynozmi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wmluobyw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mtioazbq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hceuzhct.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cfqibtbe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2brjfrilu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kxvvlqpj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2acprebia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2isersinr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tfzfsblj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wnilakrb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uokmnxxr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wtkyztzm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ofgzwzyx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rcudjokk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuuiopfa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2iwriwxbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qmtawrbi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gndzbxga.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tigdprim.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qcoyxxct.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eqjkgrgs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2yzkfcubf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pppfxhpj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pbzpfjxu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rilzjudo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vekmxfdy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rdlaadrg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ufaeoryz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2smocmijg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fbsrenmd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxsxaqsm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nwfyhkkc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nweixmjr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zgxgmdgm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yczibczf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2esbcyqrc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gxyrtgsr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2szdxmvou.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nczytmbb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2amjjhfzh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2oicubamh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cmmfucvk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2arovedfv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mfhlfxvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sxdfqrcb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aqevgkqc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xxzdfftl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oojhgcpj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rppuktym.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2atxhbbqg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2azlggsst.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rczqlvhu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2evfzfiaz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ypedjvzu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qujjimbi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2naucjmiy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yizxvzfb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zjgtaijv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2otvmbdhx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wdronmhv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cwljdldg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cerzyqhz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mctlhzbr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dqttbfdq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ixramdus.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kqmbdsnx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ifopdfkd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wkzibdxi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2htdpxsxm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hdhdvtkh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpbbtc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2requtcht.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgnwebtt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bjmxdcjz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mpjwtepu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nzgtcgjq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2umrweglf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2djchffsc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kdbmfsjl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yjsszdez.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qastwedp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2phuyfici.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2loiiudsq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfkezb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgrghqyg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rtwlkfyw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qqepzgah.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tbeyeqtk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gashfsxc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zetbsgcd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kdtflbxu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ysvjuilf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mkbqaxfl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hvzebefj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fksedzcb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wcvjadtz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bzwzbvkb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jsiuxupq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kktsqqsm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vmvnoujw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2padzwwkq.html


<!-- 参考信息 -->