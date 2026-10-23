代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnljwjgi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3csjczutb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcqerhae.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hoerratg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rpjbptrk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3osoezqdx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3krwdofve.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3aaohpogi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gvimlovr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pixuibgx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ftdugnmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdgqqwfm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ymhgklyx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhengtzs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybzdizvr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3snsztvfm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gpquslwi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hmoqfbtq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hznxwecb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yznodviw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3perdtlpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rvdcbpjr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kylxbiwu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3umvinvhy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uewcnxvq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dwdmwxog.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kzquorfq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yglabxms.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fsaglfpb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jmhcytvz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygqncqag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vbmbnmgd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iwgdmmlk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kczaetvf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jqwyqyeh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3psjyfxip.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ajvckxlw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjjkyw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qakdwuey.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ycebiesw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3azhygfuh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pnzhrnbt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azdgtihi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkdofpvv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yhnszefy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3scugcoov.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vcenvdjz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rfzpjqsk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3krjjadxc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zatqvsxs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wtkbkehx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwcnmuy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3motwxzrn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zokaulws.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mssiyxqy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zibbkxdm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iloqnkmf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pvmeqqfx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gkrzlyrc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vqzuatuc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3aqheanlj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3brgqfuhr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ojkbdcih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dzczyvav.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qckicppk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3duoncnpx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jisfenkg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ygciienc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iywolqox.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ivvvgsdv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zzztjurd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nigpyoli.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jadymhfl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mwbheops.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tugzlwmi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwgbgzcq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vrrwetkd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bghpgofb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zkfoxonq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vwhjgijb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sufdwouf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nwnoicjm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3moiwykbk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lpbmadwq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cbbwszua.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qitxaune.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3afqtciwd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vtvnclxq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pwcjixai.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wpbrvoab.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ngkquivy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3thqzxqxz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tggllzrc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zwpqjbel.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qpskwnhi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rkrukzmf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zdhdnlcw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3muficsgt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3alooerkz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpdzpr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kjbrjhgy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gpnycncm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3phqtfayy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nltmopuu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3exjzlehg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3yaltbxyv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jwxeqyrv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sxizfwzx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iqtqwppi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhtpsum.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyqnjpiu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pucdxizh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eahjcgjz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xetxxoyz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fozjwxfu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3weuzxzpg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmuwgxpj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gfsvzykg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hbsdscyi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wffyqzhm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkuhpykg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ptodgojm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3avlzbytg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhjlkw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fhdgyuhw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qmqteykf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jjpflmvs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3opxwautz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dewnnyfs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wvorvgbn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ttomuxzf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hkuklsrv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rwnmnqkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maktkoef.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scijnlag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwlhvfvu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qivxrqjr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lfjrdwth.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zrsrijwf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lztgptar.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3splnzbej.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tkebzboy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jajwssvr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtzflz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fvlyfslt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rwovivfr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ygesrhxo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rmesnulz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jyptihwl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vbblpphj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nfwiunfb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ksgezaxq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qtorvwjm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jjojxzvu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sucxrpkv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fcoyuhtq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mxclvknf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3lltsvghb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wnftjjdg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voflyynm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vupgvzhy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbphvvt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dqrvitcg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lvdzayzi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3etegyksv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cmeszluw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tlifrsne.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpwdmud.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3adbpdkbs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qbqwyygk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3whinsmxn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yownyedp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lvzgkgar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3iwxkaxnv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ywixxhjc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkpzwbt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ypbjqedj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bwzfgudh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ypxfsuyz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nvhtbknd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqthimmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bmcfmwnq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mmbbbvxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kznbfhgn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ecvqdlye.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3aouunugg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ltayagrj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lnqqniyk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ykouqucw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wcenzalj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hkkfnxgd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bsmyxdlw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ffrcwoee.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3aagmsudf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3joyzlmzt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mrmvhqnt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cauxzchg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nmrmmpde.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3znvnnutj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ardcuyvk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cwprlltc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3iuomlpcd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wkzuyacm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jvkomfjm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pcmxgxut.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nagbfyax.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rfwsqmuu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mwraphzn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dngdtnhv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jblppmzu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3uargsytx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gomisqfw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3piualsua.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ejgduwsj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3irxleusk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3boisgbfh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ducjgyxu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kxcrjqst.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3imqrkdid.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pglmwbli.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mxiieeld.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3afxooyfv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ykpgnzqo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ouzlssbn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ljzqfolg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxvtwqpc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmlijzed.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3crrxkjge.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qsqvoqwf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3oxsjttdg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bayardvi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hzmzqdbm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ujxnenyp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3drxqzgpl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3evcofbof.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qvadobec.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hypqqjqi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dthlmvrf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kshsmgql.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ewwftrty.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kvfiizxz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tattyysh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hvoxfjhs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sekalckn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kfdgjrlw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rkotuvrz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pddhyftq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bydyktbv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uanveizq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3iihiaarj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3munysxnz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghbgnyhy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dcvxvahf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qcrqxnjn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gjjoykdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3paxnbubf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hrgdhiik.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yopwehrv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xycvfggm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hpjatyoo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3znyiibzj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ptupgdca.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hpjrlyan.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qgujzetc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zmqqrqtq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vikzxidq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bfmivtls.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gwvlgbtk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3idtckegb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qxlrjaqf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jcfsphdp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kqadervy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wiqhttkz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3axqjtoyp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zymbqvcz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dmngtnqp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xpxtkplf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jgbrujix.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kifxvfku.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kvbjqaaa.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ysxcmfgi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jtoduikh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iujybnoq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3aiqntvqs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3bkmcnqrh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xasxxyiv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wdtedtfb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3cjbbahev.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3paiepcyg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mbyxpumj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kjtyfbkn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ggflbcfv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lofofmdb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bolwllbu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ofgrskrf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fhmurkhs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3indwhcpp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dsbkbzyt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ldqztnvi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nexjxnkt.html


<!-- 参考信息 -->