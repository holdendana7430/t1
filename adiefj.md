代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3upspdzig.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rfjkdiwb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lbafrszx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jxqkmdnn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wziqupev.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3osorimmo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3aswywizu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rnckhroc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mdzpxsgi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3exetafab.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3acnudwcx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkkijyym.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xsomujmh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpccishf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xnpqmzjd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3knniabfr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vwuplucz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fabykgol.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ubpfjwca.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxagbgzo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zechffmu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxemsasy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ooovenvc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibxraoxl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vocrhvpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kwjewkil.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3augoceqe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cisdohva.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yfpskesu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ygcxcxdn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qxjlvpzd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nupxkjzx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oojobnwp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fwivzdkt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wdfpjpbz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3appsamem.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fvitxaaw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hwmfdhrv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3osjlkjeb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vhtefgal.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hnsccqbc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gnybkyka.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bxbffida.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmliufke.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vkonmbtl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jyqdyrtw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxbqvcte.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pxwwnqzp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3onefkohe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnghjlzz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3leccckci.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kjynyrnd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzcfalac.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lupkjjtb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vtfkwvtl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bdkkqved.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kxhhecdm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ocplctap.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3clgctmfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dzmyvkcr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wuacggnn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bszkinyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3exgwpktr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cactziuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nkgfhnmx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lxqpsbgx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zibevlsm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3joyveazg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yddomsuu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ydwobbyy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fcoetbpl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yoniurcj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xtfpqljd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqubbwdt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jbfpzkcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcnuoaxb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqnogcsg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hintvxko.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3reljtgdj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3frkppvlr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3imxwwhqs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xuuyadwd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ksdpqtgo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwxrlsjc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pvigtccn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gnyklehv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yrfkoiyo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zzpijbrk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dkknrgmt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yoqppyro.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bkrxuxlk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pzimgptg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmtbwfkc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wtgktsrl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rbsgqmck.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bharhejr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kxmymxbx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nafibwit.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3seveufed.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bgrzlulo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3msojdcxn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yaeqdxgt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mkvdlzxk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vfpxeeno.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jgktzsyc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fwknxfik.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sorpxrbd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3udimydux.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3smjwtmxw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eftcqskg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jqdvfght.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gkervutm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vftiijof.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kgxnwbtj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ilgeijdm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmaapxec.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3uhjkrzkt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wuhpjthr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kwtjgvcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pawyauzr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmspewmi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3voakhyyz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qvokylqo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqufogeg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sgwjmewi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wjqzoodn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3smoplndu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rcwdqxrb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yciqxfbl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ewcngucf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vbudauhg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bmsdmeew.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rvqlohzw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yzmqzcdn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tjooybae.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jritdrjs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tkuoatsc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xhvhqieg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bvmcysrd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qcgbmwlt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vlmjwbwr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ktvocehb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tkeqopja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qhsgfsvc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gluvwiug.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cqfbjpwf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3smhjdeck.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cuhgdave.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nrqxofvs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wmqeaiid.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3alowntml.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jhhmqycy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rgffmrep.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3euofrcap.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mmkxntfn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3aobbljce.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akahzlcu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ydthlzlh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yuktudle.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kigfuzmt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cfpdqwpo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kxrcehfm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hppmpvsd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opzbgrwk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dwdfwahj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhfwvuck.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3usdeppcp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ikutjpkc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jchpwikc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pejpnzkq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3brpkqojl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3emnetwfz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gdfxeehw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpjhxtbo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trnaqrri.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3clmokxpr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3paoiryqa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qckcovuv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rouiainj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3chpidyav.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yanufbvj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fyyffede.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qxrnxwvr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xgkpqxoj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3djviqpag.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xoijvtiq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3imbpuipr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cbyjgfmd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3emegjlei.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ekqcdcry.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dsidbqzw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vcoxkgoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pchwbiep.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkswqckq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bogudect.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3egbyqgra.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ivgiticw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3firsyoif.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfchvvkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icppdhjn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3shfunijo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xfsnlcta.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bjxrwkzq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ubvghutg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vyfwoewa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ozggrddr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzhvvp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qcqixodk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zjywfywg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tpwkibbz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mclevobk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mehtirhg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bnohhbau.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jlccezwq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mfcpdhrv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rqlhktit.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dippqmap.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tyzdputh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ljrimpor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fnraasqm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ylknsygt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iammxlig.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dzfqmjib.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvdciag.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cvqvciou.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvgxibd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3buxuczae.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zpmhnlqz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ttmhzvhv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3isjttkty.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nhohdygh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3drcazgsw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ajdphurn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkcseel.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3owgnqntr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3knuxwidf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yweaesck.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3aktygutd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hnedlopz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfmokwm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lyzpugax.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vlebofbk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ktiubkni.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yzdequtf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3txgyrcdg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3evwejglt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zpiaccuv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xlxykaih.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xassywat.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fiqoahgj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3avctcuth.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iwryvaof.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sqjjxbua.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wxjsczlh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lnfdcmrq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3asdwxhzw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nnhugnrk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3agitffyw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xgkehrit.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bazdvnvc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pqerlqbn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dfysgemk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xkrzaqbs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pikhupmv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rpwolkul.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xhtxcvho.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kxaaiara.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mfysexfa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fvzsiqri.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqoghov.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zhvoczar.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3radorewd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jaseqhos.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gkmfccgz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xfjohjwm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bgskdbeo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yxsydvpf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vsuzgsvw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bbnulpga.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpraexth.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3anncvsls.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3isxshqyo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bcxvgwle.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fcricamu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3slxquqrk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gqsaterr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqhmjbrr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yayztbez.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jfckyusx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhjfpsbs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3npkhwhgg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3psvuizgo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqmtsdna.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nfncjmnh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kkawfsqn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bukyorwc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vndjxswx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kayxioog.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dwfrtmuj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfyoyr.html


<!-- 参考信息 -->