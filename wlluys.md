代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2amwncczd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rpmiaqfm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qkshkifx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bouvdgav.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jidupdjq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdcdiuz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aqrepgvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yzjkiesv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrdhmmup.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vozfcaah.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gukomxpr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgfismnj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2uetzmsdr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sfbydpzt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qzfqbkuq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2prhmgyzt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aiggxgcb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tosbymis.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aamouzul.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkkaubu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gmrovrzp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zdfdnbup.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2obmzgkms.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wokgrnsd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rnwhqetr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xbqdxbtn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gukjhkdx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qrwpzaiy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2klgzfpqk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ooeueabt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2josfmien.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dhqhfqwb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ujgbqrtl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2knwcwygu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2sblpqrav.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fwgworpz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lcthdfrv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gqntffvc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rrnuqfku.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iuhpuqji.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ncwmmjyp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cpviuoln.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2epnuyick.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ddbijqph.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ndpuftpp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bydewlma.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jojrisiy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lmwrdjxu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fmngfgwv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zndqxrcr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fwqgnnoi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpgkhqbl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2izjptpmr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oelqsaum.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2eqgghpws.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqozyu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rybftsrj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rsskuyej.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ycozdgur.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bdtrcpdr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wxlrypdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khvsmrkz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jtlnyujx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2adqgbrgb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrogoreq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dbflxgvf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2auglbsdp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bpftinoa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2alyeupep.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xhvmmjcf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hqnrvjjj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ybsmqjnj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oejnsubx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flffaidx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kxcsmtfi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2szjhczyw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2joxmufca.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pwnmvoyv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibqltvoh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2iirjrzuo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yikvalmy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bdwtkswj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbmarn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jdrcdfoj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2flpohfhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcozgjyo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jxpospxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maeroybr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2znzbigot.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kcdumtzc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mippsoac.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2axywgaji.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bhfsbamd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2iagaoyxp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fmrleyvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zbqnxoka.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jzwjwxeb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2chxuzdjd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2apryucrc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2izcejmnh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xhlmrodg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sowjojqs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qvsvewry.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ckizvyqa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kkukjyzw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tkyjrxte.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hbbokvhx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mncqnxuw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wwjjilbp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2slsuzsfu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rfdxhfso.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvsxhdk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ntporpjq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2actjaoht.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zvtxblzi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhauxq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2watnatvv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gfxszxaw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ymxbwnqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mtcplobi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmdkuo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kbpfmjbt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xkvfnofi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hoscipcx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2gstsyqiz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ibclspcm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nnzolpsk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jpptesfj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ydjbsjtk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2latuxjoa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mcnntrjs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nerorgvc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bxpuguao.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sbtruosl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2thfiuacs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lgzdensj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nscdeich.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmxogal.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2idxvfvzw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgbqxkx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tvmnkeip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tjquqtxd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2skpwpfnr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hxtkamzj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2qcexrjaj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zijplxit.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rolzlpuk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2avveeazh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bdathfav.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fbwjfmak.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ryvdxfaa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hmarfzdv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ljoepowq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dzpszgcz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dgpwymrq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wuczehql.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hcvqmzmf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ignfrobk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2uexosrpm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgtdaes.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2upsdkzic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mbssjdud.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2emebjvan.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vrxorpma.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ayooerul.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qkmbqcke.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qsktoqef.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nbiqrdjk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dtwmtfvs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rbdcjwpo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mxaxzzoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbuqlzkz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fribmebb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2filxowdl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpbxqppp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nxkuwojr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zhcwqffv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwlyzey.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qtmrhbyg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hqxnocdq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mndivvhw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2himbmzib.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ofxinrkc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfkvfpe.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2btjrflqm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2izvmtpsg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wtzlcsui.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jplurpbd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2aoxqcznr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2edbgrhqa.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yngpqamw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vlwrphey.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2etpjwkvo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lyutkwdb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fhujnbjz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kspkkiwg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vbujchrq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vkggjsza.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2owrfdqgo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2woajunxs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xfxoscvy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hiwraetp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tbmyvnnj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hglrzeak.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2yehyhszv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sucukrbc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hlchkgdt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tywgncuq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2etzrkxbo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdlccanb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2citfcewq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ycfvyjni.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jghpwjpy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dfimcdnj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kjbfvbnm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lazfeoql.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pqskuwll.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pxapwldq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qllngqxm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxxiitaw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xqcmhblh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ulrhnjgi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ayavvsyk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2eylxoaow.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jkpbirfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2obbjubji.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bmwwtvxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dtjqrdie.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mqxkyotd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2whgorpnx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fwzvxpjp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pheodjup.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lbomazoi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2smqwgwws.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iajcbapj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tqxocuux.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhbqtq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ldrpzosu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wjeuydld.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ofnckrwn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yyslqqrg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qcxakntu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qfxccrkx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ntakfnzx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mxukrbfd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2czokkhjh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kdkbtrwk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pqvkophz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2segakcov.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lggfpteo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jewtgebx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2fugzlrfk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hffkgqnv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wxenkahw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vlutmfbo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tkywxleq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ifeeagwf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2omqwqdtk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vrjchxoi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lyvxkzql.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mdipwnso.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jftczygl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ovnzlnor.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2awkiaacg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ixvvklom.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tadzdzoo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gbuibsxm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qsewugvr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ikmbpgzy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xsieefiv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sicfrsgd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2siygdobf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqwrlvxt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2raijlpoi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fovfawmk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pnmdsehz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2aemkqmzy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2weonvols.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bppnpwob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tfoijkdl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dsvpszmx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkmzkcqt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfjrtfeo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ikavxahl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yfyywgya.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dfaxjioh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cqgagtef.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bdpwqalv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxzhvrnp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rixtykrk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uxjxgitg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wedszizc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ksjfntjt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gsrmudtd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ixqwihdk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2khipghfu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yiokgmvc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qpvimswh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2apcahsvj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zoeivxeg.html


<!-- 参考信息 -->