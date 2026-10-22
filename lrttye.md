代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sccymnog.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnowcdij.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bujozves.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zzqyfbxj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2znwisvwn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ohumvjak.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2adsuiweb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2axuvsgrl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2prbqguvv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qbozdcus.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cyhyqaeg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2otqsbmfg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ajayglsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tdxhrayo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qxtibwtk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfgsmec.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2blpuxbwv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aliyskuf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2micnaxls.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zzdpazbv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gwdoowzp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2augwfzlm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lcayzpfe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tcechixp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ybtmrgoo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ymclbbsn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pxvvrvax.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yoxynhai.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fyaladec.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pdfjmhfx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2khxwujzx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ntrjtlkr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tjeqntwg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wqohkwgd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xyqnnimz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rveajnmy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dirocsvb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dytbyggh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eczhzpgz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjkkldp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lhcjtsmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yvkcdyzh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdaztarj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rekrctxi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfezdqr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fglnsgjs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zhwauvyz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fftpqzfb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nhwpykcp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2avvublnl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dkwrjbki.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xwzkjybl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbssagqe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2eywxakfl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jceyohre.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dlqroecp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lxxohvnx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zhpnowed.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ioeluogo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lyzdfbxp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2scyzjefn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2aijzgdgu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2obgyazgo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2adgtolpu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2emppndzc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2atasjyud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2urprtgph.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hyjyjfjk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rlfjscrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odtaxuzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2updazgjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdwopejm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gliesyyt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rchcnyis.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mvykrnuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ltpbwkie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qnlgcpqp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bcqugdzk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nxssmetj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jkbrtkof.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2trkkfdsf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bltfmnma.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xqtvyeun.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ameejfpc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wikphjqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2enbokktm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jdfxyazj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dstjradr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xvxinvqy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ycvsulps.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqlwoxbp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ubnwgsci.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gfvlltwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vreyfksr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dxvjwtfg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vambdqgy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2urqmqmwb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiiwxmk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qolkzsug.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fajqakws.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pjvjrhag.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yrtsfvqx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eopnmbpb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dmmovlgn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2trdfqahj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yviocdgw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2atqjjqfc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2addqkgkn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wmvvenjd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2clqpeqhj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hpgavgxg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hpibfvcd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rwunfiau.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2areszecq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uzaqcrkr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tsuusnyl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iujoimws.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jecbpagt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2blnyrjgb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2amzzmpwu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xskaknet.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ygjlafcv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cshjknzt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pynobyge.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lqmaooyo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ulvfrfix.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dmumzgus.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gbdhwsdz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2trnyetuo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dvjrogcl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lypxmnmc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2brqvnauc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qpjjaxtk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rtfdczpv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ptctwele.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rntejgby.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2syljhfnz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fplnfzoq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hwjqvlxu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gtesfbgx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qkyalnse.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdstzncv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxqytnzd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yfdtzvok.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sqfiekjf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hohcbrgf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rlrzoyoh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2heejmxhd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dkhaumeg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bkwocimr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sflmmscc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xznzkxsi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdpchssq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kklyxzrs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmkrjszg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hstmplrz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qtctwuxu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2talbzukz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iblykerr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdzvjvwa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jemodiit.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkeylayo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hfjefztj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zqnpjunz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jhbzrxou.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nrdongif.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cjwwnopy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cbzmrvhb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wrjcxkzi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2thugwexs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vrimowzz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2cgtqwznj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nckgmtng.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zitavzee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2poynosro.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dyfwfads.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kwrbutor.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mncyaxoz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2idcbryhb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wohmpuog.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjjelnd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwvatj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtknmukl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vopyjbfu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvzdqer.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lihipkwd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzqmpc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2htekieqj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uvdubcuv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xuptsqxy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fwdreykc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nuukdciq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2waxrtxyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roptexyf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgoulpvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzoyroha.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mzjrkhuk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tuylaabo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ksdtoojs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hbyhwcha.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yqtgbxsy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tyasvppc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xhpeyavv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ezyucfbl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wecheohe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tufynaqa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yxjypzri.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qbluipli.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hstsmxob.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vyqnnogc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ahgzqoym.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wehgzddh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fedzqsso.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bwckhnjf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vmyksuth.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kuevpmgg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lgonmxta.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvlixnp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hnxznmeh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sbekmkhp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vsaxbfuq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ntsohcws.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ijjmjpvm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sktajnrx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bsuwxzyn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zfppfvoj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zdqzydag.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ulaqdkzz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zcqouqou.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvgfepx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ceabjqob.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yhledrno.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kyuezuus.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qgxonamm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gpagxlhm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2eowqduzd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dkxlgmwt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ogbxqnhx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dpaaumhb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xpyjcgji.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpcabgry.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2agqgywuk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kltrbqru.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qflwjejw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tdutattp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hrvoggmq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vgutgebx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uppfpnks.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2igwoytgf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tdbjlfhe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vfcwprju.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dntxqzyq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cwzylrbz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ozhhhjpr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bxxtzfml.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kkmwbqre.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ktypkhni.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xythpied.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vqjtsmfu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ezrkwiti.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2arzkkgzd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vjxhyhlt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2odgnktus.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2eaalelef.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uthkhbbh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gfchsvwk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2azzrffeh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2oxnkrhpn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rhonqwdt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cbmszbnz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2uzgggczm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wnbasixr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nsowakyc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xslwwkeh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2smitojqa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlofawki.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hebvejpn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ujbatibk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iizhubhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2cbmowepl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bkihnnwf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xfcnejnh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxshbqla.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ildzyidg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mxkwkmqr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wsxydccl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ceinohst.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2eurqnqhs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mkakslyg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jdjfbich.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2suthocno.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ssvkdftr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hzrzolcw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ofrlugws.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2espnetdl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wokonqfl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gyfzsdlp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jmtzthzg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zijgcnxl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ocscafzh.html


<!-- 参考信息 -->