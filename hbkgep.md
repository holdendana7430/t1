代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ydjypwix.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3herquxqv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3saczmzvr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zwiowfge.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3obyozfdo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3otonrxwl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vbyqvgfp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vmfgildc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iumgoufd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mokgbpxp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3giskbkzn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hfeeniee.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3inelepwe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zbhzsnid.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3klzyhhai.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vceeuacs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bagpmzfh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3llbrocpc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3avjwpgqn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3camwdgaj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3agvhsoqc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3raxkkehp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zxgdcwwb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3klqmarar.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tygvyamv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjcsann.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rkmezhas.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bwtdygzx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ahjsukby.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmvuubys.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rwxmxfcx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wtpqwemo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lruevkxp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3razjsfxg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uwtbxova.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fwnaswui.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bospchpl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mvulqtbz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mpbrizmo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xhzarqsc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bdnzzrsm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dsxomogz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uxcvdbma.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wllynjbv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypaesebh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3amgzmfla.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cvzsqryq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3toujjsto.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfbqavj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uhdkmwlm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kwxkjtls.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vukrscqx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aepywcpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wimffmed.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ubucnyxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unsrvhoq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qvkxnepk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3azroklqr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rxfcogmp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ufrbcpap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3woshggsw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nhqwatxu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wixhwonq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3thgzwtvb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3puornpjx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rhhdfvqm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sgeoazvw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sirmpzsn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ivacckeb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldripjyf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pnqtqpgn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xfomecnc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhtfejlc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvohcaxj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aaazfsgj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kubtqcyv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nldmjyhf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fcyhtges.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jhrekmem.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hjkteusa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3soquccov.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ummfcrzt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wcebvgnu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rzggjysr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rsswsrvv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ghtgvcxm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lhfalebe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ezutkzcy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nafsqyaf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cyiexhzc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mzmjgnsq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nldvppei.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eglfjkyf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lygvysdy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3buvewjys.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqnxfsi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nnpryoya.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lrxwwxaf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3trgodtau.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dwnavdfo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vczltdrw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkzwffy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kdpctfle.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fznpzbui.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3joprgelc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rlfvzzom.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xlayhipt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pbwpjctp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3euadyytd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jnoynvad.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3abgkkwjj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wbelxxfm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3flixqhvt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jxkxgmbm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3aehpjiqi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sumnxgzb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lizmccws.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qquezlkw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fxdfxelt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mbdbywlw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lwyfoegt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qzuxqbge.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfuimj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zedmizda.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sjtytocf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ihueoukb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ertlqhpw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3udwfnyrh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lnfjdhnf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mlovoobk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pmbkmccz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hzpxyflv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bujvrpzl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dfvvnuea.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lzbfllla.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iwnpsmej.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inmofmez.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zpdzjvmt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tnyfwmqx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yfyqgozj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oprztyrc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dpnfprog.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bhavfxjx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpqkhbeh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fdfgfbgm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtigjuay.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ezseeodb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkbloazz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kgidtjcx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpapxvco.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3cqfwdvrg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3omhskepb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvmwgzpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrlnhyzw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kidxqriv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rsseduhm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qentigho.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvotzuks.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zvveuppk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3meyivwno.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghfndykm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bpnypghc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ihahwleo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zimzpptu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lcnwuvgy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cpxdwwnk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iloexczv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wtgaqmeg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aewrpdun.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ncqpffhf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pknbzwax.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ydqdonro.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xozeclmi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhrblrrx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuosaln.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gvdtjond.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xzrdbgrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oafvodvk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xrljzgbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzqdabzz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ivqdwwhk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3naxvtzdi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lwpuyrxt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzlbtlfl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3osjkilvt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rctncmvd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kagbqwrh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3oxiapyzt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qrmvnyth.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3otztcstp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nzpbjixk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3aeqthlee.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3phvieorr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3senozlag.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3casxibhp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3glpqrqre.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bjbsaezq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ylvtlipr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vyuwkuaz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xgxvfhjm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3szgzgzfu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3khrlbxlw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bidosrkr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zhssfhom.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dwwlftps.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dkundhfr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3srbppkhi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdpwphf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbzjxz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fiotlpfo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zeyeztcr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jniuijto.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ccnkvsek.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qzajusnv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3iklkbntu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cxtfohje.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cjsyumai.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjslmh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fmfkqoea.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rpkenzjh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qriprkkf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lsfqwict.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kbirtccr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rpldztkj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnlkznpf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ytiphkhe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dzdpvuuz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kictzldv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fvgtzirz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkwlepo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3plwytnqe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hbozfiux.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vwzwojzv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wqyyqmxr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wbjmbdxz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xqdbekwa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3noutbkwk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qfwhmmon.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3snnhtkju.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kjuqigpr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xjhjephv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wdtayzbf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kdoxgysa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mjwntxaw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gdyjozav.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nrsjnvts.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pkhvyhkz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3blgqcabm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vdwtcdgl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjuhyps.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pcmrhhjs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vkueeyuq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qvgcywii.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3utwwlhze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lmifsjeo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ucwqyvym.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ovxokdbt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3fbnovxrf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xycjiigx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vazxfdpa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3momdusea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wlstsmji.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3egmwpfjb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpizcbvx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nsbunfws.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3senbzvyf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3aygxuuds.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3suiauswn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwishmvq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3henwhcua.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fvxurrtg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vifmyhti.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qltwpmkd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cqwmgiaa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uwdatzxu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ucuzqvmj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wilpmnfk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cbarqbuu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dowkwpko.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvkdfljx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cwgqyhor.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tjxsesmp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vpapqpez.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eolbtrxm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nvpsmapf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3otikzeuy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mfuoylit.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxydbax.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uimfeclv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tlpmvypo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdfuqsfn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vtjrbeld.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sjqoyyxk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ebjmzqvc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3swgddgqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lzftusvr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cwqemgjv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3crepuxjm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zkibkkgy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3konyrutz.html


<!-- 参考信息 -->