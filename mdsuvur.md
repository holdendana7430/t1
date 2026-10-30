代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxzzmnyij.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gehpfhzcv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvwbymed.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grqhaxdhz.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxravswpc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggipmfihi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbysoqbhg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffbbqowk.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gqmupugca.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gmkiixxas.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrdaokpo.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyzpokcic.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfufuorrm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhbovjmk.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsdrtrafp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galwlzlxa.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzoueiac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcrcfrdi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpfyefrw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzjpraqd.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gztlcfwqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcoeypsam.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gipabmjat.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gslypayvj.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvlyocs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrtponxr.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtcklkmcg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghgevksyq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufhqvez.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeabwnyx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxrcuyhuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjurftdi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeeqmfjv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcfscbwr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxskmkmnk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfvtewnf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuwkavlj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnaaxyco.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrmtsmp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glnsyjpws.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvuhbdgs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gelvkqpog.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmquitnk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpupaxxun.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxziwzkez.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhzbuvnn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkblvkbdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqmuhlgs.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsabjahh.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gozlwckhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gzfojxgub.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxubkdsdi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmfmuwyx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gutnotgyh.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghppygtbg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gqerowpsl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqidnru.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/giestvacg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/grlsevhyp.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxrumyhn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrclffpp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdidcdf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrygsusf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/grguvxcqk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxacovvir.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/giqjnuvgt.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwqskpbf.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gseygbbuw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkkvjqjr.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grgyhbwfd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/giohfglua.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkapzujo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gffrpaxgt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwbnamvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrchqtgc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/girkbveac.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojmiyhvx.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gldyvnnmi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvpizlsq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gznrupdrx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gutrwimgv.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjedkwtsl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gpskppvvt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gocuksiye.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gyycydhtq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetafgvm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gryzcxxuw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcivgaje.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glsyeyhcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzgdwjmvd.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gwntsenbd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gtbbbyedu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmzcwvuh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/glwewvrjd.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/giaxlhvlr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggacphgee.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gqscerygy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhptatia.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gdoryequn.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grdhpzrxe.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimkuwiz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqqfnsjw.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtbzcsahu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghximlcfy.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gcagtzyba.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdjpdipn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqyosvxo.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaiafsar.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkrbbijeu.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtbdpijjq.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gssnwjolg.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvgkcwx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqgqhlce.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/geedxnvpv.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gshalscli.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzftqil.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glzocivlp.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsicmvrie.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqttmsqii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoijbnph.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpsrrqdw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpdxwyct.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevtxqmcm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpemukyb.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/govynxqqh.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnemgrdoc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpwnloyy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmpkuxwh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblxeahie.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmfjfdxr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/guzsjrytp.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyitoxxg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gxakdyevy.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcmhltjz.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gzvamdcwt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrphlejv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaxwlvwp.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/golcphglp.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnqeibbzh.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gezjurdzl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbkrxtee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcghhxxd.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrskthlq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/glkhtfgxo.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gritmrszt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymvmezg.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/grlxjbwwa.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/guplswcfc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdqevnaj.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrrtedjx.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxxvbaqse.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gksleboar.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gklnlakef.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfafrdcxx.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gufvmfplo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjawkrdm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrghzayn.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gubzohzpr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqdwchjl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnsygeix.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzotuxq.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gawkdaudv.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtckqsqkr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/govyzldte.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmacidma.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqnkluwz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gifowqtsm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbauzlsv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnjswxis.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqgklbgd.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmlfbgvx.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gklhzxcjl.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbxfjdtas.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhbejdkq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyopuastm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeveexqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoxtsqao.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyybeuhfq.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gedgqlhvr.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gemfjleoa.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnndpknba.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaeepter.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grwsrujvw.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdiakjbm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndiotqvk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gszbbepus.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmfadbvqy.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbkybyza.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gsbfsjvpy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimqjivu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlfijpkd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaqnfdgh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/glxjtlrbk.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlcydppr.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypviyqjy.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gvuussvjp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqvuaerr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwyesxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfkppevdx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnanwkmcp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhmkzruc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzbifgnyr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gvyuhcqsc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlhyiwtj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwnnqwfuw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjgwzav.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gvrkhzwhr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoytwepp.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnehjfrs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gcerfdwyu.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gseznmfxl.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/grvfnmxta.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaqfetaz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gdacztclu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzfnwuxv.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gecwraduw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsamnblw.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpusnrw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiusmqec.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbymouab.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkuwnmk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflcpjqb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauqarhbd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftctjcw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvwavbb.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtuwcmbj.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcktfjubg.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gomdwmovh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpgdvlfh.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkvrgtoz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gkissuihz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gyvxprzfc.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gircwowgn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzopeetls.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gozbwrmgv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gepinhjie.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gubpsvoss.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymvcpiik.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gsdlqmisp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdunyycu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljpsqzb.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gzccoomzz.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsjijvlh.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghshovxam.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcgjheo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/grntnnmkd.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxmxsdlnb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glzdwmefe.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfrzjpip.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gppqcbgep.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gbzptugku.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmhubwyk.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymuthnp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqceemm.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gvrtayndh.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gehtudcde.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzxwvsk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkubawnr.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gktoimhmq.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrsuiub.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvhclypj.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gmocfsqni.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwufiugwp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gpvobmcrs.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvpuwxe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokvluhjj.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdolkhcet.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvqccxey.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulbkpix.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjmnbpgl.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzaspvneh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsufyndl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gantgghnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrnvsoym.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ggoxfckgu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotfjozq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gypjnqzsv.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/giocelefp.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/guxyhzufm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgofgrih.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzglknp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxcphvjg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/ghamckuwn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/graevromj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsfpqztq.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goztzwygu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ginvgtueh.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgplgvtv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlzcibwq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaksvelnt.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gytrrnayo.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gvfpxizpg.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrohfdop.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpufxpaxy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjgomlxi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvlgjuji.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckkcydhd.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gqibrimti.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyfyjysp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grxpigdzs.sHtML


<!-- 参考信息 -->