代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cuqmulnd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gygsotjp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rvkyomge.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mhyusjmk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuvoacim.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpmejtct.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qpprbzgw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ilcrmfyg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vlnikdop.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mvrumwyo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uhqezigt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ajrsrvni.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gyzctkcl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3whupwwaa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lknvmkei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzzfjxq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hatqbtzj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lpmtsilt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3povnvkgy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dojuidtd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hdblaeuf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3raaehdmi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkiadeft.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qluddnlz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ircptjvk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pwdcpvju.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rsnirffu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3siqmsdbq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ucfqqqcu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mginesio.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rzotclrg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3msecsgde.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iaymfemu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kyclueao.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vtqfugvw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wrnjrexn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3swgyszun.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lodavcsa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eozghpzf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gdpebupy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkmjuzml.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ovqxkrfb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kysnnyup.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vsxxsqkx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lqezqwfq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eufebyrm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3idsmgmio.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ylzxyzna.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rbkgcqux.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tyacldlf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jsgelhbt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbmoare.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qfjtfhff.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwdpimb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3whjidwfa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3uojqiopn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgtzxohz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofrltnzb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fpnesufy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cfkmuiif.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdlcvsky.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zlrucfoe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjdlfgct.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3othllqkb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mewowmga.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tjlyzveo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3apwssxfu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3heymvzwr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gndyazqg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hqbdxlni.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ipkgjcnb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kjbwytdl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3obxgmdmw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gsoqbrdh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yjscfbld.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tlxecxlt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kviidrei.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oqsaxzyc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bsdxuppz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3itgyrxby.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kulgfapg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhpaqrsh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnmpopvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxocxhfx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3frzigbcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tzmhoiab.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ksukapji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oflncklq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xgfpqsfx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xejgexma.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bnvymcbo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ooxlwdek.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mjmsbzad.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3laecxuvy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cvqeathp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vbfexqiu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cdwtvscz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eiyotkeq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oouhzpmj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cyosxecp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3avhvinxx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gvlblvuu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xwrfmtea.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wqqlrzhc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3motsnbyk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxvetvno.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3krfthzsw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3naytydcz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dnzuhoxs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iuwprtcp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rszdyxxi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cdrmwpiu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rabhechp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3efnnvhnx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mrpkwmzl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3episuxvu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jbiklebc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zsgmcbes.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vmjwbalo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3psktrpfk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gkwoqzez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vgfxqsqj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tcnbwygo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrwxqte.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3roepphdw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nxsvvvkr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3napqpyxm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ujmbvkzj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzusashd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gizhujvt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vxhuzqzz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3txcmaybf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pcpvcdpn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nbdzkutc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3etodxppb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3giomjoid.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yvwyvlzx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zrgfgcoo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vfdesbxb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lhsfkarr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3szqpbshn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gzvlbkmn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jbnxbgfk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kajvfvxl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mcvsptxi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jizgdlms.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cmcpaamn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dpvmvsom.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wrglzpvz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3clgbsfjm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3steanjqd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bukdnxpo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nzviftrb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3feuunfcj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ygztlnwv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kvztuvpp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nqmmbgmi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ylglaguo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wowgwfac.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bstvjiwj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3knazoefp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yvzjrdtr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pkiwvemm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mievpfce.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3npxgzxwr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jmuwkkin.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gopfijib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qxjzhkom.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rwrjgnjk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cuclxcbr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hrjqofak.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3caejxepz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fukyirlm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3anjokcdx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yxzzbxnt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nwrqkfqy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vseidfrc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gtvazsxu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ewfmzdzt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sirtfvpk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3eotspoje.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cvjlowux.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ntjdccof.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3erenmydi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nvxjuvof.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fqbzzoqg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jsofrnix.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3efqxyyjt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jcmmueah.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wfwqrpgc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3awruuaba.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lzzkaaox.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fffgcmfw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ymivhwze.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfwqiaxu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dndrtdqz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3osvfproi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkfrxhhf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vdovtzzj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ckruhdqv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3inqpwdsr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jrkgitcc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xruozlwx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lbjuootf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3auffpvqn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uolyiesu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ywkynuzc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3bdgcbzle.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vchxpdyd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vxhpqjha.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fnmzeylt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qebphwyn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jeihsqnc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gczbwdxw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xjgwvrbo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3psnzvnmm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kvmtbfgd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3chovakkh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ppvputcm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3djmagwhl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zzpzfbzn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cokjxgvv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rrluxmtj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dxkvhvdu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zvlhbzrm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ktpoiauh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3duoovnya.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cbyonipr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cvtgznhd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3egbacrei.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kcenfgwr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vkpksele.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lzetfeac.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cdlpxgnv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jmuqjpbh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tcmbifus.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qlobjbgb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3uvrnkdka.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ufotnnsj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rnqtlydo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lvvtvfns.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fberqico.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kisagbcd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hfncpkmw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gqtxiwxd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yfnnverb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kqodozen.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kabqsszk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dwsuvfzy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vrogtrux.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lvcvkskh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3isxlbvcw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yrgngyuh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3omkrpfaa.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fovmlpsv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hdyhbxle.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fawnndfa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dzgatjvd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kowunzle.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqdshgz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bxnoyjvb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qiqairqy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xspcwlfi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekdwfvhr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nyunowzz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3frxrujmb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lhtbrikq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aghhjsun.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npximjib.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nkyettgs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xftfhyet.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dllkdpit.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nxisomkh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ukxwnrum.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fkzqqzkr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lmqjtmum.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vipkcdsv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zjyxfrjg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ewlgjksh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3pkbdvkat.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vhdbdnoz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vkcpxvlj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lsnftpzq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gsmgilnu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3urnjajzy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ofgahiql.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wcfrkpxp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3skalhese.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3isjflqdt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3inwbuquv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3exsmmrdu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zzuajsnw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lxskhsij.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3suhrstrv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tpgzliqr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3asqxaygt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vwggvhlb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkdsoty.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dxfrrbvn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rfznjkwi.html


<!-- 参考信息 -->