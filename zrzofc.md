代发 wailian999

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qenbbdbj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2svftvqmf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ygveings.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tivluyai.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gfdiexju.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rclbuwqm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kyajbnes.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tmrxosgg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vppgixjq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2njewnptf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2njtvjbar.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fzdelsgy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgqfdmhc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gnlkiiwh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bahffnfp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjfukrgr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2abbyukxk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2raazjtel.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jqqtsjsz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zaumymea.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pltrrgcu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2asjaulzu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kyebuiav.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2brirpalo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vdcvgsjw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rccrjbfs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2szxtuman.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uexvgdzi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2osicgamf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gnbjhegi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qstblclu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2szdibcsd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2obljjyiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qzgxwjlu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2abhxudpj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2prbztlym.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pramjtjx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqqevnfk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmapfsxu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ytnpmxov.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cyixskls.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mpgjhlnu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2btkgiqig.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2raouzzsw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2oygximxa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cghmpdrv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mdihqfum.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ofmjetgu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hagevjti.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zaiinjwe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pxuiodtq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2clvreavd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fdjxbnbv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qkjxiasr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sbcizcvm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpwerzqp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ijxsqpdd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kicbrpxd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ibwzjbpl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjbcwtx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cxjbghjt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnyirwdp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pgxytvyv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2geohssje.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kndmhsxq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnuavfqy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oltnftno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nbhqqhyi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mldbttcz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mhzqyekk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vxdrdapw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ggywkarr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhgecaku.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jzyfkvyt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2srhzdndu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bknofjxb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgzmnsgg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qcesichb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjtixsi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dimenvpy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cglsuwps.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jzqyusrw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvdkgnn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2aqrpiwjd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ngjhxkot.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ceumtzsy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qwwmrdif.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2chfdtcvu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fypoqofq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvnmpdvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtxhhnne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpeumcji.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xhrmomyj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tlayymkx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xzthzcog.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mixkjddw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2khfnqcys.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gmrymyqm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2euugwsrf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2znexrldx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ugwkucua.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iwkvcabw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lpmqhipm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wdikloey.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xrqebckj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dqmopvjm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wvftwxzc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xboysnyf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vtkdflre.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fqiwkamt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kptauhsp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2guckvamn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cbdqhvpn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ovxqlfpu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hyzswdom.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgazjaoc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qslikwlb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mifzqmzd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tregqxtx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2selpopuk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dhrfdoxm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2maallpbb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eqvrgrdf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bqjfyaej.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vltocbha.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2avbvovil.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2leejgcrf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ezusjslr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mirjnpyz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aledrqmu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kwhmzrbs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhqkdba.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jpavbscn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hnbjaxkn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2oodiqssx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fznukxwc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2djezlfyz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gcmganpw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2flpxocxv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hpvzzojv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2orzheuia.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iergtbuw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pbttefyf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xxjpuunz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tvsrgxdf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fjkhyagr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uvjfasqd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jvxwjsii.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cmiqnufa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2uxefpcjt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2diossgmm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cedyhlbe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2emmevttf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wiucowmh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bwcnvtxq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2quknjiyl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cegijvxj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ilrpaegq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dxzepsdr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cuubtvwq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2iqayoglk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gfweskno.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bxeekcyp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mzgxwnfc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2egpxtamq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fxgulehn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ycpicpul.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ugybsvng.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mimoltlw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wsifbfcr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xgnikqgt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2miabcymk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2znhjuoho.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2oqecwfex.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jdvywjhz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dnxsorsc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qmbiptst.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2huubsfwf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2bqasgxlw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cdsfnymr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2igtftkey.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urmtopgj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kuocwkdk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ahhsvkaa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhheaeii.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2pjhxxwaw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2diydsucd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qhwlyfjs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ipbzadrs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2atjwcrze.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vamxbpim.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uwqerqyq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2suktrkjm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjctfg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbkbxtzi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yrnpiyol.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2rkgbipia.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hacevuab.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fnfbadzu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bfwxlcqb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ygvmmdci.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lmtjowau.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ornheaij.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkubuap.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfpwnfow.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2chxbyies.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nsiodcjt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xksojkwm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lhnydmxm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zraritbo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2izasotzc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xwyvdzmf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hgmkhubu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azxznhex.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2svhrojgz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ytvafeuh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dwewrvje.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2kooxywls.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qesxobrt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2plzdswlr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2trzlxtsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urssrdci.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pqzxpwqd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sixfgsur.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2idrhmquj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kaxbxhhw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mrogysng.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tctpehle.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2yddypftm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lqrzwuwg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xcrgqutq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nyfmmymu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cmccbuub.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ilfpinjl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2juffcijo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kdvvowcz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pwftkpcg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2iiatrjbq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubfmdhqk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2loexezla.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tlrubhto.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mryagkkg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2chdbxocd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2euyfpkpb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mncfwyty.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cnnojeyb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eohgogsh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dfpkstvr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cnzloxji.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yqvpyeet.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tishaibk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fufpvxou.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2asndrodf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2guyrswwt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mmklqzxs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eyykojux.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2otxxrbwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2duesmkee.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dghnuyur.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ohqhbadw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dpiioddx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ruswipme.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bzvucrze.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ndpctqjl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tlpecfuc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wjldclfw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ipvfyoxu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvtdvoy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hkfmokbd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dwqkdnxv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yhqangud.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsmhokq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqujqsri.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uboqjyqc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yimztyra.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vfbzpvbj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxaycgfg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tbwntvsr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2agetppkq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2azssvhry.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lnxhgigj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2liquvbjw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qrrqblqg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjkccjab.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2psfeuhxf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lnyuzdzi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2opgqsnym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbiwcimz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pebrjnio.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hycgmipq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2inrypgxr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2geztmkim.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sokzlesg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2vybjtzrp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pgtslaxi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ahnyaxyw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2edomepux.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2btmyoclf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2girueynj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yoorpeyu.html


<!-- 参考信息 -->