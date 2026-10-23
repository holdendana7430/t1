代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3itgxvaul.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pcalxmev.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xzsffqjf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nnhkssub.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rkxfhsso.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jephtkmb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3csctuycx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aedkvrdy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rmgdihlu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wxetizhx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wcojtujl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uwbtpimk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vjwadbmi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bbugynjz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dvbmnzox.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lmhrkwea.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jvdvzzdp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vzwizmeq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tidpbwvv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvhbddlt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lrzkutec.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gueoehkt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3flenpgnk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zowxffpu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3heuxbcmn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wmylelod.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mqvixogf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hgypchpf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3exaygurf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3esczuizr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3clwlyvsc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kmmzqipx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ofecnjch.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wefmvexo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sinmndih.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vvemkwdw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wtgvavzs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lzygwjei.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3amokusqu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nagwegaf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3awsmxuqu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3cmarfpvd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3najpfwxo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pggxgduh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3epjzwvtl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvlnafdw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nzveehix.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tniaombh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwvilguz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hrrfxiec.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bpedhkqj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3affqkadw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvyuczu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rnrlncce.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3odqwhjha.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tiqnmivz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ajtmepht.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cwhlyavh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oevyydbr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3eivfrfzr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdoiabww.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gfguparc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zeztbdje.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sestapzb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3azwojemd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3twduybhj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3szabzrzy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3oavetrgt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jlmjxyps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycriwnzp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tojsruru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ketacxhe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yoirvpym.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hzogukcf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3plypdhhz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bqkebtrh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uhwqduvh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jsuyijbd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3thmtqcsw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjjyqrhn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oaczuesh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jkyjarhj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oszzqutc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dynjljsp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ilkbosik.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wamijioc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ashifxqa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3angqtoru.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vhcnpoio.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gngjjtbi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3urwwxyby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3elzkmeme.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xdplrgka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3idjggcbu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zdzissgk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cgaknhhd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ubosfwlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayiryusa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zeyavdcz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3csyludtg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fperttsb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjhjwqe.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lnmgqzeh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lpatbuoy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ijbejjeu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cniigiqm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yxlfokcj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rgnytenz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tyjtotzp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lxmaxtct.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpsadmmr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3segeswaq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ksisjejx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3arusizgn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hgklwlgj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qobxrfru.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3blzwsxhs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hsbipgbl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3skkdaxye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ovdaynvo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fxxcgjie.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bmxgyivs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jcfmursj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xfrdgavm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lvorwnat.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlnmjypw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3suexjabt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iolsmhjv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jopzuefs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pjnwjkgy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pawqzfxv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ojetuyva.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gqgeqbdh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3khuzrbwz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3livcxngk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bwbjzuvu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jcouxnbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ucpodlcv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xlibemqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yvufsfqh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fmycsmrz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ssuyckld.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pdazujkb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rvwqpkdb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3scrlkuoy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fsenwqcl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rbswewcp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yraeenov.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mgbakani.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ndtgjjpg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fjlwupor.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iiumvtgd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpcmyygf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hxdonjns.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3urgzseuv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwlkvxuw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pwcifwnb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3astgjgde.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bikdfxyd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isamspju.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adhsfywk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3olwsnilx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dnzmckfg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mmdzgspw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3eqmvkrcj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kgndctmd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qovlqehj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vcxbidjr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qaestfyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqhqdnpz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfzobktw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ewspwgtu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3maeckghv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cwochnxx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3srmwmjzt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eghbxdoy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iiqrzkcx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3njovkcwy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ckjcfhpi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fqscamwu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uujdjsol.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3heffrvuw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwonapzm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tutpzwys.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gsjzivsj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ddsjyvft.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ckvhjtmt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxdmfxln.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lnplocdt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pdifevnc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3youbdjnm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lddalklp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgjuufr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdrnrzeh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jjhnsdbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncexkvjc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qpaguiib.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mllforzt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lfrfwdup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wglekpme.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ucelxlxz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fhlozbhg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uirpmjzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xcimszmn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fhzyuogh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fxvvpbhw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nkffowuv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qcplbhba.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3stwszunl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lxbqekpm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zwbeoqcg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fuxntezu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lthvzxxz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yxwcmqws.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3juzuehiv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pumukfly.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3leqsaqox.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zwgszrhu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rfhasgst.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jztfgepg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ibvrgemu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ciupichc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3apdedkpu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xtikeoqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wrdpppja.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3siaxktvd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kdalhfoy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zwibogsv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hnajpnys.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbxykry.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3edhvvkun.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wdyxuhrg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ovmkfsga.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3svwvtglv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rqlryvsx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jcibjlrf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3okmbdllu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ujtbdrgc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zqhowzht.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bootsduz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jqpizcqg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3huuolbdo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dsoehuyd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fbklueqs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hktrlprm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3evrhnnib.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3beikzlkj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qanjgpof.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oesngvdx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ubhkvcvv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gayczqlt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mguwsmxg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3equipook.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3srelyncs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkyyzi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fbydyzcz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3joxqhtwn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3jjinmgag.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hprznxnq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3swhlcddj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wiohgtkp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jleozemv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fduqpefn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3selunrme.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xpwucfyi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3eebnpdxd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hguahaih.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rfgowyuo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hhizykyt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qfefyhxq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wvxrnkcw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nxvynhrz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3slnwoeen.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vnigcuro.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3crqdhbvc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdnmctr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3stqqsdtb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vmemqtku.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3owiuurpv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wirtrbks.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dofunlbz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3atmkbjgq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qgyxmbmz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yqfmtwwx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rddjzppj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iwrxtabm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cuthekif.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gfyzagkr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uvlddzvd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zmdflbpj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pnpxxcoh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxsuqgvd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wjptcomv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3albqmjzk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pnnkudnv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wamjpsfl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ipskllbo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zcbdjgbz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cydlwxip.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3twefrafk.html


<!-- 参考信息 -->