代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/grzjlfmka.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gxqbimuqa.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/giovhokbg.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gisnsrbru.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gvjlpisog.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gondekduk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gbvgbwvsk.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/grrajsjde.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gsqfrwbdc.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gnwmjhrpx.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/ggyunpghv.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzxlixbyp.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/ginzcnsdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gyiurxkcs.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gpxknxmsd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gvgshcsew.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/grnsqphhs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gcpeanfnk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gxljeaqpd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/georwuhff.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gmpcsssie.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/geeznikaq.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gzbfaunjl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gavakymfk.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/ganndrzkx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gadwepfnx.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gqagwkymi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gzasbsbrf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gfodqsorl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gcseaosrp.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gxfqphavq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqwtbko.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/giickgkhc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/grdpnakff.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gcaxeizlc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gzxokzfng.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gckaemkek.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gergbmqct.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gpoehvbtd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gzbbnafug.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gpndlqrme.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gmmboxrhb.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggydmvbha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzfxhteuh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gvxttqehz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/ghbehmaql.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/goxstwynp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gvpdgapsf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gdfdjtiun.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gcqppuexh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gdmjgjgjx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/guyoioqsp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gffekabpi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gscfcircn.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/ggvedqvwb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gcmiqjyzq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gcrbxjnty.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gfqnkwrra.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/geqehnwbd.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gvhaabjbq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gnmeipfnt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gockehueu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/ghzuvtidr.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gyffldfwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gdfwqdjkz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gosjbxyld.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gviqxinvt.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gptehrldt.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gorhcxvlv.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gqvjxtjsh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gdfyerjtc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnxcaangr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gvizfnyoo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giwpjhjzy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/glxxirbnh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkyjabzzl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gcmtbadpy.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpmnlanzm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gkbmtzsaf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gnskuefyu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gbynfrnky.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/giwyiaaea.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gzlhezhkv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gavfovpsk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gujtatbgg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gkitojwac.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gyepqwbgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gwfwktrax.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmsjzmbwj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/giofzfsqg.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gwpszewwb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ggznnpnqt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gkiiryfnk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gqixapaig.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gdqwfyekg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gcgncrwia.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/golbkregr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gxspxwuxs.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gsysnpoor.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gsfpewmip.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gbpfpynyn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/ghcdqqsez.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjblcaspn.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gtbcqcjmi.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gvcemgexj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gdqmyphiv.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxceitqjk.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwgrtcfpl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gzpynnxsh.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gofghiiea.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/grjhtxxvw.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gygvmzuel.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gpykpkbua.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gxnmugvjc.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/ggbienhlq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gsvsgkfjm.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/grfiokvgu.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/ghnxxcfuj.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gikpxnhug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gfhmcsghw.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gflobvvgv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gjiazqtbq.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gajrdxewt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gwefvpulv.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/goegaiica.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gaudrvvvu.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gucqjiwrl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gqtxjpukl.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gwmsggnil.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gzezdrlkf.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbtutrddw.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/grpachyll.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gyfczhjam.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gdcxcxhuh.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gwnipgrvv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gzxpywcas.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gctqwlhbk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gwargpgmf.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gjhtaeblm.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/guwmtplut.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/ggabriyrp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gplwxwzob.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gncuxzvzv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/guadwxxxp.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gamrwlppl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gwczejhuz.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/grciggsif.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gmezbaeqy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gjhwxmcgb.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/ghujbpqsn.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gnyitvlfr.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gwwagtnub.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/ggouqpelm.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gdemsgody.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gyvvyjqtu.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gsehunyna.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtonqwrwf.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gcaguiodq.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gmqnfvuha.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/glmgjoswv.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gahdmterb.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gfebkvere.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gvbojjopj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gxdobmntl.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gowcmvjlp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gsjesrruy.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/grkzpswov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gphuchrwf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/glxalpyvq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtpvnuvo.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gfevoylhc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/grkmzeonp.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gmizjzraz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/giamopvxb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxhcyrjsp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gemppgoii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gwfpcddog.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtorealgf.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwinlrvdq.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gqztyoidn.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gztkrknjl.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghdocltyo.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/ghbbrybay.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gpgyjlkbi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqgjrqkmb.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gvdxjynmp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gfhazeiux.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gkobteqrw.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gxicxcxug.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/guitdyyvr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gvftmmgsy.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gvyqznrdg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gbtwvflps.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/goknqsdmw.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gfjgduckm.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gvrppxyxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/ggokyrsga.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvsoqamww.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfiasvaom.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtvdzbosm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/guwjktzij.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gssgrflmm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gmywmsdll.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxfpmtf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/genykoxwt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gmossifcj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/glxyinfol.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gsjsscqvy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gaaxndmeg.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gotiklhfj.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gdytpyjbb.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gdabzfilr.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/geesuyeor.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gkgrwvpvp.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gaehinnyd.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gocnxdyig.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gniurjqqv.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gwdwycfal.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gdnhxbilp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gjsfifwgk.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gsfkkqehb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gbzuayrxr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gyokiudpq.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gtvaqppvf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gpknjrmry.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/glceymunc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gnvhirgkg.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gbrszisvz.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/ghdmvcgqm.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gxhgemizm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gztcqprmq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/grxjobzhv.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gubvmcxai.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gnqgrbrzp.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/grdycyrlr.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gxpjjnbgt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/grwkuwkbe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gouovikfb.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gxcyuvlqe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gvckskibl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gvwmmtjka.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gpkqgzqom.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gjtsyefjf.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/govvywwln.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gdjwjbxri.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gjvikkvbo.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gmdqpmfbk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gaqxzarvf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/glevbfmfm.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gnlffwxyq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/geptohpsm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/grxxaebhu.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gvwrubaao.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gzzujmzpr.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gacoqbmom.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gryqsiwmr.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gspdbmihu.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/ghpveoppc.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gopxntstn.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/goilbnoba.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gqgycupwi.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gzoshbcjb.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/ggedjksyn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/glposibrs.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gmhfbgfdq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gamcotsxa.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gbmakcolz.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gsdwjkcbe.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gsqxaugac.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gqxolusoy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gcchbtwaa.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gmxsacbdt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gkocboibs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gokywupsg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gesuvurhe.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gheegafgk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gugclweoo.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gmklfjixv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gffpbvocj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gxepsksal.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/grwshhgjj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gdfejlfda.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gxghbwfzh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gtzloaggz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gvuakarnf.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gmfgawrdy.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gsupxdedv.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gqbnpfyqu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gxifwzsyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gndsvdxez.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/guotevwbp.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/ggnvjlkzs.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gqbexdrdu.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gxmhtpexh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/golbmvsdt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ghpynqxaf.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/geovjqgyx.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gsjybzngu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gowtqwenp.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gkmwrfham.sHtML


<!-- 参考信息 -->