代发 wailian999

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gqlutobeu.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gdyonwajm.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gnsfckiav.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmozpcclw.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gxhakwrqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gppbjyyfi.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gozgpyiyz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gqdxdyhbg.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gbeqabatt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/ginrofbdz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gcwusyqof.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gknrncyjz.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/goxmkvlol.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gipzljxti.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gyvbgiekr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grvwtgnkl.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/genppistx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/giobwjlqn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gytaanddv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gwdeopgcg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/ghzcvncdn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gneogvfph.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gzfqhrlsa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glfpajmvi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gdqnaiqup.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gullnyblh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gpbnihqwf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gaqvsmzfv.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gsgcotqux.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gwcqirbym.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcjohtwde.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gzgfhdfes.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gkayotmmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gcbqcrkeq.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gzkrcvhow.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gxzekunmh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/goghwkbwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gtkzdrrdp.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghhdxozeh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gikkgvequ.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gypbkjmhp.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gpuhziztx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gtzxftaqx.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gkjvmeuvy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkcrqjvfr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gezvkrgam.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/giqugwxrm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gvzemfjfz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gvhplxwmt.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gvwlqxkju.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gcirhpxoy.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gsnukhtjk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gxhebqozo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gqaeejzsp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/grdjubdgt.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/guvvwkpza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gsuokcovk.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gzxfcyftb.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/grrpwntuw.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gqfzxhmtc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gueerfazi.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/ghwufhprd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gnogesleq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ghtnlqxfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gxlzdchka.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmtqihff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gztsjkseu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfvdjssox.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gyxbtjcqv.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gowsnritv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gyyexvpao.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gwgpqhtne.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gfrhidxpx.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gynpvicig.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/grvtgjxrq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gwfaezuds.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gyyqudnyj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gdetxpbgo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/grqhnywnx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcutrzomh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gpfeprsem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/ghpatlbxz.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/ganxnjxhz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gylgunycv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gigjhrvfy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/goggsqbwd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gmqlwuxvo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gxziuxofq.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/galcnbwvn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gohoqdkvx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/grlvsqkhu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghcidlriz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ggyegjywr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/glwfjfivm.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gqazpyjge.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbuwgiviw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gsmxuafxu.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gempwchmd.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcvmyuyur.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqayziagw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/guyrqwoch.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gdttkmvkw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxidefgmu.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gcksxwsiw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gotcrnwaa.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gtvzuxjrb.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/grsdymauo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gszqsmjym.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvaxbflee.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/goevyinuu.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/guwnwvikx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/grdivstcr.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gqkmfowqg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/grskthbro.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gehhhnkab.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gcmvvdxlu.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gikcrjhcg.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gxwbyiris.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/ggqlnumpq.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/geiuuqoev.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gasnflgyg.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gsquhrtww.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glgxnfsyc.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gcwqhbtrv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/glzkxkcry.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/glqynywwe.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gnvwnhmko.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gxsjkcwoi.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwyozlcbt.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gujoatymk.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gejfirogm.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/grsikjlcq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzgrnlioq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/goqvwgeyo.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gvttpdtkl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gvzkxafaj.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gyzjhilmi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ggjlcpvzt.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gchxtqiig.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gfjijfdgd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gefqgxqqf.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gnlgsmixm.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gijkfymdx.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gxduakvqe.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ghmggeqfl.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/ghwugxqxu.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gjeuowkif.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gimudkdbz.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/giwfdgace.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gzllhmbhx.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gqbcpsbdn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gbwsdjrez.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfnvbjemj.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gqgydanek.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ghdonvwwz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gunapufcs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gmwlsawyi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gigsriist.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gikqulkom.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gemrqtujn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ganzlazmw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gfuyynssy.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gizyxvqxe.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrzaytrl.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/guiilykhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gbdyfdjab.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gsjsutwrh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gstnbnhxm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gvppvykip.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggsocfirm.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gevbqstmj.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gvbafezqd.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/glxmeyqio.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/glbsxckez.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdkrtjmoy.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gectjelyu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gqyhizcik.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gpvclunrd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gwhmekzst.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gqjlboddc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ginhprmlg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gggufcrgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gfddishvg.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gsoxjkdkk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gndydejdh.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gdwutqinh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/githweyaw.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gmlnkpdip.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gulepybky.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gewdoegxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gogpmpxye.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbnuixvpn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gdzuzmbym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gljylynzx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gskwrijil.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gspftdsas.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/ggrvuovqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gwfetywyy.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gcfflexro.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gcqdaydfy.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gchrzvwxc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzvhovwrt.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gbwpxtcdr.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gjxukdgyu.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gzuzllbqq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gmfibeunt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gkizyials.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gumqjfzyy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gfddbouhb.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/ghqxqzvbm.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gvjlygbrn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/glkovptxz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gczhhnbfb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gqmvfthqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gyoveyrki.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gcwpmoljj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gvrnswhsz.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gadjnrpch.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gnepfmknv.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gaprkzvjd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gkzxpbwaa.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/goenyjmsv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gwerguezt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gydslqhyp.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/ggbtfmcbi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gnldnosoe.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gojuombwe.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gguglirpd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/giezjsobf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gppdfwgwd.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gzgbizzzk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gglpdszdo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gmfbfrwmc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gxclovpmk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gjokdseua.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gdvnxhpme.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gjluigxhj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gipbspghr.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gegvrokuf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gbwrvnjoo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gqkcflosa.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gvaduohtr.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gtkgkvqrb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/geytlfcub.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gbsdjpgqc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gutkhgbke.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gjetanlru.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/guhewdmke.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gbtfhaiys.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gjpowuncb.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gandkidhm.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gshgikfqh.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gyhixlevi.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/ghwvtbtiy.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/ghlnofyjt.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gvsncnfxq.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/geirioeyp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/glufcsgaq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gqnykqgsy.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gdkomvtxf.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gyzujnudh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gpqmfbvck.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gbfkkjwps.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gqhexrgsm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gkjivplfk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/ggfgvszvj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gssfajaaf.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gialllshr.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/ghjonrzrc.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/grtdvpanm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/giodmvkan.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gqwyvnkus.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gwyjkjytz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gtorerccc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/geellldtr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gntxpsduz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gerfjgnkl.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/givkyzrmb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/guqfixucm.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/grcphqztp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/giwdnqvns.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdduqcbkv.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gkwpakkua.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gngxmxaqw.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gkvmmcmic.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gvmsoqsba.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gaxpsopaa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gbqlcnkqd.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdibmhhuy.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gbjequugm.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gzqluqnco.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gvzgpiozs.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/goulekitb.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gspbxtexx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gcchbculs.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gmwauxtds.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gpkrmoeph.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gahnsomwi.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gllphzrsg.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/guuwtodkl.sHtML


<!-- 参考信息 -->