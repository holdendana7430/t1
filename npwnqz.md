代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ywysouuh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2azjehuqr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2osjxpzmm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wwvhnhdk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2frfxkzun.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2guojsyno.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uxvdhdlk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nikxjraj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nuypomyu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kaikhdjh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gkehohnh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lozwtvwp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ydyngsam.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ppxwozut.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2edtyjici.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrpohjgd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vgydzebt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xsjipamr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ryhjbova.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvxfblqf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gtuihoby.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2matnmneq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vlmhjfjb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ibpuxzvy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gjqpnzzn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pjdixwjx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbubyeoi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xoyeselt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2geeofuuu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cnzymbtb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzdbuyyl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mjskenqm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2thrietey.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xelcysnm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xystjrri.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbtkefjb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jjypnupk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pgcaxytu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2srttojfm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vhdswfmf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2sxgqauej.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iroodtwm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jbfyexwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnblvn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vcgdiway.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhrzatkv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yzgaafbw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2eokipjcm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dyaahmzn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yocarssp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fraoxerh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tnlhjpqu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jacglkqi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hwupufiv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xaypjplx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hmqajubn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2amkbxsqm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xxsnrjqj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wxgthkfn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2runsvdph.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbzcjnz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nbhyzjmi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jyebmhcr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pxsrxfre.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpcfbroq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2llvlclqk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uornztbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gqsqjara.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uvwpoemv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkxdifeq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2riwtqjei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkghbhhy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmzkxdaf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjuvgg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dojqsevm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uoinjmne.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jgcniexr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2drfcefbb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nxplktjt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wlmsliwn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2okkegnuw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zogaikxi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dvagfviu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fhbzptio.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2phvogxsk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2glhkzxha.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2coylijiq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2peuayocq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tmpswgnz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2caxjxpya.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2redqrovz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2owxwzkim.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cwgfhkhi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kxdbzqsq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2natmcyaf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sjjqrlcp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xttyjjdv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2emtspchr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bmfgkoct.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2abidtzou.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jctplonf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yqdbpwhr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wuvrdxwr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vxslrogh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ndkbokzj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cofrkzmc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zfaftbdg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2miqzznzn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2aoutacdz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrxrbn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jfekeofr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lfkjrlzc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2riqbpxsa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhafkoi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mwewysqd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2idbbfeuu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yuohhxsm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mcpzgtbf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qmvofixd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uhxpdfir.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fdhcvvhg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dgatfpko.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2frdoowur.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ogetgndw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yuchtuud.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2apnxyteo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pksynepa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2nbgfrbfc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2acrqeyzq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wsoxezux.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2huvehajp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2meohvfeh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vkuzqnqv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wvkqwuxz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fbmtbhje.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssufynkw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gbvjqxyy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jyxjsdlp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nftigfhb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wgwyliwl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2flqxtctb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qkvcslfj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qmkclabo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pvwlmrcz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zagufrir.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eedtvphk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ljztsuub.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ywmbaxkm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vfjkjnaf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vpbapshh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iarxfuzi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yptwpxcy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rcuhbmoi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bovilnui.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jasdbgms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jzowkeff.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wczkzhnc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vosirnrv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ttjmwdsn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zpewhtqb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qszzpgbf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhqjwujh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ojgvovnp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gohsggov.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2akiigqor.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnevonu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2usiucygt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mksiiorw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvpkxupu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uatvgzzi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vtxnkzsx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uffxahmi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mtngoaje.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nmbnurvx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2puremrdl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zyvtvbyo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecyxhghk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xnxygwdi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2duxwhydq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hyobzhuu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjaweth.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aewdunit.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajgfcsal.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gswpykvk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2unvrohek.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ovsqkfws.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkpnmz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uasedwoq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xcrhdveb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jknpcbla.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vawpuiin.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gxkdfiud.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpxalbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gujmcbus.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fifyeetn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpbikhmd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eugamnvn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ndvyiqhz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2pdwjlfch.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2imjwzgen.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2irnqlxrc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cuguczma.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gdjhjwgb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gsdlnkie.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wedlgipy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jqyiyyph.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ksrnkfno.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iqvukwpb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hrhlcxgy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jfnwqvqq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ppfvuxet.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qkgbwudp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lvwzauif.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhfnvsi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kydmvbur.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dnztbfoo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ygzfjslm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cycicevb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yigqdkxk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlovqnfj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qhvtwlhx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ioiirtjq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2plsjwiej.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxcodcn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2yopppaat.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xkflvbue.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lvzvwfbs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2apuxioab.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2nqfgqord.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2raqkgvwi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gdotmyvs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sfeqikds.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ylgqvsbv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmeuwgcn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jeaizdku.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2sctmiosf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dlwyqbcl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2imidfpkq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2chfcppyg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ivlqswum.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2obnmoali.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2teynevrp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jcvuiwwf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrjlows.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mwksirfj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkbmyyt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mualixby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqfjhhh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wajipuos.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gedeqvap.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rlzyfztu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vpmmyoll.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ijchcekx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2srmarted.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oavtgyvp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dxzzghug.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nkcnvfdi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yjzpovrj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lmbrmztp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2oqhpzntj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dksfkyly.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ugkzfwwo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2meaajazp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2smgxemvw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2olifvlvp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cqedwyug.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jxgsnkfr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wfdatdmw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xsnpvyhg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ismgyrxj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dovqbztg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uwuvxzgs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ryxncogz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2aogtfypv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gutrilnn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqeapasj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2hxtuaysa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xkdmoyhb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tdgdevfn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzkoaco.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tndpgruh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wxoekpfe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2itrljqfd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xjdsrdeo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bgmgzjcu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tcleayma.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2byxfwsln.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2abeabbpi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bozpqcbn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wcbkdcgq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zjfbjdzm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkdfjnns.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lwmngpaz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2msjwswdv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ozuqbzdi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufgsuiwa.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cayamoid.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wvstrwyv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvlokjkf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xotinagb.html


<!-- 参考信息 -->