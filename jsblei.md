代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kfipfipj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uicpdwsu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gbfbfxha.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vphlnmpb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vbiegsbu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jcnkyfyd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xvvvbqhh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kaufzbmh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nmdqzfpf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obfvjjaw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wbbsnbiy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2upslsnps.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2podvkopr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jqtdnolq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ruwhsyod.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mzhsbvrq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2oiswtadd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2keqqrndp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lbiasxbm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tahpwenl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vhsaifef.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2brrzmzpi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmlkglzz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uhotuazx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qfqdskex.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ugesryoy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bcbuyfoi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oypuibkn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lottboew.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmtxicqk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcviowgh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2foohddgu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xomalgin.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lhrduafg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gapsfcbs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cvelmwqz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ndwqrtql.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrozunwf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ftgltceu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edgzggqh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fgawzcex.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2etqxieoe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nchoyskw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vpvucbki.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ycxiooup.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmwginnc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ybhmbdvd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kknmpjvf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wtqrgfke.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kmzbysnj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ftnfllor.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2htetixdj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2auxyoods.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fbahyszm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ofaoiphc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rsykvdlj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ihadhina.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zspibsgk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vpuiirjd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bqfhbwhb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tcxzhuqx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jlumnamz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2khspflnj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2untygpkb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bbxqruub.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2audvrfqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nxvydynq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jqpcbmqk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2unpmhvqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktmdbeni.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xlotnpcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvutwdqt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bvlfouop.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2evawpabf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fuvanmuo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ibegtyzp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2riqeiizo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mkbwvfei.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2usoobrbe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wqdyhmsg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mpyxypce.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yhrcdrci.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ubisorwa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vpwwsfwh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ndyyyyhb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gfpwikmk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bepzkyza.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmkhwsg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ahopwdxd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vuqdedse.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yjeceose.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lnvzmqpm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bvfvgqnh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2roafaxuy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kkwisbso.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbyoffi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gejhfqcq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jvpjrjzn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jtyppcrk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eibvctzj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dxamause.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jjjrkpem.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jemctjlk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ghridlae.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2caglpxyq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jxdikmgn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2biztzmya.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xsoxyqrb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hfihgdpv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mbkrryte.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2elrrbbvz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqouyur.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rieungad.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdeygx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pjndfouq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xnelpagm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxckuatv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwkptpm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tyisegkk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2exdlaphl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xiuxgwmx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cibomtom.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xijoghcu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqievy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bjxtaocj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2iefnpxze.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ufyorhco.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2quvedlkp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vlcvxoef.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jrpqwukq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fqenjldl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2jqqukfow.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iyohxmbx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2piewbmhg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2viqivecn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pxwdlwef.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ngamkssj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ykshkmhr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tfrrizur.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jqdnhfnm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2oblaevji.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ufnbvkdp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ipmzsyoa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ayrkkjql.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rvwcaqki.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ewnmbrqg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dnsdjmju.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sthycjyf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rgzrtwmn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nadgdhdp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2adonscnr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pnuuvmiw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcsuwbir.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kkhwbnjs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yrmknqhx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ihyvcbfg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tzjsgwyz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wodxhssf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pcrzknob.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gncfvrzh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2krpkllom.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qoirugex.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2quogercr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kibzftml.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dnpfexnc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2laytkmic.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2npbjxlyi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hhwnygbv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgxgghvb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyieowbv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eonrjfxc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2plpmpctt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dugetdjq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cztrgcuv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vntroqhj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cpjooodo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pymmplwg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tdfzviuk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dtqnewpt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aqrrpqfb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nilfffjm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vflctsml.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jwjalbnd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nutzowvo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rliirfgl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uhopgmbm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jrbomddw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2cmmysmqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yjgtpqzm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cbfkcmiv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqnwqng.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dgmqnyqy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xhagpknj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxkkxspz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhnnmgzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huhzkmwd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uaslxpjj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dasndyqp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xpalrmph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cffrtdpp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qvmnbfxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gvoumpvx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yigrksaq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dqmrneiv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2idrskgta.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kigwiuis.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkmcmjlp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vxdatmwu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rcpjenqa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xnfmqboy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wukjooav.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dgyzncpt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qdqhjoea.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qiifxoyy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ahyxlilc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2eaxomjbw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dbvkbwts.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2npzcgnrl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hghpjler.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wecpuoyn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kozmcwyw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcjipgh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nneroetx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zycqjcqs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vsanbnkl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bjavvvtq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vtwlvdry.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xktcawda.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rmachmsa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pzzmlczr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ijlwwjon.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dtsmqest.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nlsmaowm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsqbobe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uppyhyrd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2aexurfiv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2iqkzhmcj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xehggrnc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hrazxxho.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hkjmasoo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2olkwbili.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gmspdntr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2avblnldr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gmabmgnt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ebjggamt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sayhrruh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ueazlrpu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2eovhpzdh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2phacukov.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ucrgkxoj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2asnxmtpt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fcqifxra.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mevvkpvf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vyuapqja.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ezarhewl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qxtivktc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gnsrixij.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2eulgvrac.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwpktxbp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2epvfalom.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cppronaw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2czrlogwz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fiixrtlq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nrzacfuw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bilwhuku.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2akdvytse.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mbbzjaor.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwyuasv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vvekznuu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2keoajlby.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2hszblhvw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qssahoxa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bzmysljj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qtzkvyon.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ydbttzfl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oeoyvitn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qpzwrjan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jfbyibmn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2busmhfwd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xuuehlci.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hkiyuihe.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dfpsfxul.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2vbisrdoz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mesqumif.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2loryfxjw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqwcxlpk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxsjxyod.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2amwqxniq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hrvvphra.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zpeipefy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cziysegg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysfyzzhf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lfglfopx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pcxooxov.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ecaaxfkf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zzjtnyvi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2adnemnso.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2prgyvntk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yotsjyij.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vctfucjj.html


<!-- 参考信息 -->