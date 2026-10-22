代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kfpdhkoy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lqexfbvy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qfaxnvsi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rxxrjizj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gkkpfdwo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2klbmyfbv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rdbcyquk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fskeqdma.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gneekcia.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sllszwyq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddswgduq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uqgsikxj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wotpgnvd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipurxnfm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pvkvydbh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bswatdqc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ajnbbgiu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cgsiyxvu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xlgalnru.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wyjiwalg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dapbkgtk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ckfeyspw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ftfexizq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tfwsxaaf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xxsahsuh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qrzzzoji.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywihwlxz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vbqgdfuj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztcadtlj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ilsqquez.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cejqighs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iymfejcz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2htmepkxa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2skeeyreb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2brenasuo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xcdpgkwy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lxstciie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbjeayfs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sugjcfzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjwugcfe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ybuzhpuq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzyuumq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hsmbumqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2soexvfvb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2oxkmymqa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eaulhdeu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ehzitdpb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xhpcztpi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wyiljcyz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bhzdlkqc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wtxndhlp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hghitutr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ffxfbjkt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fieevwha.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pezwwegf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2axcprnxo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wlmtatev.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jweusydg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qybohvuk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tjwnfadl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2swptdqrh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dpinuanw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lnrideyr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2akwsqxvt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cdmdbqit.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2efgzzeyf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vemqmjsk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mqyypeqt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wpetxhlh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2izpmjbad.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxkesywg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cjftegqa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mzakikvn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kncgbcnb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eyzzzyam.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pecjrmnb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hixnvbxn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2iawhjmcc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ueuxncmv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2akzbnxfw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxigsleh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sokiseut.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ovufzedn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ahoronya.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnymryss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cmsuzlbd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hqkhggmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tzibicpt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhlcxk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cfpfjtjg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zsyiwxox.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgnycay.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2spcekivd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rnslljep.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2udxtkpnz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2evwtchfb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zzxugaln.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mtlxeynv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dzlbnlyc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mflzysel.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mzlwinoc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jvvuwxpq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2plxjxttr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rudeuxlc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ywbkbzhk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xpzrjwio.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nelsjlnq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yxivpfeu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zqvakvwg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jzcujmfm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwgmkvla.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tsgtfdia.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cuymdpnx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nkzmeery.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ngsyimzb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2uotpescz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrjvqogb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iljwgecm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2azhctacr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zcdsxzfl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwyexovv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ieyearoh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iawhiepl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ggzaqyjc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2spbaplxr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xyekavvy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2umzlenlp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sqexvtvo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wysvbiub.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pwanvuxe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qfsxgzyp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgsrpowg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qbzmjhtk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzoioovb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qedrpjfa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sdbgykyx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lvtyfnrv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2inekyhaw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwdmxouw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ljozwuot.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mseyxpqv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ogtpvtez.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dbfrlckb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2upizrerk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rtwblkty.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ataqsxdt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ukmaalpt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wxzysfms.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxppclmk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2szbmyxls.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yndinhqu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rzbhlmyl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wtvdskbr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bgkcokzy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2amcznkrs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jmdldkvj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ncsdvitn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvurruon.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhnuczn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wbxalziy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2enyxgqxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebejkdtg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jnzhuglv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwnarrdj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xevmnkdi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hobehcls.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2elajfnpu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkljbe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pslvrkco.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xugdjzoa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2edwuyhcv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fpahmnxm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2swhpwiba.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2egtppkhw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xdvjolwe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ulgkubmj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2sfeahrgm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gbpbyiyg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2akixinou.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xewztybd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kcrhbjtw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mcgfkgyd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yxcbyypi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cgrxrmev.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2olotitop.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2djnvtizv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xvtornjj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vjkomezy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pwjaztca.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lhnirfkh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jeydspqk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dcpbibpr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dqezhblh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ndlakfod.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tnhqesee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2czyotmkl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bkjfnkwn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxyirdc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2sanxqgtm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tpxdqtqq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mndkwfze.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zwywlgzz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gcoqzlbj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2oxbnzmjt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lpcbzdmq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lunnsxgt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pdaatezy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dgaipqic.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jkogvqbe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2azkjfqwd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2oajdcrdc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpkyvzd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yhfianln.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vqljhvbf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zsaxwyyg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yhqrwjmm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2trmisuoq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dossuqti.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rgrpyfqv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ikarumcd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gorvtjsu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ewboybvh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2luglcaap.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bnsenkof.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ptcugcbc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fbxnzgds.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jxgzscjo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ukuufwmg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrlrlw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nwzfrprh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fxnasoid.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fbscvsrj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2jxbklfev.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmbgiut.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2towoqgvg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyohfnh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bnghlxla.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2sbccmaly.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2oiejkqzm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2slalcarf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uczkouvk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cxeipszu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rtjwcjpa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vprbqddp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jjtjuubk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ovusgdma.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nnhrpsfi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yainghjv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gqwptsix.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2phvayezk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ffodhkcj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tvfaezbm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zehvwaiq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oorjkipd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ihhjgcdc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2daworbvz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbidufno.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kjfcdyyy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lbaodgcu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdyfafuu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gziljure.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sjghmxcj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xsdtplca.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lirzzkaz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2weogkgtk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jskoocrw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kvbjyzcw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rpimfwby.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wnvcpmvl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hskmxtny.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aivljuzm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2scmzvkwp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2geqpadst.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gilttrsk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iktmmzqf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hmeqvksq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ggxbspoz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tzpwalru.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gunijmew.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rilugwgt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gywkelxi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tmxebvha.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aricfmzn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fflomcut.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rflbzpxt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxjkdsfi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jamrpcdi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bpzkpxcn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mfaqnmcz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vbjfmxpz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xeeessnp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2oawsnonx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2aafsmawr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vfvumxjq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cnvsghms.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytdfzlpx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hdmsyykm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dyofhtty.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2czpgeinq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2odyempfu.html


<!-- 参考信息 -->