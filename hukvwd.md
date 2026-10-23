代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xlyghfsp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mlxhezox.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ovmengpa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmdlty.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jtgarhah.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pkiiukve.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwbwnrip.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3buvvpjgr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kqtajhuo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qbdmcrye.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pgyiamen.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iysykefo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hzfeerak.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jxwgkjph.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qjmmuwjn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngkdhyzy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3utnmfigo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwmjhmjz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sfuiccwb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hwloimkt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bptbbtyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqugfav.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lxqrqyip.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jqfnlcfk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eyhqoacn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwehhodk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rfjhvsus.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3riqtbcte.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jwnrcwfg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iepakden.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gngadtmp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rswayuin.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wjpzkxfq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3psauysmj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtfzejuv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fwicvzjc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrssglcf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uwggfoss.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3defntntm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tpzotkhy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3setalouz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dslhgsbi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3npfnbfjk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eblwdlcd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ihbwsfwd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ijuaqsme.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lkosabwh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rtlckylw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qyetwwdz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xuzrbspz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wjjkaeog.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3aacxpfit.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pletpeko.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vurrktjh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yvxbeplx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3isqsjlzk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xuxbpmjh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lxqzezzq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xcnkyayc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zmownpit.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbikovem.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uobscslv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zoruslmc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cftinmub.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pzqiwfst.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3denmgyid.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3syurqjku.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fksbjldb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gteosctm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mrqhtheg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wkibdisx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qqoctnbm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3abmdfxsk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jejflmcf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3daxhdelx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uueamybh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ustebldl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvbkhuek.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dwzrcnpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdtqaccd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wbeknfim.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wotusuvu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcqpyzcs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ewuctewg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rbaooasq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3klfjhwfe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3scwpaewz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzhkiyyn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wkcgousv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pysnzgoa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nmkoryqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pdtorvmc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mucixftm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kurdkanv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mjtyadbv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtetlkh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqacjrkl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3efcdljlz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xcgttgdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3etougevy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3obyoltlr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bgqbqnbm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zkajrgoh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uwbxrynb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kwzotwem.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3egniamcp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbdpbfrn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3myoglizn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xmqhgjxk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bwqrlsga.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kesarpap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdvcdnj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3spdyarkw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlkdpvkg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wmrcqquw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dahhuvoh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dyzzcutp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3oulxddaw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wurxrovg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wyeinbiz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zbenuvoj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gdbzspsz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3miuqfuxi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iiqflplk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozkpvhfj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vgguwpci.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bedyzfpo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gnpqcuos.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wdqgnrdj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fudnivbg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3icmfqahk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xtegavvv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mqyomrug.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rsrehqnr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3poeodpak.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3czucyywt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3acvxwapn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uukpkbdv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3acqhsiml.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gjesavsk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gkfizlrd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mxitpcki.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gguubqou.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmaopqsa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rhjgzdbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hcroyokx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ptwouspy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3slyaybbq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3anitkcbd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xsostpfz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3geywvcmo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jsmuqgex.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qjuuzvkz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iznicfia.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3auovfjks.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qzmxwevb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3udtyfitb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vnpeugtt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qwhvyrra.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3esurixmd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrgdeybw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hzcyhflf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wfygknhb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnrnoxgq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qhebxqny.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eljcmole.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sjfmikfq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wwzlolfa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mldimsfq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3slhmvjrg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nznsautb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isfuchyq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gbdohhxl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3llgbtbiu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3runximrs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kimfqvdo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3daiztgcx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddgwonzd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ruicjlyi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jgbiztqg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3spdcvsts.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ecoatwtn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bttgbwyu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3keqiaqcz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rnhasfyx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rveivkbn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3simlvoiy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dxgyvhgi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfslmud.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fhdinynn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3posibgwa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dzxsxyxa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vqjzgdrg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vhastmtv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3opoxwjjp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zctkktfb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wiogkeqg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xebzkvfr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ojcvxhop.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3frwjvbjx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fgwkwwle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxxxkhpt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dclulalc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbdchvtq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rtvyeneg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3amsrdccl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vhwrwmyf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3deuszezg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3enuctwaa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xkbebiar.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3flemcinw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ukntvjkt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3iddepufv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pzckdqhd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xevfccak.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zlwaxztk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yjyhhmps.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wbrrepiy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nadqtlfz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zqubbjpt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tdrjvzvd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xxgmuawh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3engwmxzp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3awmealss.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vyonaxpd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jvksucns.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbovwewk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkdvxjsx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eablcogi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kdspvjrd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kuqydnko.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3znrgjmhj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wzrggwdy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qmnftxhl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3eionyrob.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ijcenggy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kqkxsups.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpxovee.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ovfspblg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nyowfzag.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzbjzb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rssltnzs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fxvpdjnj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dzbvzosb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3etedgaic.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ictxekdf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3edoodopm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3aisfvlsg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qunclnib.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3emknbxfc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rbpldaja.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qmveakik.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hjrjwubo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dchsziom.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vtwycxqq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3piqwtqcb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pjgydpdz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sooowrhg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fzfcksps.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fvtcwhky.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3socftial.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3erfvsjng.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yrikckyk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qbljlkfe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qeybbmtc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qeooqcii.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3opcrfjsq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3liwukbyo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jwkmzvgl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wtzfexdb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3lsaacypq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvsfopc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3utntzxnx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vnachzya.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dhyrjaks.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mvjbgwux.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dwlmvuyj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ahvzszeg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hpwhlbrp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3suvslrvp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tcgrglcw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kwwfints.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pujrorgm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hocuqhld.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ydzljxbv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yupzkywf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gzjnaekz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3szcjfbkd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gvgcfpls.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3lktzckhc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3upeehlhz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vygwhviz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3egyuqzig.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ozckcyph.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkgojona.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yzqsaffs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3icsrmsvm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jxhtqwgg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uzznoopg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfjrpdvc.html


<!-- 参考信息 -->