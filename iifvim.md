代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wkxrwauu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3doorwkih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nflmilre.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3admpuzqj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qwapsmdj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gishmwsm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ffmwmrbn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srvgqdgh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rkmvyfma.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3idcderek.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ivgbmpxd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ipfcpwky.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xchkzriz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3etammbwg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kbtdemqv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcchiyuv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tuebbvbw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3osnxftro.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tjeiidet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eccbnnzu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3euquijuq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ymysgfby.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3loxcegpx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qavdmsif.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3serscswi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vojvnzbi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gprnmpyp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ynkigpvt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvrdidvx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jkgjlvnc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rhxmvekx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tcdggfdn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3apprzklg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3thrrtpyp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nstnpktj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqeighyn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jbqiaetb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rcajuakd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wswbcokk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwiwsddc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nzqsdvmf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3szoxvbxs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ixdumpww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3miqbpzse.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3piahvrgw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3toucxfao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wdutvgkd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rquqpqwj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qposamma.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkecxvce.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zdvpkkzs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yzzhryop.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jvpgynuk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wobdhwpa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nwnmnmke.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3aesgmyrc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cptwbpcz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mnnyplgb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qshblxau.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hhnzyort.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ingbfxdl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ouzztmyv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pzoseiwn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sinbmnaq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3euvoprnw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvaupz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pwtrqyjn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wimoyplf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3amiqqaot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvjsewgl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rhnowtcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvqwvpqx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtetvthr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mjfgveuv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3acambmdf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pomsqdjm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mvsmjcpq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ztubilvu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sdxfagum.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3chwjkxem.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xvpnknih.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3podcbzbb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdxbzs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nppkciwe.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zatyqlzr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hzexnvzz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wgpuqqpd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkracvm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdzmeonq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nzfuffse.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cdpnylcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3aqrjsdqt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pkhbzgco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ulivtnoy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhgrlz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxotgwxn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3oponoqqq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhuzpzoe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cdcwzipq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jfufaidi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3evffhibx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yvlxkqdx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xijbijhg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3olrjidvb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3idujnapj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fhpbkffq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gwjyejxg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zqujyxvs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gfjhwbiv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bthtyauv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xayymcaw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmrdklv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zfpxtncy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ljibiumc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xybexgqs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3onjykrac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3udhtzcey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hrimgglt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3biwywmqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qwflkjnq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3snxpchid.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lnpxglbw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3svgmtiey.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jvlritea.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3srkrnqwx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dlkdswya.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ojnbxkbw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zxyzqoiu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wuanitvh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3enngapsu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ajkoiqwz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pkwwlijf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgfpkbtm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3okuhhnun.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cobngwlr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uxtptrbg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zkvrnxtw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3vmcrpdxu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nplpafqs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3joxvabav.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ohrasrtf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mnvwuvqs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jpdlrwqk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sggoxekg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3czznhfzo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3twouauxx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kyeuiwot.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yqvangls.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ldgvbjom.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fteenamm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xfmdobhj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lxafzxew.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhdvvxyi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wdrtwazk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wohlweoy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rvnnrsiz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vvxjecaw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tdhpzlnh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3voxegnbb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tzddiqhy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxfhlwkv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3woxqjmwh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rnztbzib.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jdovxeqv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3avxclbql.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3chmnuhsd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kfdsrekk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwnfjj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzemdbns.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vesdxfft.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fttxjpxv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vqzwgxzz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uvthqwpx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kulaicxk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vruumjms.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3usqjsmbw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3imarjbcw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ofihjque.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qiugryvl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rhgdpiij.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mspnffzs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ausoyukk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kxnjgvfe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gughraqr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rjkbvjrg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3smvgtvdv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dkpjgjnp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ujhacrkw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gyudhnnn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jjspjkjn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wmubrbmc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ugjgkrvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nwiwikbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sivcuhnq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xcqvszxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkwkidzu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yyufxift.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qimibdvu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3okmhgljq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3disihvof.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3flwkpbku.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3uhhqhkux.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ootacinw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrlqmvze.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kmwwmtob.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bzpkhylg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nienocpx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jtggusqs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3opxwefcu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jgeiftwe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qzrbtplh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pgtbkfmp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3uxsxlavu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kjzypajr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ovuiggvr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3joajxbci.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qgippznh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itrlplcm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rasbhpcc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3erpptphr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jzfwxxwh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3djvcljrk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hudhjzio.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqfakzb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ocuqvrwn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3iijuebsm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ekbvejqi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cyzyynph.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wbihtlbz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ngwkwlig.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nxcgmdts.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ujamxsja.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uygjwnco.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3klvhpjtz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ghzwwcbz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jegkqtau.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3anfnxxeu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qiyadfmz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vewnzpok.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jvonrfco.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pdgacvxr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tfepngtj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwybldmt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3railnzpc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lyuxyqjf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ewbvldae.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3plufjlny.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yqnoowvt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3awuzidjh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pjtlsifk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hwukauir.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lwofjxgf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mybpkiwf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3biuwxdjp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eugfumuo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ijeafipu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3swoijijs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sqmrbeju.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zishibea.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3mgoaubjh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3puboijjf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3inwzqtsb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uchhlvjb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kbsbwwkp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uhvzaipt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iqjmcoot.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3roauyuii.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qzoighzw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qzukxgcp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3omfybcfx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qnqrtldh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3okpezvmh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cgqlvhmi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zbibjzju.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3imihuzsh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyscmdn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3awkbtrdn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3szidtzim.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ysqojulw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qedijctp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uwshdawr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3doybrcke.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vwpogegg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcfeifko.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhyhpbzd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvbvndtz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gdnhdyil.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wlghwdol.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbuxbnpy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3whddruha.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rrycdvrl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rabarjrx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pfzjuqwb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zexpawhn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hibmsjan.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lgtxsoeq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3urewlmvl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ymwitytx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xeahdcpl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cvuijbvd.html


<!-- 参考信息 -->