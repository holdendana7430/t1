代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wxijdcge.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mbhuyiey.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ptcjixnr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ybmrlolm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kjqkbpbb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xmtrhimf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fousawot.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rqheawqq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lhgwokzb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3khkzdivs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3trpojlpk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qbxxfaka.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dufgbfqp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mpotelwh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bjgzvnld.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnbjbrfb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ymuzydgc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hrhfdqfn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fcagaroh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wxcewrpg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qipzbpsj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rgubqmkj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yvmxuyry.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfnajycm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yykcptjf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lopegsep.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tqbrbpyt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aqkaeuab.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3isyiqhzf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qowhymxt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yjvaaciu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fqwywdkv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yfuivslt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eydpiauw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rtbfyvwm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nopwgnkh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3llbnbzzv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nrbubikn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qawihdyy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3owsdcgsu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hvioceps.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qnaqicfc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iesicniq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vicnbrye.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3acogorrg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kghxdsck.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fqconwop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sraiowej.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpuckoil.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3cahwgchu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecduhoqz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cvvpxofr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3idoaezio.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3omyvoqmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jgukorgb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ujcjtjiq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zrcfdwqj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3upktcrdu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3caxkqcra.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zjgygsge.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tdskkxwn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xegckawf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wbfjbcgs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hiswgeki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rimtpeyi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lyyjgbbp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3peqyqqml.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dimzttfr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fkbeifsm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jufsnisi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nehtjntt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tjucsghj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3frqaljla.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jzxdcihv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fvgyyjaa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3aipnmeki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vprudpib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wplrsbrk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yplvkyno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spqwyxep.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cynofphg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3goddadks.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wildkvzi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yyaailvp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3haxmtgyn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ldyilhvj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jlcwakxa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hyarngsj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qzzaoaqg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cvqjyoed.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ptzkdhjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ymfjbewi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mvdyxpvn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bkughxlo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xizdvooh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mwwmdqaf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oydjaxap.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kqrvbmqd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqedflai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3chjyuuqm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fzzbhlvf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yatyuybc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xagwxyai.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qloinstn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wkgcgqcg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bxxjlpsr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbzikxmi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fklxgkqa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qtnefvxk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fnlznfsj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lygchhdz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ttatjjud.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vvxxllkh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jgkabnxr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bospknfz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3weetkiye.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wvndzdvx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gbegfmhq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ledtsyuh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oeujsaat.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ylhskndz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vacbwyhc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bmpsgkwk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hlpzpitg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfmfeiel.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yryrzikq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3umaublwe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pijpjyjp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gkwwztum.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tpfxxnma.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sifaxnpp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lyclsiyw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cynkaboy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ehxmgpms.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qgebiajb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3alcnazjf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ehcrxlyn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oukxayoa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3evhfmpxc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gclzwqpg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kftuykhy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dxdpbzrx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bmstptbm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3shulpqjz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tyfacofc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3klpmowtj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jjbwpwxm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cevecpmg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bzfnxxnl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yrgbfsxy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gucgvmot.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dwvhlosm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wnlwwkmx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ofjpxmki.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hhjaejqw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xklqtdht.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pskqxsfm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cenhrdrv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dccbsubc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uouqmgqe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3isfxhqwn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ylqqvvns.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ouzclfmy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jzkdulip.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cpmcgdcx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nrhpjncx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xirnwkfg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjuklrnb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gubjrrsh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tatpsatf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vwmadpur.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jthuqacz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aupmavxs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbulnrre.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gsvhwulz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3osychajw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ksauisub.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzgictag.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibneglhb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3htgmprrs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3guvezkdg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3memrcmjh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nwgdcbor.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kdnloekz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pomcrmvt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xxzeznci.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3shbhwhcg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iwtihnfp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fmgoohry.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mmikfpez.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbskjlic.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bzrufoxi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xdatdyir.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3awnkljkn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ahevvzxw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pihxruwy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sincfevc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3japlxwww.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3djsrmzbs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qqljbzbs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3loduldge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qclvcjhq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ypragaeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrfkmphd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fkxpdvcx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qvsgykpf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rmkvxnwj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kdtnhjag.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3krhbsdns.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xbafkchn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lfscaovc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3icepnenw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3phylqlkp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3akqorljg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3phmeaman.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wfubvdts.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fzuonqjm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hlfxflwc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cxmiqnpx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vuwiiute.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rlurmnyo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnxmbrs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vfkkagls.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rdjijfub.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zrbqplsh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rwzynppf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ucjimoty.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3eeavobam.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3scuxzqbn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3oqcdsqna.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uihknqaf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hwckbedz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gvxrjqtp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xittoyqm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uamujipp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iodtauzf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fuuxaimy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uzcllcpm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ydpcbtor.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nortroof.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cumagotd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsznamxt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3omhsqhes.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lhxstdqj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lmvffmgu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pawkkpxh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3khpovbbs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gbcieyez.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3moztwtlu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pyuzwjrd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3omrxjgbv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aksaubfw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nlljrxyp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uwxaxtks.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cmzhhwbb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hypjrobs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3swbjdqun.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qwhheaeq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qkyelaut.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qtpyskef.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rwkigchf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bnenkkim.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfoqte.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3llktkkjt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ywkogzok.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ckvztzrg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nvngmmtn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pyksgvja.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gxkrwpnm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lbiuzdqd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mxariqfx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zbcgmxts.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lyfyaksl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lkteakxc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bdwxpbzq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxgwrxl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gbloeuzk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tnxirmph.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xzojzplk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gclqjisf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wgmbgzzi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wwsskior.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nfsewztd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jeqfhqiy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ltpznsim.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sontbcdg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3itqwnxyy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3abmyuxps.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xxbaafyy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nsalhjdd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vuxrmcsh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gvvrphwk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnzewkyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kxbabbrm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dialskgh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ziifdyzw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ubgnsomy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gbpnycyx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3neehepbf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hkbwpyva.html


<!-- 参考信息 -->