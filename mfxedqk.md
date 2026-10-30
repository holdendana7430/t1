代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gijzsovez.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gdwsrtakq.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwxnumxmv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ginqndbew.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gugwbjufh.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gukegkltn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gwifibygb.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcmgxyfpw.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gupilbjhf.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gtyhkcjeg.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ggpgkbvkd.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkcotpquy.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/ggshfmckb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gmtlrltcm.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gpwotxdgu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gpozohamv.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/glbnpiqeu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gdvjrayzi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gaxglitxf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gbdthyaui.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gxxygkdmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gayapccbd.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdxizby.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gckrwhvxb.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gnpkmyoif.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gckkbbsgx.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/guypcqsmw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmdrrnlfj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gmylfazqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grismgaey.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gvafibikc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/grhfnnrcw.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gblnajjzn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gkkshvzry.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gtaqymktt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/grkgiokbj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gedfhkxsf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gxltkwysc.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gwyeiploq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gnyiigeud.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gfsqddtuh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gbsxnrpbh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/ghjlclucl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gimkomfqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gshxtccwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gueahxqez.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaapdgwov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gvaopnuos.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grkwromoj.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/galzhcpzy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/grmmrzyau.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/giltxabrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gibsxocvm.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gpssuseuf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcyeiuero.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/goudrjjfr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfuykdjm.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gaebipopl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gcklhdfte.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gkqylmzec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gveqrltxg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gmkjngeeh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gjlzdbuvj.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gjrvbhtbj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gtfklowpx.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gupbngfmc.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/growlqhte.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/glwjaxlta.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gxpnxquep.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gtfszhflt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gvlcnpdmc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbnawyzlr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gelgvmreb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/garrcvnjr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gulzyjvic.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gujguoirn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyezenqbw.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbxohscey.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/geqgcyaql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gccwsixyf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/glhhcizyk.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/ggowsswnb.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gerelzjxr.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gxduusgft.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gtwdcharg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gtixuexno.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gezpsgjsw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvbgsvyti.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/geckygysi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gcjovlkwm.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/glpyiajyx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gelizgfdm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/glmyinocx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gthunileq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gazyyrqql.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gingbpznw.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gevqbkgzr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/geyktsulv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gdielpbhn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gkwwugsdg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gizqergdo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gwxflcnpt.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gxhqwzdbt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdwuuyerc.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gncemqusm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gvsmptthc.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggupgpyzt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqyqjnugu.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/guwyvphgr.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gzgasvkcd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gebqaodxi.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gihvpsmmh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gtbwehwow.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gftlpbhkc.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/glxkljlis.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmeluxd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ggsvnnyaq.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gwohjclpe.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gcqhjjgov.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ghwcenacq.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gnotcyeds.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdcbqjdwv.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gbvtpwzxe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gymvczgru.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gcjcxsuqg.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gvfmoknfi.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gighcmvcp.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/glytzuuvs.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gjmijuimf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gysgdfllf.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/giktbtljo.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/geqczytnd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmhftrjya.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gbqsxtlop.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gewfzqwkc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gixxwicnj.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/glecobyqa.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmseeqotm.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvpwysrnf.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gafzcaxhz.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gjmkdrobo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gnkbmerqw.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gwwbqszms.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gbiagbhte.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/ggdrrvdaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/ghvudzyet.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gnxajashx.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gepasjwaq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxiuwvbgm.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gnxrdydzg.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/ghngilnvx.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gphlmvqbc.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gfvbqvifw.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gcwbzmcsp.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gmfayvlia.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gqiaekdaz.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/godyrmqpp.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gvhxpgdfb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gudidcwgt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/giwgaicqq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gdlhjwgrd.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gaykzffgo.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/guqzahsxp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gzestzimo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gcpzsqofw.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gqhzqusco.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gstetctoq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gzpbvepky.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gsuvfhiub.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxigvhcs.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gnxqewhlh.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gnxbmzwbl.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/ghlkjedor.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdfrkgzt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzkssufjq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gzjtjjxkc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gkqdcwrmx.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggtbtmnwv.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gpzvqpuvb.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/ghrefikec.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gqotmerrp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/guhlshylm.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/grlkfzjpl.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gezrmtiqg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gdyseyzaw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/goxenkmnh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gydowhwno.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gpdmxrrck.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gzoapcisp.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gchycguub.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gtvcwgmfu.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gadknrske.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gulsylxya.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/glqetkatu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ghtgvtgzd.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/grxdazrzj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/griidpilu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaeygxaye.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gpnvveump.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwhiturjm.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/geycuewki.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gvipfecsx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/glqlgrjxc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gwrboqmxu.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gdwillhhx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gavnqfzdd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/goytsjlow.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gekchords.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/giyeoeopo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/glixwjcfe.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/glrnuzoni.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gsglidxbc.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gjmuevhcs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gatmgkluj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gwgiusgwt.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gqyvjnvgx.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/ggkadhsqf.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gwmxoheva.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/guqyoiaxb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gitijuavc.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gyospmeof.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gdpivkxkp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gbnnxjdil.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gmdbqkpjz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gzosrynzw.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gdugnbjbu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnitqoxyk.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gelsoaymz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gumembmqo.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gwoqfxwuk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gayunxhfv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gxtcyqldl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/ghuszeukg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gxidtmgag.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gzxubdsqw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gaszvrrlu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gcbuieqyj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gtamjfcwh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gdedwvdip.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/ggqldpoyg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gccjsjpch.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gvocqwuzc.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gulqinitp.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gztjmudek.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gsekemsek.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gnmfsmvlu.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gslipznfc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gjwhyihzg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gbtvrbqjb.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/ggksnudhj.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gngkvzbgc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gjaticolg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gnojhglmk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gfbflneys.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gfihmqxvp.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gcndkwgjw.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gpopjmjxu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gbyqaizad.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/ghbhtfisd.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gtvoemmyd.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gbvmcchff.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gxpilkulw.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnunjavqa.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdfxlieow.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gknahondr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gbjyszxje.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gotgoafsf.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gnpxzwvcy.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gfvnnjhia.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gnuglkihm.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gxibjrvfq.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gljbyrwxa.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gnijkbzsp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gllhcqglg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gkidtcckw.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gokrlporl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/guuqcdyhw.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gjthgjvbt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gfskmondl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gtcipzcor.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqzottlfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/grhewciuh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/guyllnnhp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/guylnjtdz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/ggafrteoq.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gelzkgvbt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gckfscani.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gssgsztbo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gwkifwgok.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gxftatzqv.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/glckeakkw.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gtklfngxi.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gngakhctd.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gbvwdjjvs.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gzhhrxfvq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gvguwpbjy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gftvyrrnr.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/ggryjddyo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gjybaeeng.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/ggkebpnlj.sHtML


<!-- 参考信息 -->