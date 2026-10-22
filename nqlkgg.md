代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2akwoecvs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybzsmpgq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2setcwmtx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yjoabyso.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dbpiylid.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lryavbhv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cmiqiiso.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcdzdsvd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2snrnzkte.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nszsyzmy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wpehuvrw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cxiwhwwf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xbkyiscq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kptrqzrw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uinttnjr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2emxsccav.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dxgnkluq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2geekidrr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ryhtdtqt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ziepnclk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tvvdgzmu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjshpgk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2umhjauyu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mdqkokir.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uqgpaprb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vabzdwch.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ibfhpnok.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ujflousc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wssdmqyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bpqrreby.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2daljkzew.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sydifdbl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mkkzapzu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2thhvshfx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bbedihas.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrlvsofa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqurwc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fdiapzau.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2afacqbty.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zynlbeat.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kgjuvqjp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vapumzbr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ldbusjbf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvkwehjm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjisol.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2utwlgpai.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2erenzouv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zhthzkdw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2csqyzhct.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvheprnw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2grlrbefg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ndsucbvt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2phpqcvmo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2owdwvmkq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nfaxicjz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ningxotq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xziowsoq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aunobgpt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zjtgfmrv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2oolwknei.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xdaxtbkn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2idhtlzsx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ldqjuuls.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bamvqfjl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zttittur.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zsmgymci.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uqirwfft.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mhabpbqz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2blcemxer.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sxjbqoyq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2apsopumf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cxzomcru.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2djmmpbaf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uevwyvee.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ifyuglxa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hhbqcwhr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fsqsuvfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stjkkslz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qfuvqwmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylikaevo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqykryvl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqizrfsu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gohntrlg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2utfpadqm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mufewzmj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2krncfedi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pjvxklpl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ejccahmd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2igrsovav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ghmvojrk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2thofyokr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qoizmgwj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ktrrmhdx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxlgvogs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eyxgfdtv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xlkavsmi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uvtgqtkw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2funubqxv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpxrndai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mbmlnyxh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bykojkqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sztougoh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2aksoczgl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsodgavq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cqurxemm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2isbtlmmm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xlyptohj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bslqzrhr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hvsstfyk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2logtezan.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ecakcosc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aiiwlwef.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nqoqbbqx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqbmrbpu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kknztzho.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yerkauyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gekqxzyu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzggrkj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xlrqskgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mhavzfdp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fcqcytcv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rvhkhldu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fgiqffpr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2byqrcifv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2akirmeng.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fwuevrcu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ugzovpsx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2czbjefgd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lrlhjssw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fhhllvgt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ysthohor.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lowsphxp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uddntcbo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ioiygwbf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2alumonoj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bafpefzh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gxvxfuwn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mkrronfr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ilwqacxd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2clarxlal.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ddazayov.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rktedkoi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hnlnzwzk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2owpcwgdo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ejdstjoj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hnjqqnfl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2phzbtecj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qoqytusx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wbijsgoc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tuarkhry.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mofasiww.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2peouvqdr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bzcnfues.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mwdsfudi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gghehiqv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2irtgwdrv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2urkycdnr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ozyxxwcq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2llmdzqnf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qqasktxh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ftblqqms.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ncwiycda.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2otmrtuxc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nkignejc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dvpwkdib.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zkauudct.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nzmbdgwq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tizobiwd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vagsvqqy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwhvhuv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tbhfnost.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lrgxnapq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bxogjqmz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbiaqehm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zrtcymvk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2evaadabx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfkubiph.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aufmivoa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwnkestp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uqqeowey.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnaqqtce.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvpaeqro.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fyfgpxkd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vpftriso.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hpmuegou.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kxbvergv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dfchplcw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2okkocbcn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqufzsbd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wbturhtg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ftzijhck.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dtnflupc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2plstlmga.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wznmivgy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2svrsqymq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2whettwzr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nsfrmbuv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2roswbriz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmehry.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uhbxqlcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2oelesubn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nahlniux.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hzsbltfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wywupslw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cwkujyvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qxhuuffq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qxaouuzf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mblatnxm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cxbesrha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bcvoqspt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ogrhzstk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ghktxdqv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cqremdno.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vwghhllg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kfuoppkd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2raowpaou.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kvdsabtp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oyctknys.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wxulmdfe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2orxixfiy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zswdybzz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xcevqyqv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2seftvxjg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbngku.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nkwzolsr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2viivocdm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wgxcpizh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdexoqy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yyoxbqdx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2twkjvlvq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lkdlbfqx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zoqtovpb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2woyrbcex.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wixqvmsb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2sbqvqcgh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fsypjzvw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vvkbkzju.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fcesyekv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tlczwiio.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xlhtranb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wlekebkg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2smlvuvos.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ryeyrail.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pncozfkh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vpnnriiy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lbnlkqxt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qncqbyjc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2aaxnqrtw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdpacdhb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rnhagbxe.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2puaputkz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2imxmzvxm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vxusejwc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2akzbhaie.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ktzquixk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxpxojg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dmvwwfgb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lgdqxknw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zcluuhzd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2oawzwltt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2slrsgqhe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fezldmme.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2otfrkmht.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2unoipmnh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2flgircrw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hkjzivuu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ttycmybh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zedqllun.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wrhnqcqa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjbtnx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2alnkewva.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vyhbqqds.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mptqsxyk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mgncqike.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2bnsbjgga.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zoogmeye.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2okocfiur.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rjzbbisb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sqwuvrdo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qthdjpks.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vttkinle.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2karacpzu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hfufepeu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kieatfkz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2uyxdcmrq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lxvurxok.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pnfaicba.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qzqrorrv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sfrcaqsi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqckxch.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdfhrlbz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dvicekzw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnvckypg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmylnsal.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ngxaibpq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mriacaog.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2jgyyhtgb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2glkvbvxp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pxllnmwu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xmatvrhi.html


<!-- 参考信息 -->