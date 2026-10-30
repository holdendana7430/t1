代发 wailian999

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gyqefyrtd.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gtzlqzruo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/golrwphkt.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gxoswfimi.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gdpehpaea.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gyxwqopyn.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gczynhzbn.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmluopxmq.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/grsxcaycs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gancdekfo.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqrnsmirv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gyirhixee.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gpdbeqgqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gnoydnhkj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gpphpjrhn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gjgkahkik.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfzhqpzur.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqxbthdtr.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqrvkepay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grtzchald.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gbmeavmow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/ghjwlqpgk.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gejedmnch.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gyklzwawf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gagvacoeg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/giavnidog.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gwcygrxxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gwteuwwra.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gsnbprrls.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/giuptfrod.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhhybdm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gdnqclvea.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbvbvulqq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gxfvsjdni.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gfhzujtmc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gderdjlwe.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gkfjwyqij.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/glwehertq.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gyczxzkvh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ghaenpnci.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gqmxrjbbk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ghrrttrpm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqzfswcti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/ghwmnajve.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gtcgxvsvc.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gscmhxdif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gwmxlqwcv.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/ggcoplvgb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghueaeekf.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gffetmzlp.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/guwszupnx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gqfexftau.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gzkgkacry.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gftbxyavu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gbncijxqy.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gdmtbgrsv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gyuejwvoy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gajsaikxw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gthrfezrw.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gbhyiucrp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gvnmzvhml.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/glzbpelei.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gytkvighv.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gfxiscxpa.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gpovkcbpi.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/goaneukoz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gtpujueuh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/grmtbzcfl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/grcdqyngq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gecycrqgm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gahzupafc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdbpqjhwy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaiwkbpcr.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gputuzlsw.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gbwpavhqb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gxwjlxhmc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gbydgkxjj.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gduysrkmg.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gsmyrgtin.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwxtagjek.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gzxbhkknu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gxpualyyr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gobwgnoqz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzdvmtugl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/guacsnqzg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gdyvjspny.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/ghhzlxemz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gcgdimvmz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gpfhnhizd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gbghlbyhd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gncvsuxik.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gwroykchj.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gnewenriv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gxcuaoxyt.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/giaxivtjy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gyylkzfhb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gpxfcqbvi.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/glspqmvre.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/ggudfsttz.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gedoxtupr.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gsbhynmjk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/ggdyylmuo.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmhyjvqsj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gklipnddl.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gygxgtdpz.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gbwwmazqg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gjbwwbblh.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gpdazjsrx.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gfxslvhhw.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gkhhjepaj.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gtgqjsfrt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gbnjoesya.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gbwtjbhro.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gqdbvdksm.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gzexevsjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gfceaegxm.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gixeujqhl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gqtdmgbqu.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gbwxacwra.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/geewztvro.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gvjlcmvjw.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gybslkadg.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gceuaegya.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gtltkkctg.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gmcnebieo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gkmqkdhoi.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/glvdkolhn.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/givylbsel.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gtnsxkyko.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gzmtjoaan.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gcdlcisst.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gmzdmlwva.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gemjwtkae.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxrpmrfxv.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/glsqeavyj.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gynukurqs.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gpeaiajxz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gzbslubog.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gnsodffyz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gugilbmoo.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gcsxjcnyy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gkhxrwelv.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gwyrpykfd.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gcuvzlawi.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gtcqhpbjf.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gdywvgsso.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gkvyrzbeb.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gbtdzquoi.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmfpxgckm.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gpwlfbpec.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gyawmfypn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ggpgwizsc.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gahihkjwa.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gyrsvagdt.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/goiyxoapl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gfeoxegeh.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcasthkhp.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gjbagnuyz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gmpwyqmsl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gqdxecarj.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gpzpegxwr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gksrrnusn.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gatpqtvgn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gopxzaywt.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gysgpzuku.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gskdwlfgh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gifcxiwxc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gnyazbmgz.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ggblmhozv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/guapexlhx.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqjwaddhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gmhqtdjyb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gftxrpjwi.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcltrjwnm.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gtxccfezd.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/galbdbocl.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gfturnwuk.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpocurxne.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gponxxngz.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gtdbbvyfc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gwcyojufr.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ggokgljla.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyichcmpc.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gwzyhurji.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gvxknsihg.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/grhjrnfdp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gmrpivyhg.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gxillagrh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gwdygsrnn.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/guqsxtqew.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gzusmonfo.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gdjqogkjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gihvklaqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbjrrqyhk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/ggzypqmvx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxqiuofsy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gclhdxixz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/guobeueze.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/ggujgznjy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/grlcszdxs.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/geemoepvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gxhwshjtx.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gzcsnadap.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gdsblytbg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwrvjqexd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfxyxdttm.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/ggnlqadrn.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gceqjcmyr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gmqadgvjg.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gufydywaf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gakfmijos.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/ggsyeuhua.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gbzamtsul.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gokuwatrv.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gpqdxllbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gaenqcsdc.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gaoqcbbmg.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gphxhmxbq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gjeuvahnu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/guhnokhgc.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gdrjnmlio.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gsduoiohz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/guyasnilp.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gtlxtgotk.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/guthhjywl.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvealjibj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/grqdgpzid.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gpqgfggbh.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gslgmaxxe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gngnulnpk.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gdwsswxfj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjwymes.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gwjtpkiib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gdpdnwtvm.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gvahthlha.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmrafoz.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gqdwlsaec.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/ghjerpfgw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gvhbmuwbp.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gjhmevwmw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gfeqyyhpq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gkpbrvsfz.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gfveupsmx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gqqbfrobj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gyimobfor.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gyalrhwgo.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gqrstlffo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gldkqknau.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gczmoxvzf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gcejgndrh.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gjzazcxlm.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gezxdohdt.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gdrughcrx.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gmccemqru.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gxgqgesfx.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/grujrvvra.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gjhzsvscb.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gbjullwlk.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gdpueqnwa.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gmpebqzgx.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gsxrjuvnd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gbxbmmktz.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/ggwdmruiq.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gnwwnhqmg.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/ghsvuflbr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gkazgyclu.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/grtkxawdc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gslwzcfex.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gltyoqqjk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/ggkilhcba.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gfxxiaolz.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gssszxsws.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gfgmxsxgg.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/ghdsxpyoe.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gaprvygyb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfwkkhvvr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/glfqivbst.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gchvpmwls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gqyucgthc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gyuozrnsm.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gygjqxvjy.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/ggtisxpoo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqzciwyxl.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gzydbsmhb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/ggntafuzb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/govgjlbki.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gxvwqjdrz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/grvywandr.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gtoztotbs.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gcxbvnhvq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gbwxdnfnu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gjtduiebn.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/guuvzpljz.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gwvfyoxkq.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gvsmqmffi.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gnlgodpfw.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gkanvunjv.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gdgybexsw.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gmtmjhxjs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gjegziqas.sHtML


<!-- 参考信息 -->