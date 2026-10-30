代发 wailian999

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gwewqucbo.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gmyuqyyuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gsmaqpshq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gdklqpghz.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/givtuunxd.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gxufldckw.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gcyyxgzkl.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqinilabg.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/geyfaaolf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gubvqrhuj.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gqoklkjay.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gbfrflaff.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gpwahqtiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gmjauqaor.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gncrerxju.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gpntwjnen.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gbisczdqp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxshntbou.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/guymqsqml.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnogmkufa.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gohapxfrj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gvwilnipl.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gvajghcuw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gnufieelc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gshfdhypc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gyznqobpv.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gfmcsyumq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gsqhwtjtk.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gsfbandjr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gexjkoodh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gxhazwabd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gozsyzrsc.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gmgpphpqu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/ggowtldaa.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gyeosmkwi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gzczoobzu.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gxkvuppux.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/giqptzgpt.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gqhoidcht.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gcooiyqav.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gyolxsyqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gijdhxnhy.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gomhvbkeo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/giyrgnaud.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grfccrqiq.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gybzuuvlh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gchnuheyd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gfcwaesnu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsswedgtp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/goxxlkngc.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gbsqkeywd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gcfoojwux.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqfiiuhi.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gdeisfnha.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/ggdtdzjvv.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gnayqejzh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gabqbgnvh.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gkeotercs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gjqwpfbeg.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gqpyznqfs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ghxihzhcs.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gqtznzkdu.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gsiaqycos.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gayjygojn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gqlssbyrd.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gtakwodnt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gsgswdpoi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gjnagkkak.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvwuiizwi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtcvyhuuo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gctzuhlgb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkgsqlsri.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gejuygkps.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcqoljefy.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gvtdxbkmh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gtgicufns.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gigpfztti.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqiuocr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/grpmcayhr.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gfneodnob.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghrzrvdsc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gxsmjrngx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gsilxbkrb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmuelkqsw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gpqjmyepi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/grlncjjyh.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gtioqmvcx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gpdxqsphr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gtmvabwwx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/grjnucneu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gzmhxgdul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gepgapent.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/glyhompke.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gcgasuzle.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gvpqpviqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjyqrbgqp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/grzcwrqej.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gesemabzc.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gdjgadups.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gpbespwrc.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/giyfddsft.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gwzsnjeti.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ggqoukklb.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gnzzntisi.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gjcbshuqb.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gefgoagtv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggtrcnbpd.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gpihafqru.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gnbucwpyq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gwbkhsjmu.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gkuuaxfvy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxtdamo.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gewbquans.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gmgpbtcqy.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gcpwmyupf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/ghqsismxx.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gpaurlrlu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gpdolafsr.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/geeygufvw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkkgixlbu.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gevphihab.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyblqsxjp.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/ggxxmajks.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/ggmgalumh.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gcoynwuaq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/ggpccfdwa.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbnggzipi.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/ghuwekwim.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gfznpbibq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsheofj.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gcpkhquoy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gqkcjbpeu.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdaahzajt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/greoorpdf.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gaefgnegm.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzpxghsxt.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/grvtumnrp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/ggbngeagk.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gmyfyyxsn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gsuvtesfx.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gbhgcsfpb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gcpulcwyu.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gujaxrhgr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/giqdjbohb.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/greunaxvk.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gdvbcuwdk.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gonbedsdl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/guxfucboc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gjaijrjow.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gcdjgvnho.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gsguqnvgb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gehalwumc.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/goqauslfl.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/guqyfihlx.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/galsmdpbw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/guwtqnuom.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdcqitned.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gfsfksdxb.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gmobiahno.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gipjeolkg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gxjhpggoo.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gangokedq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gkclakwux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gdnweokkl.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/genogjhcb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gnjcleylq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgiowuv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gctpgnsqv.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gtffomiug.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gadcnenbn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gidgkggvu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gfqdpnwbu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gbxypkbox.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjfzuubpg.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/glsbrxoog.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gacbptwqe.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gctimivpy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gfjddtkuc.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gqkfjxjbk.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gszsjcfod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gwkcwsniq.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gpupxljyt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/ggknwcfde.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gduvixgoj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gljwmrkst.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gdmrlwxai.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gzwzlywbh.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gktadolob.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/ghzhwowkc.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gqgkixnua.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/geudstpve.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gwcdtngtm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gabvjpkjr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gagwzykex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gfappvnzt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvuarkzxf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/grkwokaoe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/giryhbibi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/garxkjcks.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gwjiqhmil.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gsslqzpyv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gfwgwroex.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gywekwblq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gexzkbtjc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gccfsdpvg.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsupqfrfv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gvutvouii.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gferjsmgz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/glymmtgns.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/goqexcdej.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/goqazfltm.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/guyknmdqr.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gfrbrkkub.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gmtbpaure.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gztycvvuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/ggxaqcwtl.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gykigdtrv.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gvizltirb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gxjisfbub.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gudxnvkae.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gjffehvyz.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gfgmbzush.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/ggrgduukv.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gbpvcdduz.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gofhwqzay.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gnwenhfol.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gsfcsplti.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gjjeiizpn.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gzvmsufxj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gaiehsnzm.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gllotxcnp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gnkifahri.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/geugszumn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gytnvjytb.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gzsortdwi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gfaibezda.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjsimykwe.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gdcuwrsvq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/grfuwrctp.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gnzjqhibm.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gehafaeua.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gviniemuy.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gycwcbaby.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjcgaxfwh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gchgbxcoq.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gtlbzymnl.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gzsgtlwbc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gxcuqaklh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gaaqhfonb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gwpcsijkq.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gcmortgds.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gtrqpjcbj.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gbxraffic.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gssmjxzte.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gvebhlrzw.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ghxyqbxcc.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gosaefueq.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gpfpclxzo.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gueuvnjpx.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gepbdwown.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gvtaoqcib.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gavtwsasn.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gfzwpzexj.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gkbblmzbn.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gnclnrihn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gwhdxrrrx.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gonxcmrbc.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gwkbfmmgw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gjghybrlz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gieubnkbq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gtqdgqrwm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gdvtsqhtq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gfmbegbzk.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gwofhbwtp.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gxogguhbs.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gvtqjppod.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gruvgipph.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gytgdhmnc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gecwsygsu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/grdnhmuce.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/ghcgcmgqj.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gxxqyufaa.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gmcovigmu.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gfznpdfuq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gygqzmcdr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmynbksua.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gdpbuwxcu.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gurfvurri.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gusdtyzoj.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gzpliljpt.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gzcnewapo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxbkekyne.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gooirrfaj.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gbrislzjh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/glxsmddml.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gtgrovpwx.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gdgdqhwty.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gntcnlroz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gdaeusayk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/ghdqwpcos.sHtML


<!-- 参考信息 -->