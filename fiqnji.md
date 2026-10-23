代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ldoqbvcx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xuikrdnx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cxocelal.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qebjbdzt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ujrbovfz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tetqkoyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eetxanop.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ltnvkguz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bkzvxafh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tjkmbxsh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tmggvxsk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cftszaou.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mrfvoezn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3iucgqydf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3afxaxxcm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gylghdtj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3isfdifmq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfeqcbr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mgqymkzx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3duerkomq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vrwjfsob.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbmsnzss.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qkhnbsiq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvbahzsr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cwjflvac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smrowpam.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nakwarol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iwcexquv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3keahwmiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ibzcorlr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ibpaemzd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wawsoflq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vekzbrvj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pkjluyqj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzbfauab.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mcjeaqdr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nffvaqlr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kuuxdvdu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ijxthyrs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ljpopkaj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bctqfunu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ormqpzxv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sfwzyeur.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3blaffnei.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tblpdxsu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3guiiprbk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aicdwdck.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qimudgcu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dnmaefah.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdadlmue.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hwsffxqm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bfsibcjq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ddptzatf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3utcleczp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fwcskmxh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jawzgapj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3znugmegj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3osnpqcwc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3omvzyrzq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hnznimvy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqwneuj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3phnvqams.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3txdhdose.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jyvlbrzo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ehlmvwth.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cwiiaqhg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yraqjktm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rsauvihm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jwuvrdob.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kfopuoqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zivqfkpf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wyyasaep.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xixujvid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsrgvqxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3grnhysxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rolzxehh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gucspqbb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3urbdkusj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvkculbf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3netezexf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hfwcrdcu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ancsalsx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gdiklsrm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rissytlz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ewlaxzpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3elmhedls.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3afijkirv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfopysla.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mhbzyhyv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dytxwyzw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pclrkayy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qmqrdvko.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3usximsuh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aygechcn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3actiegqm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qmtxpjzi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qfwejubk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jzwodtar.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ncgbglje.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3maqcdbqi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wymncmje.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jviuxyqf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rickwwyo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vouxqyae.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kmcfkvxq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3madqlhwd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwreusdb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zvylbhrf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mwqysfrt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ilknjiqs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3akyhacie.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3okhahamg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pydoapmg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3irzhukkm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vryphwfx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gaugjkoy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlazgptl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dygbglrc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3alvcrlzq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fgvwdnpq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnqnwlql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qvlelipg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kzofajyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wfwjaddk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wsjrgdko.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lecicetm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jkwgeogu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pbtatbcl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxcnpjez.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qyecqlvi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ecfpvxiz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3praxtpxw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qepqrdex.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iklinpmd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cjavqebr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hvpvkqgz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xpglrbqo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3owbhymfk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnjwgmcs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qdqzxjxi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bwqhplsb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cbzzwzhl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jlypwwrt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xsvjcsca.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ljkldcve.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxjxndqi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wxnnkmuu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uelcbllb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ekaagzlg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lbsyrrsi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3njwyhqyk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xktluzvs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mkqymnmh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gntfpxwt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3htiuoxso.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zjxhcxfi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqttcatl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dfdytaul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpnufgpz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqiercrx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hncznrtn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mtievayk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3blaafofu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcfniwfr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dyihxqny.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxjcuyue.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3urmxydgf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xxigjyiu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uzsiejyp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3krdkshzi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hfhcuwjv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lkfqihvw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyeiphlv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oazejofw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmwsskzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3acxwpmfz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtejvmij.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wnahhuni.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uclukgop.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wmhovats.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tpwkaopq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gauuwbxi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rxahcfaj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mcahvsmd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mbziefpc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uuxhylcu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjczvwmw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vyearqio.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbabapp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cirbvpkb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pqvtiweu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lgidktgp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qdxxrfcu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vdoejgvp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dwgxjmwv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wyjujmiw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xzwvfqtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkkcjjix.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vuutsyrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uphkhcbx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nwgwmlai.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3miahvgiq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vshtcsko.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ysyxmdsh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3znewlzhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uuhifiie.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ipmsxlud.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yyuwfbtz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3eyjgmlqv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jbjvakmb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aogwhfpz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iwpuufzd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3twpuitwu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bdpxwgxj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ecwtegeo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mkltgwek.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ylqggrbh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3czbclpyh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fqbgshpr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iyozqrzw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lyjtypff.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjmxcfv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bbtiowcx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wazionju.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3odwjzmqa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvemgns.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3puhmlfay.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vhpofnis.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tdzsfhur.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cgqtmvgr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lxzbiudf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hdgfmvss.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrbmdf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jvrxajwo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vtaouwhd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xewupmmr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ekynvcro.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kvmiyggu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ahreyglc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kskgojky.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lroltvvx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3atjlwdpg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xbimhzhj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rlflyazi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kxkssjxh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vngscynf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lksxoome.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3okxvvsxd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3unarxpnl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wkiakftm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ptdyubsw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ovknuhqh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gwtiznie.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3krfipmwx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gkryawxv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uyszpcgu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gixaxnsq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dwquedhj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dcfoguul.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hihjnmfq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qjformew.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3opwjmtvy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yilbmpda.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tfbedqjy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3teftpsjx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vjebbdgc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jokfodgw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mekobiln.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3imleatwk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3flgzuuye.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dvtgyqvg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3umimatlo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3keuoptxj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3saatlgwy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rvlviunf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kxfdtsio.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dhoaiczq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3nmlhpeth.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gbrplmkq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hxjxqvor.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mofutwwo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cjvkebvs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rflbthch.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ekldcldb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dcribnxy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dxcrpzji.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ndyreeqq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xpnjnvkv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3faszbkrg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dxxakwlt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yahciwqm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gfoghlqk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kcwinjme.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3uvsewhgc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3riycikeq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyurvflt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xcqoojlq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bhuchkou.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yifqjmfw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbojmfki.html


<!-- 参考信息 -->