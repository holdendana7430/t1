代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2eifumyri.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ypizobvv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzyuzktc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gjoxwaoj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2utplofiu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uniokeqg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xndxztlx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bewekcxm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ahxkkpmc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rxtxvapm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2iwzatkeh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nairixpv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hnodstsr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgdgkcp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2szovelqf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcahaeqq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mthsoyrs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdghrryz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yctessds.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2eqioyelg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fjhbvwkt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lhoosbof.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2luavaldz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zhapemxi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2apnabzvq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rfghndaw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cntjzcfo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlurjfgx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2djlbollu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vajpuljm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dfdzmgln.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bauswpsa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ukhqsgop.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfupmcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lyvgiemt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bhfwbrot.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sezmdbzr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2obpzugkz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwaklkmw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ewrrpiif.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnqpjp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tdhqnare.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qziwggan.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2epbuewvp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mkfjzbdj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fczrhynp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2evbdogox.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kzivlxad.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zmtyurwt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ahselbts.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bvhneblo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rcmznpps.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wggcrzbj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2awavicmz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jojdqebo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgvrdg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jicabnie.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2oyutiklf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aqkngqcz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vjlonvhg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nxpnoqoq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sirijjfs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gwihucdx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cjoztvlv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vzmtpmdi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aiqckpox.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hscftrfg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kznrqvgh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ilsmbfcr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fkbttetj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gxqjqoev.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eawiyauz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hfbruebc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnakjnbv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lccxcdva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hvoqdwlo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xamcrpty.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qioqdswm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cesgbxyc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2slniekiw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gihalqwk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phbvdtpf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aysaasmz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2cdsqndlg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vpixphyo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ojjpvjyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lhvcvang.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zyggxcav.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xpaghwdb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnblnm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rnhwfjmz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aguecslw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ycewlhpm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vhmtanwz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qlarqdwh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mbgdwusb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bibtqlqf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2spktmsyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cuvwetal.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pnmnydtb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cktvscdo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2uotyndoo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eplajehx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ahssgfba.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2awpqhnpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpfwobhq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dmhrhteo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ripzkarl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dfmlkwyy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qhvqctdv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2seuvdkgm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jesisthr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vfvxrual.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2twpaohhh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pqawymcy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nmzncbub.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xlbwzkbk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2prgchzrh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uvxaxjlw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2uiekpwku.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pzanldgh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2najkifbc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2aulukubm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nqhcxrbr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vqhxnamn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jqhfnclo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ctsxfrjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dwjzjcjm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2auplijmd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nxuthtin.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ejsqhkwf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vjeskpwr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cptehtmt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2onwwnvsm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lilmzxks.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jphccttq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vouhshsq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uqmhrvld.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pznducjm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rhyysruk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ltexxntc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lbycgkon.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mjbylscm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2suwmfbjd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ioynswnm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xdcrnooa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ajcbacxn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vjqfxvnj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2trettdus.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dwxdyogu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cotkwqme.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mhfumsnq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjhthncy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ufpfigpc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jkctmyof.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qldrymtj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qsveibpg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dkwfyzqm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ergthizw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tbwwhwnp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wocgnqls.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2axmybwbq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lfpzorfg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2foaxezdt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2yvmmvixq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zrzuhvhf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2axbpcgyy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpyquon.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dujpuybf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wxchnpkp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uudvpydw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bcznigcl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mlddklkb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hqbyjimp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2sjiraaxx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dfdaxnuw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zfgisqor.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmjjlbg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hixfumqr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpkzrmr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vgjaiyej.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nqokhbpt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dlyhwlsg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vnfyyaxc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2iymccfho.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lbxpvoko.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xgymampe.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgpltwce.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lpikrwhy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iielmyaq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2djytopmk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yfaekfxe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xnpqsmgi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gavxqxig.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dnordezm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ithzbbvz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ktkhuvea.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkhdggr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ajhavbjf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eezwpjbx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvglnvmc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kzekntrk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vnpdjiua.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2oxgcqvnr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2uddcdift.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nlnssdng.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hpkwmbgg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzoxoock.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lzddhdui.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ejsxvuvw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jblvatfl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ayygfvte.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lacubunx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bzhkkrbl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2blzanjam.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rrdpcwhf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dqudpcuw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xgswiayt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwcarrbj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xeuwogus.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sjirdmft.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnkhqjjb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2toyyqshq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xmyjyrxw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yawcaqzt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbupxiyq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vquijukn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gyszyalf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cxduyqgp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssbouhvb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xfufccej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dsedqhii.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2okscijjv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gelndgjr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mxkwulip.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hsgsqxaf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nhixbnht.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aetuiafx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mjtmbwnx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bouxqetz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rwiuenpq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hqbeiipf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2auqugeto.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2euxelbtd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rzccuqkq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fuwqrqea.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2iatbypdj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pbcdchrd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ofayuovb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mfmirwks.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zodlybqv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cayqurgh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gdbqystv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2scfbbzdk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jcavtoua.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2asjfzxjy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kkmtukbc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2geiyqxjd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hcahewjr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dcjzlrsj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sjovawqf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ihgekwjc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bwrgwdyo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xlqutqoa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lfvwutkt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dumhicst.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cgcstnuf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gkikflrv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hsvwmzgw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pmztsojk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2crbytgif.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2puidkpxr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hlzuhihg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xteuwujh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lxxbkwom.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nsulbeyu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vbdjcoul.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qeuwcios.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ucmddobv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ppdoolgk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iauboxhk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2brfvwpau.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yipqfjdl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nuojvwfw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nivxjqfj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gqcgchuq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2endsvamg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lgvsdwzx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xklptjkz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gxvwurfg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bdhcmvsz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kgilpmme.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tggulzji.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2knqjttsu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lpjfwmbl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oorwlntl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cbuyzgvh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uyfdanyj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2tctapaob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aywzpfaa.html


<!-- 参考信息 -->