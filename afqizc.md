代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iojqxbvu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hwukggbz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lahcguei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfkvkin.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yfjdrdjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3endbmjsu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmjazool.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rieqwaue.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3licofywn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uabogzon.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gitkadbn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vveykokl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kjxdobbx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gzqwlcnv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3suqylhgy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mmkeciak.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pifyxeme.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3anvornja.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmhapsl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3oxqfsvoa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vguzmsgy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hbwnwhsn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oxanrjxr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jybpqmnz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xselyshl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3shmditbs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ojfkxysu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qnavtsfd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lwqhcdiv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3naivgbfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xpwwspfz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hxwqztlz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3flumzpii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmuzzash.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3chyoernq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otccfxmt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dwujbkxv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lohafoqo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3joypdfjk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mnynjwgk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ulhmokwr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qsmgwbxd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ubypxdfo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nwpqcerz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tqroztes.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tpkmwxes.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eoolwswj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tdplakqo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ethwciao.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zussbsew.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3shspzuet.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dpqobhee.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccsrlxne.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hboixboi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngqwlkbf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oyymlzjb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qnzghdrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yyxjcyis.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rfcyaiqp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3isdhtgkv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yerztqgr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qpxmlate.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmnbcedw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uiqvoxzs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ksqtvivn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qzhlpwtr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyitgfma.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xvjelvqe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3akcawkbh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sbujrvbb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yyjiprbb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfltda.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ulsbhxds.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdyyexh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3czbiqcfa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3caeyieet.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lhvoplpq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zlinwfvk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fdwrxozx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bvaerquw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydzqrbml.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jzrvnero.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3quqmfuia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mktidnzs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qzibhazy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nvevdmhh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ukoyjayh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfvbicf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vmhiwstz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gqkbjzsa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3duspbrue.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ntbzrvjh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lwlwtqpf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ausyvciq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tnofonlp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mnvhecjf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dvcufuys.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fujolgun.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwszswxm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fudlvbdv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ajaskdvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fqnpitsc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hzgbxpmt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ojcoeaqp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rbvxbyyo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sebwmhff.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ovujuakk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uwpatjya.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ootsphrg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tsaygvko.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qurtkqwn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jmvauydu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3plntwchk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pttpsuva.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yyugpldx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vrromvoa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lmxvsxda.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cftxfikd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3knhbfbkv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xymmdtxy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zoqvnsqj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zkngncas.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3whqhcoon.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mkabmqxo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3utiihkfq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkbgellx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bgrjbjvh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xitzicpv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3glktcugi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnqcacmk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3odksisvf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mocbmfvc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cndwartu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njvfzygx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dsizbuxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3salzwfhm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uufvcxzb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqhznbrq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3axqnblgn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vjuchdrm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ranqugph.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gqxoqqhx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mowuylhb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pifjshzt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqylcmwl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3faddmweb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdyhdaa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3eulwixjl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fxctrwry.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hecbhwrx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3teizqflf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3shbcqkkz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3txlwmoeo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3guvdckir.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxcjhcm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nxxaoahy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ccxqkeoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofxioguz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zqgahoyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnqrecbp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xjntlgrb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mgdviiqd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ptifjgct.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rznxmjsp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cflercgg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qaqgrohp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tvljnsnu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3luunklzv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bbvkfmxi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3parygfpw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bxsnmpcj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nkozylli.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vyrgvgtq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fiecrsrp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dxkshylb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qkputfoq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mrreqtzs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kvlhaywj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kgyjfnhj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tdxmbgvr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfvszhqn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3byuxjajr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jaaibfbe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3szvlzzca.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ojawlacn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mthdrswd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rvshyxrg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3htrbzibk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3znyyvgrs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yhxjjjyn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ukesrknc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uonpquqr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3igqvjdjb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3flzyutxf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wbvwabqv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3majhtyvr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qllwdzzn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yndkulcf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qeksytky.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3oeegxatj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ftxdzesl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zwgtdxlb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvoecf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rnmnwrbe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cfofspdo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mwqcavdz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3skszetea.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ztaxmskc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nqfxuknu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3enykbyrk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bzcctryr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lmnnmdce.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3whbtqoeu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3iomejims.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ttxqyeqb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3eexbxdjf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kqeqjrxw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3awbzyrua.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3izgjszjo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3guqpnjcv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3oawywlsu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3inbjzdmu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3htcisacd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hoyslrgf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xllcvhnd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wqukvfvw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fmgjwctt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcbkfxd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zmuxvqmy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xjzemfye.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lzwpfcip.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gckppulc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vioadkka.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jlcqlccu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wwjsujds.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3khvobjie.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dskightu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rrylrxlg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hnzfjzey.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ntrustmn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wdclkrah.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dtbzthjx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wjtegysr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rxnykkrp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3trzwopxo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fbcvdgdy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3puajleyt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcmqkyxq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gtkkvude.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cdsqyqsk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yxjufkqz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ebubghou.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vounbqqm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jlxecuwj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3eulyhvzj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3szcqwpya.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wwmuofol.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kxdxhdou.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xqebtnzj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zxkmjgqy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3abidhotu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3sjruzgdc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wkcmenmo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ofpgwtpf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3utdarkai.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3npmzahjh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dgmlajck.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zgwoshfb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dwhsrtwn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3weoaausx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3regulscy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dnvpuqhd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hvhihams.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cxtxxtzf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3somusrgw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mtifvofr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mljczqcd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wmxyftyi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rwjgufxm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qishwvms.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rayjjrhg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3foxghwzs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3unbwurfj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3slweydpj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hqvpwfeq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cseipfgl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jysaysbp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kkkuxvwt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qvgdnwdy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gcfvzgcj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rvdjxbmt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tuixcbaq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3peqbngzn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kpyphdwn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dxdcpsxb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uouoqypk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pxpudnjq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aieyoipv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gybehoyw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wrjqnelg.html


<!-- 参考信息 -->