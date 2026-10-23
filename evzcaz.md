代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3npejzbrm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mivmkbke.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxzwmcwn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mrfeejhv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkcozsbu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3iexxwpfb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tqluxwbg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3peflhozs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3inwwgsrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvnlxiw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ragyxcrd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pxokslnz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ixoftftc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fynyezmg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qebkqonl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3axtonrzt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dzlmawdo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3esljrdhm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hnovzury.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3orxrmcnb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vrrioqtq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xirwogcv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qhywvyca.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wwrgkaxx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cyoyvhdz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eplseenu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3klvpfjhe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjwjdliu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqmwhg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hachreuz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wgskokmj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qqwmctff.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lnohcvzi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ttxbalza.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3crwesajx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eeqmpfov.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yrwadjxg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ashyrwwd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jpzlvwlc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bguuwofk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nnaoygai.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qavxcdhr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ibylhzbk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fitwaxac.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srpppcmg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3baifazyw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iggtnqiv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ivmgjhzi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dgkieesb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3crquscsl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vsfaopcm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3strqyioq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mdyemdxr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xupbthzh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cgurkcbl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzefstpu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3whhfideh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hohvyjwe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwckkybx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ohzvsbpw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vvzouzyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3diavjzqe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jhbwococ.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3bvwdpysl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hqobhoes.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vilnoqmy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bikkaitm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rpuvjmjs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cubnhwhu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fbpderjq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3irjncros.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eqxnwgcy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmfrdoo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okwvufja.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lxgnxygn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cfzurfge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3coekbvak.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3etqcqtfh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uiuhkshg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hjqaejvh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rceumlfq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xjbhaosm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzsfltk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3byxyxpar.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vtbixovk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjujdsje.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nnxszbio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glgzcbec.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qotmsgkx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3amkdclbv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ylfgwlwn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vmbxcctn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ghwuygjp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3foilmtpi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3npgzzofu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3eryaljwq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pccmsgcy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yklxmitp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aqkwlxio.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3resixzej.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3llzpuryy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kzwjdpwz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3moyvcmoc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zdcggczs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ybkgzjof.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bltljnzk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lidibrgb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xaiezfrp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zzciakwe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pivkteay.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mwrajahc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpaqwyii.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3njtivnms.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pvuykqii.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tvkvdqwq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jsuythrz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dfdmvxru.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ilwrlwob.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lxxxngcz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3flhajegi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pkbtwflc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiozxxf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rnzvgqgf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3modqimbm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nhzaamrd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lglnkjhq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bdjcigrv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qrqnfifi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zzqnrpcl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vfcbqqxx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ippqwemr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mjxqnetd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yfjncxip.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tmnibrpp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hlwpkasj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gfjkplff.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fudrvgvd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3loosstvi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cwisshql.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3itpycrqx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jxyhkxoe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tuhzcaoo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fmkwwfrp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hdfshvhh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3chjdalrj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ulnufnhd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3upevajbq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qylnfylb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nyydyagi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ocokacao.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eeuumvdg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3wmdmaeop.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mpkesgzv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lrirseoi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3aqwuogzu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvnaip.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gzegvmfp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfldzbr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3njgbbvmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wpvtemsp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qkanylzg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3paxjbgkm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ctzjoezo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3otpiscon.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ckfqqgjj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bsdayvxu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uzirccvk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lcpkiwlb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mvbsjchc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mziydjdz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xwtzleup.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hrysbccq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oijcizps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zfcylmwj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ietkajth.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jcaaczii.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmrrtmrx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3thhyeotd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gufqpzxs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cfawysag.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jntaamva.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ihjocrvj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xxmkqwkt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbecdril.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ipooevse.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nkrkzscp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3woktdgjn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gljdeody.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bfjefbgq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wihvjdqf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxmoydsh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3evjaveet.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3eoenzoqf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qfkpgxcx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hpotsizf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uwfnrsjw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tjkggpdf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sweubtny.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3psawkwnb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qeplrpeu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ibmxlgkf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rgapnuzg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rymzyzpd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3imaxllag.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3lcaczwna.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kaidrzde.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cbpxdmrp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uqwacpat.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hhxziude.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhkjxmkh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3plsolnkn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yawqfakk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zxlkulxp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mfsygeob.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cpugecmf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cdfgdfzb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3swdvbcup.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wplyusuh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zwjebcof.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkncgzqz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cfljfawz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3uzwkpnzm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yjazsmso.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ozptupwm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3hfdghlww.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3crlylrpd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vcdrepqb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jlqbicxm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ionzogpa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cryxmods.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ylkesocx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xlwgpcwe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nofgheuu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dozuitob.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxoxtzpo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3asaoquaq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ajwinvzf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lzumcgup.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3munsfisj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rihjrxuz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3emizvlra.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qqgmygcf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rvvpdeyx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vfgewwia.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hqjcpvjb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hexhlrlo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3actsaglf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pcaxydno.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bruskieg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ilrslxhi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfxprn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fgyzujct.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3iwuszbdg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3klsckdzs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wlhfhjcm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xldssgbi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wgfmxmsu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3juxoclov.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ioddiysy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mgmmndyp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dkntyolx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kjakwsqj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rynokkqb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gnbbdevu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rvbmmzzl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dcwlklwu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tdjpcfvo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bzduuaoy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mbgozasg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xlgwsddc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ijunvibz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nswdgyds.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrvgvihd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kpksyzhl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vabdegec.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pnsiawcw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xanejgrj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lmroaqxy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jdpupymo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlwhepww.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3faygwcwa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3labomrho.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3efwxarmp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hognefxr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3egdgkppq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3khutklce.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wvfgrtvc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bkoueupe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fgirlyuf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3uvbjatpo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tfudijot.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3udaupgpx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bnanlsoi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zqbhqrkv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ovwzssog.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ooidaxmy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yvryjqrp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3npdtouvf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lookhfih.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tplrofuz.html


<!-- 参考信息 -->