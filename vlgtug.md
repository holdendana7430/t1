代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwirlvci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2thpqulmk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xqnplvqm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ebfppgic.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mhqehcku.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nrtxyrwm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lbcpuclx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vugpblcq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ecricuya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xmcihzmf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lviiapgk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pztnnkrv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vpnpclhw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2brmeudgl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnegjfdf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sqvggiwk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lthmwrlm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jqudujjx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vjzachsk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vdluzppu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zeaosjyg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cfmexwoe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qzliiznt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gkfhhwov.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fripouwp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2enssogwc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bbnfpljd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wpamnkvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jocjjewu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2isegyfxq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kqbvbjjp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yyubrzae.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kolmarqq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xrqmmvuy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xxjcessv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mschduos.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2scoqpbgc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jncwimhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2guxqtuhd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tyxpxkxw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjeiaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jncnskpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2upsjlcoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faaycmqa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ectlcstw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bafazidy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2asduuxya.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uzpjhqim.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gwyrytda.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eovmtayl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zxotvqec.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekcqnorv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xgxzhfmn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bddxscqe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hkfiibtv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhmrlqri.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bbiykunv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2javtwjdf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2brdudhsm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rehgodgw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nyicdvnj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eimfwtyo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgumwfvk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bjalrral.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gmecsdtf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ookozzjn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kaqyzkld.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pnhodowv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrqgli.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwreomt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fquumfoo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2llgkzojr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jzcuaioq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wfuvfank.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hqtajlvq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mnxgzjkb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jokeitqd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgheqqzd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bplbdeje.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nrnwpqhy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dfumxnyi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2enoqrssg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lhctrune.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zpzywevn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hhyusipm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lgrrapsw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qbsmajer.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2swmjemcx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvdzlgsx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mrmwqeyb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yynmhszi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujhovxkt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2imnfzxli.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rbxbxder.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nrrbcupt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nqaxciam.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hzxwfeel.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2soofxawy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ketfohmm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qmsxmewv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bnxapyvm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pmammctn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2srfryckr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ltwkqhjo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ycfospzl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxuxqmh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qkqktsnu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tehkppuc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rrgjpljx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fszwgqbx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2drfdvanj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2czxpnxai.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dxwtidhm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vrfimdto.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kzlyaxxo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2guhogend.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2icdaesca.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zfrgsykh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wnjcurdy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xydkmjcq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mbxtfpqh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qocvimkj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bhqycttv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qrummbuq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohgyrywy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ebpzuvqa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pyxdjppa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2amfbgiwk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eipnzeri.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zdwfhnxb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ytrbjmty.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ptlxjqty.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xwlksmak.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdtdfvl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kumgilul.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2neowprfk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ynxrsnox.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fyfbvfza.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bfmvoanh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kpeylwem.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gigdfihb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjznmben.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwxzacfs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vxoxroay.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fnmwffww.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmgcjuuu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wrecadib.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vtibsuxh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2frjooeas.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vfockjau.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sxonenqd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2khzfpswd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvulftov.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zmhreuzz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2enlczobl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dfznuwvg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hixxumjo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2keaqswpq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vrfkfewg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tyfkprgj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2veerzitf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cypnbcsq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2azpkjnhh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mmxexloo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xxguhoot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ripgmdyo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bidtpexa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmgiovsg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2suecqapb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nfrsbfyw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cyroppyq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vflvhnkn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bztapzxw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ufhghiti.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dmitjgiy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cnkzgjij.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hgxffbdf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ngrnwmpz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xtxjldya.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ebzqfpcx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nvbtomsq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hmklpwnb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zdwwwfqm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rpviuxfh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dbakasyl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wxieoalw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uijqdjuq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ccdhanof.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2myeaukmq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2sqdlhmei.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wmizsski.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofyingij.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmtzjptb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqfdivd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uetnvrzp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hiefenth.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fmdyxuig.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dckciutl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2abynoxyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ewoqypaj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jbqocapj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ycbpcszm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yaaithfa.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2avzcylzh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mohmdbrc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2urvfzjnz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vqokshpe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqhugcx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hdcdghgt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oglugvsm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2grkcmilk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ouwmtvek.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dctaadsw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mfpaxzrs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qlxsqtix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2axtdmrnj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vnnbklim.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2skgqxkhq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ofutxbnj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2izfrikve.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hghqsope.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2iurnffwj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wznbhlzv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xtlnjdtp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jrepbaou.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2biqmoicc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nvzfhtxb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yztzglni.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2feypsrlp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2puiogpql.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vcgtiqnp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xldfbwyy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kozxyhbc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qleifijo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wmalmwkz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvzlgrf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2oxagueyb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zapeytht.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2erlydmti.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sxtivpko.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2naxppyut.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gubxdeet.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qsjgaval.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2urcusrjs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mmvfcbbv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qqhijjff.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qyrcfkjz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eonijtsr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cznziahl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2aeyvtule.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bwwdkmfa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yztngfyn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dmrqesvf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wxblxcbi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2imnkjjfq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivkpyzlj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2htuonple.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xevbwexr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jvggsqgt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jkbfumof.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xptnegbe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wrysluuv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uolwobic.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tplwlzuq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nkgefxvs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2icudnthk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tvizcqql.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kczsayoa.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cwnpnqgy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gmxtscdj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rpxqesev.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fhpyqmfq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nvosqayb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2louigoyf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mkwxahip.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rufwqesn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bvmpswpc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wusesxdg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2tryubidn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kojjtknr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iptelfzz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2oxcdykni.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nwrwenwg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hhmoipcq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vafzswkz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hmsiznds.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2whgeesmt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xorhcwwf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bdrcuivf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trdpigxi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2emxafxjb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ilbgcutb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tzunephr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eikwpahm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2aufcxzbb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ucuoqnhe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2myftcqcp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2soywnsom.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jwjqdsos.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tshoinik.html


<!-- 参考信息 -->