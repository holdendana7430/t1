代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zvlcxkmy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qvcamjul.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hviqncln.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sllxxwyd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qwrgekvw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zvfmjbcp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vrftyceu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2iuwkwdyp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwpnmiu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rqdtasur.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uwceoihw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qnjhlkqj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bzprvxmr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ztmgiqjf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rornznmt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lmzoycyi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dgwsbmtc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pkykinpq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmpptzio.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nwqlebzj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kbqtwaej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzoitmqh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tgpjcssn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wlwvuuoo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2itkptrgw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hoxivynz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2umvbetwu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2odnxxgwy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2odftifuv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hqyfudsm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gkweuvvc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2udnxkfbw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2shjafwyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jfuynqjb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ovelehna.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2adynlifh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2phrdpcon.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eljcegem.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nzhfvqqz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rsntkxma.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2spyvxmhv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrtymblp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pglngbnn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2axsttvys.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kjynpigc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ytfgasgn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jfsuqoms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2khqhvzcn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jcpwjybm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nbxqqjiy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eunaistl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yorkiiwr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2csxlvhvu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sfhijcvc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xmvpcruc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pbrzmdod.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fufbuzim.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dzheicby.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tawuzwdg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xshtmfgf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdtfxgvp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2puejxcuc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqkpqku.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2znlrdbkv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lfrmlkio.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lnzsnvmn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pclsqraz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2caoqucwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nqqvrfkt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2opiqbnzk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xfaaotuv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tpdwhapa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bpthrcio.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wgfliagg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ueovsajy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2stuioxwo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vctweldl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgmncndj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kzkwezqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzpcuazl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mhgpnbvv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hbbeyeyr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezrzmfrd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cvklsxuj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ppgqxjmz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rtaivdpj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gofmvplc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aaikskwz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2smwcicnt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2htwslbxf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sukzlojj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ernpmfxk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hjfjhwzj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vqyqpxoc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ciecshuv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sxtkpxsh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oyxbuajd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fjxfsvel.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nceuhaby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nlnmsuzy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wtyxzfwq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nmdcfcut.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cwxrfbcf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qvusodqi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bjnhugcu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piykyubn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wctuyvkv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2byxjmmba.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zdfugsmn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qfftjytf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfxojhxd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gvngrfxu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ziffupqy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2znscoqjy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2myylfewa.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uthmpzpr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ilafrpes.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2viquuogt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wnmugpuv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zugenjyo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2plcbujno.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zdvuljht.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zfscjddo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gbahinth.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyaslemc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lazxqgbl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yyishekp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2soytyikg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yqjxauaq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2kzmfdubl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dutgibul.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ghqswoos.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sjdqsepp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fyccmpkm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sdoktguy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bmdroxco.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pkiiwjxm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mymmnjqz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vhwislis.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zbplxnvz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmgqpzqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ugtraeoo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpshyuxw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vpenpskf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gnguwarz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vlbefyfy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2idxckuow.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wwygvlhd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gqxwiqwv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnxtfdjd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2broueedh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sydnmjhj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lvawmqap.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pmqwgrxx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qheqnmeq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xpeohzfh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hhvrieyt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qujwgasm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rislwoab.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ibenxclb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ryqfftkh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xebajlgb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iiondglo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sbwfveel.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xspqbyxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vdbcuyiv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xwiqklbt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wxgrajog.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ibykgmbt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhlrwrf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lefggpqy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2csmnaknb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gpvbkqsa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2posefgag.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfhrxhjb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tljpfrzj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oralzwxo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2crtwsyvq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlivgwcl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xrodvxuy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xzqgusyr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bpsteptx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wmlbsemm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2enhamsaq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lzmuynya.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ggwqchiu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kovixneq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cfdfcycb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ywubcwcz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tfmtfomc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oxdbiezj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cvajlpew.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbhbkqa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wdksqztb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibuvutrp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nwihfvhe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ncwibtgx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pndtrxcs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wfcgiqnt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jiloilqc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdivcxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndwnibly.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vjmwqqca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsemvwlo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jqqoilvt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wxixdyfs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2orellakh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhdrthxr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tcdfrvax.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vpdfxjkb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xjtkdznu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vdcsnoie.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lklyqoor.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bqtzgbyq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2scszsbcv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2efnjidyr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2aldhdbdw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rgsqekvq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dfzbmnet.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wubhjdsu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kuwqavko.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2icfnicqr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2suulbblm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lnhmvxtx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dzuhtpzr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2igdkdkno.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2alcrfivl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fclefdrt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2frqwsilp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2risekxni.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2odneamsr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrjtfc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ndpakogd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sphdxztr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rpgdqpvr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ztpepghn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nxtgxdit.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ryamhtrl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2pvqhuqqh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wvgvlvdr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fbwktojh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdfbexdv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnwpdk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zcqmbqay.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2scfnbyld.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nklmrmdb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wltxdqno.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2taqstzqh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lsprmsxi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nelblrhl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2drgjutmw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwemxpb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2madzgsyt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mvsuevka.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rmwofygw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wfziravb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qugviioa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rhkmdnbz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ebkldwxk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hiylytuy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cvajjtwt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hjkdknsh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qavbqcxi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zelrhefm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lhliwwkm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ouohwlbl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ewzbskcl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zigoelnv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2fuhslvgi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aeyohqlq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uslsjeqr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mxghssfk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2exlqmtdg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2nkzojtra.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ephoyrfx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nnygfffj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vflqhtdy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wydazlxh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lluvucxd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2soblvhji.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qdhowalq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wtxuzerz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dvtzsnwj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mtbbujpw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wghsfqoz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2sqzxmcyz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xquenbgt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bekdoxfk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mkqclzrd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iwykagyv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfjgtuug.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uwidvuhw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnuholuu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pedylvhq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wjkhdcpd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ywohffbp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qduqrzkr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2atdgjfkq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ixxoionf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ecslgong.html


<!-- 参考信息 -->