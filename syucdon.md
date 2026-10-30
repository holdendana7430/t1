代发 wailian999

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyynmsbi.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gslrrriaa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gggemnoqv.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gzfhjxlwb.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuewbnke.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gizydjnts.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsxdgoxx.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyqxmwsdp.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gotisuyrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyiktmxvj.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghhaekfkv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gfoczoqhl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvtcyezb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvftwkoz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnqvwssa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlgnciix.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gieevddtg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjqqfjnj.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdngmbovy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwozxtakp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gtsjqnbcs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/geumqphqu.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrwwpsto.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvwzmaji.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqkfuuxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejgfudcf.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gahvglycx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiyyuxqu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiniwjzv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gawiayuvz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycjatkd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gzmzoupon.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gzdpfaiei.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcstxij.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gmjqhzcjy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gypkauigx.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlohnofd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsxcvwfu.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gkcjwoenf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gevelxtxp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grawyxqwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexzotitx.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdmlfyfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grklupeow.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijzrdunp.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/geijyjrte.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gqqktbgxd.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpeyjelyg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzrbuvd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmmflrh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gteytooxt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqeoicpg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzyittof.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gmwfkutsd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqnusttn.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gbigfhugo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcwdnzow.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gvtuzmsrc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/guuoxbhtn.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gsggbdtqc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufdzokfi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtyngqdl.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhagtepk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrgdsmxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqqvgeyv.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ghggiipyt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzflgpqt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmxbdhxc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gcdgukoda.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnehpalvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaalcnluj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmybbtnwc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gftfpttqa.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkevaoume.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfbwyxbs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/giawosgtt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gotupqhwh.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdmvfyyt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzdgzrwq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/glaejmsay.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocwxzhhp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjukaoqe.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykowfkgd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepvwjhye.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmwrkha.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcqbfzaks.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqapltpjr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsntfywfl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvockoq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcchwfhht.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwcdpwf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/glxljlgph.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnegvzbk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmebaqcy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gragtwxjj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwhxfldc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/galrvxlkw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxjbcmfx.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gialoykgi.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhtclus.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjksyldm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyrqlklp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjykesgiz.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gidaghxuv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnlbrjnp.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/giotuylhg.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gouctqqop.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggommepwr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgsbjjz.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/guxxqmvlr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdvmwzrj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gasyzrign.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gzvjsuukg.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfzkksos.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/glxgnroth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geywlprjj.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkseyiqcj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqnmofcu.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gbeecwikl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glbjsqyux.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvsovdy.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gfrhahxzp.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrdgwqwi.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gqtxlpihv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxqumux.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdpxjtja.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gsukjlqhn.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbgirtmf.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gsgpgaymv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjificeb.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvbusehs.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfzhkltv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzxzpyrk.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmofwwqpk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtcsvckd.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glddrxrwj.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gxgwaobxk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gfwxuzzap.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkbupgzj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gelzqcqnk.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gejvluorj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggietdfln.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpoxgduw.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gqbkllthp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/giommizyg.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggoyhjqde.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaldyydx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbfpxqf.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghonwuetc.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gngbxyvpi.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdikbpb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gokvdcska.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfettzz.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhsgmmov.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvvefvkyk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzrvwery.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guerwaltt.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrhburmj.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggybvrsmn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/griogywfu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkztgds.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgvwwycf.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghsypqyln.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnqnsvrjq.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gllvdokso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiddpvtd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvloxqjo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajwbrsfk.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxeiuuomn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grafxjppc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxwikbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqmukegv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxwemgapf.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgbbbeza.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwrcijluu.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbexirq.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjwvbaqv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzhkrxdl.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/grhagkhii.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzxmfamr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guowqfian.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeoflnsf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gansdgqng.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmgplbwl.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/grknopltx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghwlxhokr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbvwckuy.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gcttphnsv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gevqgahjx.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/guyqnydac.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gipmlpgua.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/golhkborv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybnbjya.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggkstsuwx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbetpkgbo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwdjnmsw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixzvjfyj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gvroatuqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxcicxqh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqdidqlpg.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gszmtwmet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmwpjkesn.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesulxzq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/guwkshrgn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobqzqxf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvgdvysr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzagyyfgp.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqskwbnvq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gyjjnkeoh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gxcqnotxw.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/guczjgzrd.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gelqiuvjf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gyusggtsu.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gipgwegxm.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpxtskts.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsuhwnxd.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gibecjchj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpljrvee.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzfjkwsah.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgcyrrda.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfsvgviv.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjrwric.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gentisodg.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgcwghmr.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/guqetjanq.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gqkeqtjwj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gydkzfeau.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgxykxic.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymtwrdc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gppyaiorv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqvykgss.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/glkzaxoop.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/ggvnhqdte.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohapyuw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiztwebn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvprqaax.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gzemniyih.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gipeqvzcy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhvdsljd.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscplgumw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkimrxlec.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gsrpltrbq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloukcten.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcudrzeau.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gqrinxhlg.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gdkgnmjvo.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajwnosg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjicifdw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gragbazdh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gbixhugxd.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/ghvfnbonk.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gfuepadpd.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gmmriusrh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhiqxla.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojnncndz.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjwtmesb.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzouesnn.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gneqboxfe.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbiazfb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbywdsz.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/geinwbhsu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gqteyphkz.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxffvyudz.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/glldbqjjo.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gkkluikwq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gilluduou.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grchnhzuw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gimxgpmkh.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/guohwdwzy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/grrxglmsc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbcmqfqj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqllyyqo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzacwrfmy.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwiexwm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/guydquljj.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcctywwh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpqieuhl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/glhnwbkja.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gnxzpuysj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ginyttpwz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfujafqb.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtktfaue.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gspeushbm.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnejgepsr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkuizjq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtpmnggm.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgmcvryz.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktwjwfsc.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbxaywrd.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gqttgcwwf.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gyipmbvdg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gftjhturm.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gaigahurz.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gyinpuyea.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gqinvswtz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbolctja.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/geeskkclx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvygmdms.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqqqrfkce.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwfrjrsu.sHtML


<!-- 参考信息 -->