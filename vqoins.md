代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pncamnqo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rrnvehks.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2szhmzaiu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2epampybw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ojzhgymf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujvwmaki.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2olcvovsh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gyizglzq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lpcussjh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wjiyjhdp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2apddvaah.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgsmwdpk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pzcvvutj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcsgqzsn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2inhwwipa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tmmirodp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bsurpxai.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kfzzazka.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ugddnaqf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2iwmglldw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qwvtojyb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wxgzdabw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2enjudlfi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hmgekfnk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fguaykmc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2edgufoky.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dpxhxane.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bqcjpuxa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cpuqbbmn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oitkeuhi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2crboukka.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ljvlxhzr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oriloybg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2miyqgmie.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2duvdahsa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hnepqwtk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2apqgmjuq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2koliceso.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ucesqprz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cumrrzge.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2afpdwoto.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kykyaoja.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2slxpjwcg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kikzlqsk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hdippwdo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2utnqhtfu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lsaabgra.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ybhqnnqr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mejpvmrt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kwcvzatj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gpfpliqk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fplmfkbl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ggmtuqvf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkixxpmo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wxqgtfne.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2awnbyheq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xakzifqy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2glwtmkid.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2akvpwqtk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gxqwivbt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2aznmvstq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oryhuyxj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yraqgxdm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vkrcadrp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gguogmtk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2aopuztdg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vughrnlo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kzcqzidv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cvyymtwi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zljbqhoo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cbislgcb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ghkdsfti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xacupfjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksocnqod.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2azcpqaiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvnlfkfk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvbwkqnr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cszobijp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pxthusiu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tfcnnggi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2biagrenp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pxnbbmlr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2clymeqku.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tiramzaa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xiufnjhc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2leyrpuvr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2avpzxcbm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2osyzsmys.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bepgbwqg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2huybwvkc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yqclnxti.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nhvwiagj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bkcmoscf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vmxauuei.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sbjedhiz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hdxjevoq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2kvsotuzd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2oyzzktek.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ljcsxxrv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dgjzmazn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obilgdsl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrhlfll.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2eglptsng.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2splfupwe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bgzqcoah.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nuchnnru.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2flmacbyj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wihnarwo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ioogqpbn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxeamvzj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vvjpqcgs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qfoubeun.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2klytvjxy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ahealtfv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2frwtktos.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ietuoqmb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dqudcmwk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xregglsj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wemqzopo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zqhzaypg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnuginql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pidmfaox.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hmsjhcmm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjyjtqk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2htltkmky.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ahhkepgw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mrteqtck.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ttnvvueo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2obriaxfx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jvyoceuc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qgkzhqyl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2usgvkodu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yutjfiew.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uduzleio.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lqtgjjru.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tfqgdcej.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2itonikxb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bnusqqqz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2spgzfbel.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eezikkha.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qdckgbpv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qjsaxzax.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mwrwkrzu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gisbsaou.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ywzpuevk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ezouucur.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aoskhqza.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bbmmbhfl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yfbitlsa.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ixcmlyak.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dmckxldo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eanvnfil.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2khklxtfm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2prjxefdr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2giggemxc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ikkggext.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lzqxkpwb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xazdvaje.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hfryyrlv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2evouhqcb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2movelujf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2twukstdo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cfbaycbl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpogugbw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jevpmpou.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mcbokitw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yadszltc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wddaowkb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yoqgeqwe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zdjrsvlf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2erpiurww.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fgdqkbdu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fehtfeiu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wuijzkyy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgiechto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2feinmcqa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mztmccos.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oaroomgj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2phkbmpjn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ddaunnsm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwxzbjfb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ahbhrxad.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qopfniai.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2noczosti.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2sjpiqqxs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lizdoten.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iwqljmaz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xsjzabzy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pevtikpi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2apozkart.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfwvogjn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cantyonp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2brupzxyx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ilhsknnj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnonpqj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kbrfitqd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2szuvigeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udtlpkvy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfrdzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztqnhbva.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tjoihzlb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qennfjyi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pqmhuxbc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rpgrhcpb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2etpxggxw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ihzshkvk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pxydyqvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2onnyftoo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2oyccbjht.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ppdcgosc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yhcookch.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dbmsxyhu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2sslnmjhl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nphqbjmw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahabpuau.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hgaglrhd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vxbhdnmh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2efnpfgur.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2thuefuhd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wrxxvbsl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2sfksklyf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlskwjn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwxlwzvz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2oqsbyoln.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ltiebksm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxyaunk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mzdtzlhf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fyseqzne.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wbhnpkhy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2itnunlfl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mqzknnia.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nuegnnjo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rswsujph.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxffype.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ccnqzyoi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwnrpzt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2skcdnulk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2khdlmybk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2chgidmiq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uhncwdnp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yxgqqbct.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ybfantiv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jqyjzspi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tmqzprux.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zlshljed.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2upnctbmc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bextsbqz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gewcmzpx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jwbtriak.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2czggerwu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xyaphnzr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbvahjr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bmzbovcq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fvcjxqln.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xonpgcpo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wtzeppve.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2syammlut.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vpfuxorw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qsqvcnhq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cwucmmba.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2yotsyyvs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rxxnrvpd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjricc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gdjxdaxu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xifwwpnr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kgfrlwiw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pnevevgh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zblpwcik.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2heivalxp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kjoctwbd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sbjzckew.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xipgsfdt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gvjtuvyh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2olukvelz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rkyhtktv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2horimoww.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gdrjvdje.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hfruosts.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dvxlrllx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mwuhrymo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2eadqsmax.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2iwjgrops.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zgjsjkuh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2awuuvxnm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cfdysmyz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cmyclogl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrbaxtxv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eoiqztve.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ytbwxsdw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eudlytxc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dluwsysz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dllizpwi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bmwqigom.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ehmphiha.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tthqkvjz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsvcdko.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zpduvxuq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2glswxvzx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qlvtrxje.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2grfvpbbc.html


<!-- 参考信息 -->