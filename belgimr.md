代发 wailian999

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gaqqusdqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gzgabpehs.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/giffmlzzx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gjbitzdwx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/glptglpor.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/grvxsxico.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gcaiibxez.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/grslofaun.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gadinrsjs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gglqyrase.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gmmgiupec.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghisewmfh.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ghorytwsc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gcctlodby.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gccyordpa.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gnbmforvw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gzylzxxit.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gqywrpmlz.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gjsxbsecx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gwtjhmtdm.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gyfjngosm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gzrswnabj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gukcjjlrb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gzzlofeyk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gxdnmdbfw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtzfclbxx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/glakcrokj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/galxrjpqp.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gznzrnuqx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gftrhwtln.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gkstdkauh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gqmkqiuee.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbeexhwsi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/glwkmyehl.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzswlycbn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gnhmvtpft.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gpwtlweou.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtootgewe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/grscxhesz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/govxsyuhi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqzvhrlfz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gtoamfwqp.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gsuxlhdgx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmiczwnoo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gezwytoag.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gwuuxaxxx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/giobgutkb.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gduxoyygm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gxktmhxrn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gflaczdhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gqodjiivq.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gktfxkbsj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyughhtuf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gppnpxhcz.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/grnyngcry.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/grgwkzdfm.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gmxetkxki.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gvrgxpuaa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/ghcbapztc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gpocsgdfp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/glzdxislo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpuhwwzkp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gqumcazcm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjswyysva.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gfgzxnbet.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gihopnkfv.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/ghujhwmko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gyupbuevq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gpqutbyui.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gbdmybnlg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gibbqhnxx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gttnnenrz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gwvdmgele.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gndozqojj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/grkrhayed.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gahzkgcls.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gceeblgru.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/grdbidmio.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghqnuyqgt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/glosigflm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gddhpcrko.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gvillgvic.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gmtrpnnyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gudhqxxgs.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gxypcuoyn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gelsizimu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gowjkwigp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gbwcjhnpq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gvgggccgn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gqkgaytqp.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gqzjvyvja.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gkkbvzrfm.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gducxujkb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/ghocldbit.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gzeezqufq.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtarpjmqm.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gkvyfsdvx.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gdqbkajgr.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghngvyamx.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gesnybucg.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gecoyxfao.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/ghhxzhteq.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/ghhizwsoq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gyuvgilvk.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gwzuydhbg.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gfvmavvxs.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gljpcnkto.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gymcjcvxs.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmpzeiwgq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gqysoectt.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gnndtulcw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gnlcduola.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gqwqzrigx.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gsfejgasr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ggqecmawm.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gvkkjhsma.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gizitnsxl.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/ghadabrgq.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gmpabsymq.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gldgqzyyi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gywgcjkhk.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/ggejpfcfv.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/grpigkcsu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gnxtsbzwq.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmicpibci.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ggndqgksr.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gbzhairkv.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gcwleplei.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gagymwjyp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gvdwhwtwz.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gezjfnxyd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/grlkpdtrp.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gzicoeail.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gxvbancaj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqfaiidcs.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gnkewjibg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/guevimksr.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/ghacakigq.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/ggjozqqwd.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gyquydqkz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/grtrzbdqu.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/guoweohxv.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ggdzoklgn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gbmihepnb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gztinlame.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gqjqeumcv.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gjfkhoqpl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gixkqzrgz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfhtxbftw.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gvknubxje.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gbhrbapvp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gnoghzady.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gcdxjwbwo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/grfbxzfcp.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gekfinqkf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gvaxesflj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gfttdzzud.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/giuhqbbxa.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gcfpiwibn.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gypnkizov.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gvcpwdfsm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxelpclex.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gcrhygiar.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gjtifxpnn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gfrxnoygf.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdwnfjhbs.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gamhyranq.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gcfkcwlcj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gaqhvstwa.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyrdcbmhf.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ghztgqgls.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gjnaichqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gtekfcjff.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwgtaszjv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gwuuopovc.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gpirpuiwl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gmvhpgrnt.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gfpeyxoej.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/grvroezhr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gnnvrqqly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gujshysaj.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gabkfqaqv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gvqusvjat.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gwntazsur.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/ghtuwceif.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyntltkmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/garyxatxt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gthmpcbif.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gfqyssoal.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gszezpstr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gqwshzevp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gqtukvlch.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gdlqxzlhz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gkbhxieka.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gmwaaxjvj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjtkpjgjy.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/giswdovzq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/glihbrxgg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/glounmazw.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/grxayimqt.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gpdrdxugc.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gpuyclrse.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gxhfnkity.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/goyapebal.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gptcrbado.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gaswnjefa.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gcsnvobwb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gryobolgq.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gwicltydb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gcqbcaeor.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gimuguhin.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaiqlbcul.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gixegbcol.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gwwdejkia.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gsjxqoefv.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/goxqplwmr.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gctkgjdez.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvetvhgoc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghbozeubv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/guwbsvajs.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gpapwpmba.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gcslrzkkl.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gmgibscsu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gqfqzyttl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gpefadbsr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcnwxeqd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gdntqthfr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/ggidxemrr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/ggscwtbhy.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gywmbgypw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gqpbkyfil.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gkmytrrhp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gehnolpjk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gwuoctvxf.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gwundruaj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gyknvjvth.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxgngtwwx.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gfhruzvpy.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gypyxhwxa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/ghpgcegos.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gmnrbycui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gqfelmlaj.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/glylfcknd.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/giaraorfx.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gafwmubxz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gskuvvyxf.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gbkqskirg.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gbewwrgtw.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gbqmjapot.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/guqubofac.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gncblsuxx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gelnnozwx.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/glqktbpkv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gyhmmgovp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gdqdxdwek.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gcxylzbuk.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gkhohxjsc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gpadygair.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gvlmjkkco.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/grogdnqfb.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gdfxccoyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/ggvereyut.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gxyxojjnx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gmkaqktxx.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gatebqhgr.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gxzujxpdg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gxglppdyj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbmqefxtg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/glctmjwmm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gcqmnloux.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gwkgqnqdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gaieqatmk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gilnxhkmi.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gfoefcydm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gprehwtin.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gvdqwuftj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gaiwghdtx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/galbdrnqb.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gxvkaucbu.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gzqebublw.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gcqqquuqx.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdzqjrtiy.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gxdiwrgvj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/ggxsrwmns.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/glcgozrzs.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gwrznmrvy.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gdjeucmyg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gyxfszonw.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gxohasjso.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gqugwzgox.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/goytqmqji.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gftioyuuc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gatjogvcn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gmrvoermj.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gksaswjkz.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gpsdbjxox.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gbhvtevon.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gujjmixow.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gygosdjsj.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gqcvxeezx.sHtML


<!-- 参考信息 -->