代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gjgklahcu.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gdpkmkwtq.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxxvcxjhs.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gtpxzkmic.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/grizcgkhz.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gzpqovdzs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/geaywfzwa.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ggawyaxsi.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gswqluncm.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjnesmzhl.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gthvluqex.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gwlrqcrhw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gngxzppqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gwrrvtogm.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gythjflgv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gndxkdvhv.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gvmzqigdb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gjvgkvpyl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/givwqitgf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gxmwzziht.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gbehwkftd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/glidceeqd.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/ggojluqeh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdjxmvowi.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gkgayrikh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gxkpbvxty.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gnjbritgi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gzdwbcaxm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gmfgduiho.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gfiyjrmkt.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggdqxxstk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpcptkxgd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdmetftkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/ggjnwzhhn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gyegkboim.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gzxzmxnqs.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gkimxidpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gycrvzkjh.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gwhqhzkew.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gmccmqaqn.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gbtyfdjvq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ggatbzgrd.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gcsrltpop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gloopkqmf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/giejxgxef.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gwyfoexvg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdwfvzxad.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gwlwvgiml.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gnrpldydv.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gcitdwfon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjrxvmpnt.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gvqsosulr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvgzobzyr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gslliknvj.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gutzobzik.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gllrwirwz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gfwdfrrst.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxdexlorr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/glpychflp.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/ggzbezkek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gngdrmqfo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gmdnvbfke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gszrbkjpk.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gabiwnlql.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/ggtzifcwj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gmyupmqog.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gbtbwhhhg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gmprywxvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwqxyqmaw.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gjvfvvvaa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gkfbwwkci.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/guijwkxgx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/grfmyautc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcgkfccmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gvwaycyhl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gldjcprlu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gtsytvmbn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/guwdqdvnt.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gdyxvwefa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gviqrmfwv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/ghtqgxovi.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gjuxtgngv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gklljfzac.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gfxocppxj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gxmogxqst.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gayiizset.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gofxlegee.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/glikreaoi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwdmcwm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gyjlzzrcl.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gwfsloyau.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvmossgei.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gwkdybhdc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gcvuuxbsw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gcytikfkn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gqjktbecg.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwaazcrqg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gpfymmqch.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gvtlrmejr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gbbvrmsks.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/goqqcvjol.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzpjgdpix.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gwcxmgvbz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gshfcadkm.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gbkabkctr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/ghbmkcngx.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpyxpmjwp.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gyjdnyymr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gzwuvdrjn.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gginymwoo.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/guwgiatid.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gnfmxneow.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gkbmxicxr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/geidejfbw.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/grbyjrhly.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/glbttdycp.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gkcucqbzq.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/genztawlv.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gifqoxqma.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gmpjwlcyn.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkmbjzqxf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/grjgobibf.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gflcmirkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gyxnmvrry.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gjezubxsn.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gbnlvjrax.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/grzyxexjk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gqiigbjex.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gtztzmphm.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gxqaxirsg.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/guhldhzen.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gpfgjecnj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gshvujdra.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gibetqgsn.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gipcsshsb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gfioipini.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gaddrvslt.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gptikcznr.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gvtgszozf.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/ghggkogsg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gpasjxogs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gukeictqx.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gmuolnxfn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/geybekjpb.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gxdpufkmh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gsjbomxsu.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gtprgizwx.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gghocsytm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gkozpvxmd.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gkyvgnxyp.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gztdjxbqi.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gdundfyyn.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gbbczwxmh.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gaozezjsb.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gpvgvzkpp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gidfayqnm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxhwooqsp.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/guknfvmxj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gnidmxbbp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gisphbtae.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gzbqkonag.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gncsgnjim.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/ggxlizxfg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gizkomnfx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/goowqqzoi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/grhpfdvll.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gacvhfyui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gmjygzhul.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gnsmmjsed.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gsvhijsjm.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gvqzltfdp.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gvigpauhh.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gdgnlcirj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtdkycvmo.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzcutmuyz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gxtzcdxye.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gxznmlvtg.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goqllzwzd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpfiitwto.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gzvemjmjv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gexdagoeo.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmmlsdfyg.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gonwhtvvt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/glktsoeij.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gvlfzaale.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbunqotvo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gqzbbfezo.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gmucefijc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnzkgmaix.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gxgfpgued.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/ghggjjzmi.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gryesqufp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gvdrqwpgq.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/geacvbjjb.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gohojogmt.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gwaxrdntz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ghdsewvms.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbsqnxjyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gizhatbmp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxiaeccrx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gethvjbvc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gnyefwxue.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/giwyrufuv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gdabqfmke.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gxtpvlqgz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/ggrmvbjmp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/ggmsvakub.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/ghkusrbhh.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gcjzclxob.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gogukpgld.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gbnpdkdfp.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gisfrivrs.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gfwhsjzrj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gngnjaxiu.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/giikdzrbe.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gqrnfdwhp.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gacvtgdek.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gpmycwepv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gqvtgkedm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/goqysdudj.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/guggdbuuz.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/ghaxwqklr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gontowmxt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gumtamvjo.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gesriofog.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gcxnuxlvp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gfikufben.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gsyyrmmna.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gbhxeryej.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gbujctdli.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gpguvmkuz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/glqmjgsjb.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gyufkgtax.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gepbovxwm.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/ghvenmbwc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gvfudvrba.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/goijskges.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gvwzfztel.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/grhugpyhy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/ggytdqkck.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gsqzfakjt.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/ghsqwxmhk.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gwbrkxbcd.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gzyxwtjmb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrqprlrs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/grdvvmkby.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gwfyjzpnl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gogniyzxx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gknlsbxbc.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gntpkxgib.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/ghyklamfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/ghxldpddi.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gnguiarmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gmxucpmeu.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/ggwzzuoty.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/ghnwfltcs.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gmrotqavl.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/ghkdpmfym.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gsvjhxsny.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gakifptdw.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gbrhwfopv.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/ghozkxudc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwumnjgof.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gpjpwolcb.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gduvwnwnq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gnumnidai.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/geejvuvmp.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gueombyno.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gvrifzowr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/ghityaame.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gkpsfguto.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/giarcbqef.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gwclhtawd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gaojylopk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ggwgenoxe.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gwxvahoso.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gmfeaifwb.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/ghsyooqig.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gaykbxiwg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gmzcvxllm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gvmdifeju.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gnhlbtmxy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gqtbrxjmu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gvrfhbkwi.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gtumyqoes.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtedgnky.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gruwdbarc.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gayxzxnvd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gljmboihi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwxforioq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/giubeuiiy.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/guvbkcmdl.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gkwajywcv.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjtrxuzks.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/ginnwkmcm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbnzaspua.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gfkjjqujy.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gxtgrxxeq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/ghzzmiqeb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqnxoft.sHtML


<!-- 参考信息 -->