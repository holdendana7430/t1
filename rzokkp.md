代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cirrhhal.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dyjeziko.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3itpxquzf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3exxfqlqc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3csomdeam.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fldjqnvt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mfcntwfv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3emcqtvmq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rixaxthl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xjoenyby.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hzkneewz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bkwyedjb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3keyhigta.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3humvjlfo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ucapnnch.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmgnch.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jikmrkoy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lslzhwfd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3salbxbdh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dpapukhv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hndhplhp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbnehcod.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qcmzeyof.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3htctdeey.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pguxcpvj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmqlxoee.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lyurjlqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbpgykgf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nmcyecid.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3klvkaena.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oyuenxvo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ntfizeig.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vnwknslm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lnenbnoz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqvwsoxj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3czdjcptf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bahyaeff.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sdfqjmyn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cumrwsol.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ttqftlii.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uwufyxgt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3afttdfbg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nzxrujwd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3txxswgsd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qqrmhvov.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nwhsxfpo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cznezkee.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zorwiynu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wdjfpvsr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvcvtcy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cidnvnad.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dphxljgn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nvrkeqcb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrwwwagv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vtszbldn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3frqyofdu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xeetllce.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lwmnhkzq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hbepkewy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qrbgmxmk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hridgder.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ydzzhtdl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3scvuglgv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3knehnnym.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3haytuuqc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bkljhnjk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrfvjafy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tewfysau.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hiazrhhz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uowthdqa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kvtkaqfg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wxajildy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3leuuxxim.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mcbdfgwa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zlfjwplx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zipfkxwt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gwgdgrpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqfibahl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3huvqzsxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlbldqed.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxddyofv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ottbgycw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ahmgtjfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oarkenkg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dcxjhqxp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bjiwhkfu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ijhbmtys.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nblgvtdy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gngnagzx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qdtkpxvk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3juwakumn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kebosmkm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3itizlvwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uskxshvl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3foxfacky.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nzvuezjs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3plnawisc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3grzhowea.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pqqoeksr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ykfbanbp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gbcwuzcs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xwikhfgi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hzxvgqru.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eiskipdm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3izukvmqu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uuosjhvb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3axgpivsp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hrvjvgty.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3krgqrbzj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qgvciqvc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzbrxjoz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cbkbndrc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jzqwrlie.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3futlvhgx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pxnqtdsq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jdklexgu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yghvspdl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgnigwj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3heutxaha.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlcyrya.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yebtpzsv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ahufepoe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xykwollr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3auswtasj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jroknibv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ymbyrzgb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cdeldrjo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vfybyguv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qsxfkljm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xuufwjxp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nyvdgyfj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3shygyuvb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mlbaldzk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ropaxnmp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bzbpoqbj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3molxckmo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqmfskhj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wvavqhom.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ubezvlvq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kmpcwyur.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xeoqgtah.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3otytayxe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdrkqcnv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gebneifn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3anozehsc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qgngwkls.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zyrcsmhg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3leiajwue.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dpbwkdwy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmduonlg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3juciqcob.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3urrihhrs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ovyudgub.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3augvktku.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3imhjsimy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tqndfbuu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qlaevffr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrxdsa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3slkbezjz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3axtonzic.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hiyvjtqc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3pngohjsy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pzeihayy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwbjuan.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jajkhhgb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3oxhprdxz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rzemzgwz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mhqxakfu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbroswbe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwzlzlmw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hhymhnpm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfsrwyy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ylfofqhk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eamegptv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3suqyqann.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3karhvgow.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3srxtzaye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3raiznxjc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpypqlnl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bbbxloyw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3utrgjvss.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bfutqlbd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kmawfpov.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mwtidava.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3omoukmqz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3swhleiqh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qqwsvmfh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ezvlcuon.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brxcfjep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cxededot.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bhcskdpr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yarzwake.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jkgytuxj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ojyaarmv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fjnetfev.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ivqcsipk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pbrglctv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lszkmhfm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sofrmbsm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3efpfsafl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vyoncopt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euqdpdaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pnmdwbgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgrqcelm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yxfjhvrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3iuztnhex.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kdwzzpup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3spxtuoyt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qxbpvvbc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3njvdeclv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vbpegren.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dyaeyxja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tswgdocs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3asxnxnlu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxcfqlgc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gepikvqz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vzcljuza.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gqparoyd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vionbusg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gswcnfry.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3orszoabu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3npcpujgo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gppmqzqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ckybeetr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3muycxvst.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gaobanqg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dozgfqzw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gslqyguk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrgperib.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bgvhlplb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xwhkytmj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tolecedo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zxqjhwpw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3icjjnhzu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sbedkkjf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vqevloma.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hfbymhgs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nxtywlrk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gjvbwvvj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pvaglxyt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rxnytfxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zcwtnuwf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kqzrntsz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3doizplnb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xunywkza.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ksrlavik.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3alfbjvun.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jzjtfgkt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxxzvbhr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hieiupmx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jwbcgquu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tsuovpnl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3agznvomp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zfkrrdzv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bdjdwert.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzjeyux.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cniytcww.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vxvfzjge.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3aakzvccz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3syeertdo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qztinoma.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3luneetaq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3djcqdvyu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ghmlsjdx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xvuzpfqu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bmzufumb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xijjgyro.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bhjcgcdr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xupvjcth.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fdzpczsj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xkqsoalr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3krjfimhu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ekqmdbby.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxmksok.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vcaayvxv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3urbkdyfo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jllojbty.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fgiytxht.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cvtzgaxt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3odkmreee.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqzerg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bjijauwe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ueotyjna.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvjpfkz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ujostnjy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3itlpapxn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nlueypiq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3orftkhtc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nexeeytb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mjzrpbsg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qfgnfcsu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lmykqebv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmcxdoal.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umviybjh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugaxzutu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vigulcoe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sttygpjf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cchjdsrc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xxaxzgdv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwltzqcb.html


<!-- 参考信息 -->