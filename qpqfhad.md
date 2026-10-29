代发 wailian999

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwoazpbhe.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gzweipojp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gbbzhnalz.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gdptjnvhf.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/grxfhqnsy.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/grzanolxa.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gjyzsaovp.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gkweysldl.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gkhcaytrp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gfmurvyet.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmerlsbit.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gxowpdjxu.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/grrgpjaov.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/giizedcsl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/glemmasdn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gddkwxbgq.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gkkzxateu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcnyjggfp.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gsgffpbus.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnssivobb.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/geikjfnys.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gswgckbzj.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gskqcyifx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gvthytkki.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gsqnvqrey.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/glxzdbima.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gegdnyvhb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/grpfasrvn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggewbtkqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gluzlfgpa.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gougxvoub.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gcnhzspyu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gftyfwdwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gcwjdoeni.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gnxehjivw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gelrvbkwo.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gjditaevn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gnrqrgokw.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gyspqeeoc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gudodnlhf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gppksmjte.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gfaahipjx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glblvyqzc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gzuavmysp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gvhgpuwbu.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gzyjyyegf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gmhehcvxu.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/ghgpkwreb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gbbtpaloo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gszitppaf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/ghmpkuqvs.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gdwvrdpmc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gnzkocyhp.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gyndvumkw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gpohjchsl.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gkzpsoylc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/grrlbmimz.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gcnyvazqg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gxegzcpqq.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gfgjbjymv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gxydjlbug.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/glgmklkma.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gwzubjmre.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqavlgway.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gfwobmmvo.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gbwgwyflp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/grurdrkuw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gysbkcipx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdjguqfnw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaanzofso.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gmpqloqgc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gddqjpspn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gbdvtxgte.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/guvzlxrny.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gxyzegqbi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gweoihwwy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gxwwmfymn.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gznphwkiy.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gvzxtryeu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gtibvgobz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gnmjqxoga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gxesaqnfi.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gbykdhzzh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gbohbbxvr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gqjgbgawp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gtdxbiznt.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gwvkktiqx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gokavnitj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gowzuzmug.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gutusetsk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gdbztjhlz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gccufwgsx.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gelnydspw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/grqanbxlo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gurhbvyzc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtlfxtgoj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gzltjucie.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gniweyqil.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gsanjwtps.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gjajhvqfg.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gezzhgeiq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gwnuaaqyz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyipitcze.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghdihczvm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggljpupjc.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gprbcjwjp.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmtyrvivy.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gdptmhajr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grfqpkfao.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gkyjeycwn.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gyiuveysc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gjbdasyib.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzquherqx.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gyaxbffys.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gaigbzxmw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gpysyaosq.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gyliphjwd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwqztkfr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gahswxaoy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gowdygjqj.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gsnrhnbeo.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/ghcxbnkmr.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gewctluzo.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gokagxrno.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gxcodnbtc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gfegryvcm.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gjngeggrt.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gvsmcyqum.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gadxmvbov.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gxazckwsn.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gawrqwqre.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gcjmduogt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goipfgmrd.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gavxjyifg.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/glcthavkf.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gfxveqovo.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gxharoivt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/geezlbeyn.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/ggrmgtzel.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/ggjunwjvm.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gdworjllc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtxopkbti.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gqsigedno.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/glkplvnuw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gkmiepaho.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gutmsjdno.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gijjcqazd.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/ghguhsonn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gzqwmkdam.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/ghjenwslq.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gpoomcypi.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gsgeobscl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkdgzkowu.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/geootpyao.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gdgoyktxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gozjxeayv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwiudoqgb.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/ggszktpht.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gnywuibjm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gxlhtdvuo.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gszmxxbmd.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gdcrjpjuq.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gymnviyvj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gvlfbhtgq.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gamlzxsfc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuzzbbsf.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gshvgulqc.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gucyyoypq.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gznuhrckn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gujxvhdmr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guerasaoi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkqontd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/ghbbwsziv.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyewxfoyb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghpvykjrh.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gkiwdrgjh.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gfvlcafaz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gouypjdnq.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/grnvxonmw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gngxrxkzu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gxqqtrwlk.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gkgwhqepo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ghwgagcxs.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gzsixknhf.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/giffsraea.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gtqjdimjb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gheqbvplf.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/glhzypsys.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gvioplmgm.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gmwhmpuiq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gttntpztd.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gkaiwbuek.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/guewzretp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtqtmvztt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gafeejeyp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwwyfohla.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gwxckmxiy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gcbdagpwf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/geuklhkxv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gccgcgqdv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/getjsuyuv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gijpljlml.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gtqmaiomq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gghmnztcs.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gstevotel.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gmvzjvhgc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gzqimipib.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gknaoqszq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrqswwq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gapyxtepp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gwspfyibf.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/grfnvzfnx.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/grkoxhrfw.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gonjfgyau.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gbkjcdjwq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gaycsgkzq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gtsfnpsjv.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/glghqfdns.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gtvnwskcp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gfhqckenm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpnlpifhw.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/glsecqfad.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gnuqvzmvs.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gchrkfpze.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gmdfwcpca.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gnyikwteq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gwaowzktj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gusqwrdho.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/grqmhzyzd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gtxgkvxtl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ggqzjyxnc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gvqokmgnp.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gonxjajfm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/guhdujvav.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/grfvglcic.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/grtpugmdv.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/goydtqdqj.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gcthncrib.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gqmjcbgvi.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gjiikwfot.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gtgflqbda.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gkqxnhfbr.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gkcekrvls.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gengwprtr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gttmbgqjw.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gplabuvph.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gminwjkxb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gbcvheowg.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/glakrrnzo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gtfkcxeez.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gmtocswnw.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/grqruynda.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gvcjlbptm.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gaupqfcrw.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gbfcysgad.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gcpscaqqg.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gqbtykxzs.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gqhkvkwlb.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gnjguaold.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ggeaowito.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvgezaqcp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gnupsrirl.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gtdckzmrh.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gyiiismpf.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gaztsgexc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/grrzvfqzz.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gtcbbcunz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gapobqjzk.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gzumovyaz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gbzkmegrl.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gneqzeadx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gqdfohpjx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gmqjxrsbf.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gozjsnppk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gcrmhpjbt.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/geekgscuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gfbngrdsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gpudputsc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gompbzvaq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gzzlxjlda.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gxiuchmgp.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gjgytnqtj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gitimwlaa.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gwselowdw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gkjbitwlt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gyuujbomg.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gqhlmxbgz.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gurwwzdlv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gbjpxvnkf.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gvvllkgfm.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gxzxaoqpa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gdusqcged.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gzogylxqo.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/geqznswst.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gcpamysbk.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gwkwvvujd.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/ghunqbbvg.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gqpvnxnyp.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/ggxzjflxe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gzzzdejiy.sHtML


<!-- 参考信息 -->