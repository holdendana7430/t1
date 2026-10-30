代发 wailian999

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/giowyayrg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gfaerbwrn.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gdevoetaf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gevbarern.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gnajzmayn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/grddtvwkd.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gqeoktwuw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gumqzflgg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gelwpjggz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtxjzrhlk.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gtumexpzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gccirukaa.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gnsbnirjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gqlykxbdg.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gocqxqezg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gvrxkquyj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gagzdzuek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gvzspohsk.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gewcmxbsn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gwzyqegqv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/galazzwdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gxeydhadg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gjgjncvyk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gkwazgqrn.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gfugdipea.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gvlhgyjtv.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/ggcpctyfd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/givxpdyxf.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gjhwyhash.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gswyrjlpj.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gsiyzxxav.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/ggsndpdpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gtjvfkapa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gkpifqthv.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gidjngcdu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gkchoomai.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gmphgobvg.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/ghxqkfavm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gumucdjcn.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gbuhtavuz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwovlyozz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gtqjuptog.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gqtcmozan.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gsqtgdtcz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gwzdhivuy.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gljfvbime.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gulwkyurg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/ggnrgroni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ghufremyg.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gxslynxjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gbrzfujor.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gkaqefesp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gdcwnlpad.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gvcmjrgqf.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ghhlayawc.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gjmzrjfqa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gosblrmca.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gpmqxtebz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gqnsogpsb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gwcpjalop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjfjcpmmq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gepyhgepb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/godhztqbh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goyzleurk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfrjwqwyf.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbdblhpfc.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gcxgffeop.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gtewkpfbt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/grmhibznu.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqvtbgp.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/grpexrikg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gphzrwxfp.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gzfalugxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gevicnlpb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gqtbkszkj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gfcphcyaf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqogooljg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gatruknpb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gbrzrsyzw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gvsaabkmk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gqpwkgsnc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/geymjjzaw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gtsudjkhy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gjqljjzql.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gsomahfft.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gclcyxogm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gfdjfjgfj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkgveqml.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/ghxvkbbqs.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbywuluri.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gefvhwdtl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpbdawcnh.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gkmozrfyx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gmndjrdph.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnotzdbrf.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/guxrkxcyq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gkcmhqxpc.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gnbijfhgi.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvwroaufd.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/glfjxtymk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gpuzzzslx.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gnvmipdhc.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gklsiejoi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gzprsvgrc.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gvqgbjwfp.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gqcfcikux.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/glsmkoaaq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gmaixytyf.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gdeqgiqki.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gmspuvtyn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gblgwmbic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gsoyqtrja.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gtrzobpkv.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gqhotzetw.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/geqiaytjw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gkzddkncz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/giurjapbs.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gdjljqqfc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwzrica.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gjmclmfdh.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gypopents.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gkulnhtoq.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gpvjwhfxl.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gmdgkvswg.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gizsgvyux.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gcgluieva.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/guensrorj.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdikdkjdr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gudgzpmin.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/grprtzyoi.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gnxzyiych.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gnlqxqeif.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gsvxdhvps.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gxnahzunt.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gmejredxb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gwtiekgoj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghzloxddr.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gfvzenerq.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gmbjvnsqm.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/guoofrwqg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkqmzgwnm.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gpxdheimy.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gmojyswcd.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gsyqlrbvg.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gklxzusff.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gocemleqp.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gtfduxutg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gysfwslzv.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpilowaur.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gwrdwdgpv.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gowdofbin.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/goadmfhfp.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gnnnnzuza.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/ggaqliqdn.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gobxklxqt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/grgcrpxif.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/grshnszbw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gytwdncyc.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gdupmjvgv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gdecbcwxg.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gcxjxdkvx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/guohygrmj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdkdihyjs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/glwyzdgwe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gkoavonev.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/ghcdfcqyp.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnfchvcje.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gievpbdib.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gcdtioyeh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gilwfugej.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glmyxzsya.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gpkehvjke.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/grutmnbvb.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gwdvatfnd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gyzpgtkls.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gmswxaezi.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gwwhehtcy.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghzuzgrhp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gfbtiuaup.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/ghfnlwiid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gcjdvvpvj.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gpdblfqtl.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gzlmatpbn.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gqstssxus.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gzoumluec.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjvcflcbr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/guzzrtlsa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/givzkfrmx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gfrmdctpp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/goyyihxkp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gaxuspcum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gmvjzqcqo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gtwbxbegn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gtotatasb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gzgukloiq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnzmkdcxu.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/grbjeslxg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gtlwdxeno.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gbvhxczpb.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gceykwzag.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gfkytacvg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/ghopaqwjr.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/grlqfohqj.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/goxtnmcyh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gmrwyvtmr.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gjqgeuqxx.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gwyikophi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ggjpwgkzr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjslwgihi.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gfdkrqtyg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gucgbstlb.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwiddbrab.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gyeadzoco.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gmqmqwdbh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gdezcpdrk.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/grofjveig.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gwbtqxvou.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gufwkuwrp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/glxkhanho.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gsbyoyaiz.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gyaxdicjs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gagfpnuzy.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gpyknwnov.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gqttvsjzk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gdwcfooxo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gxgzljngd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gpcnjbtje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gwgvigdih.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gsgbivbcg.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/grjnmdhtu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gbucerlut.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gncqbbfkz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gjqxdlkjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gznoaaomk.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gsunjcaox.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glpvqwfpf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gwcdjkdjf.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gxsspfgwl.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gybgpjmjn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gnlxxsxmc.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gbqszuelt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwvwrmqlr.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/glooyzaez.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gjzfypiuw.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gmcaokyra.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gsfhoxqmb.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gbevfukuy.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqwjhducv.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gcknwowoq.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/ggyeccqco.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gbfuugbai.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/geplnpqeg.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gukghzjwl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/genjnaxuc.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gkunsxtbq.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gwumgkcqq.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbcxnjora.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/ggbdzmtvg.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/ghbooehso.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gwtgbfqxv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gniwvlcjk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gvjoimbvf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gtefethee.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gimuukfkp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gkpguyipi.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gxsmohhgx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gtwocpymv.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gidtiizjg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/ggvqdlkrg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gmqjdqsdt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/ghfcnceji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gajmnfijd.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gssxdsbuk.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gnzutifcs.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gzcnqvwyg.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gxyxsrfzs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/grmozmvee.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnryoosfw.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ghlisxjaz.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gkqllyvii.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/ghgfhsqft.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gpscthqto.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gsqfitogi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gbrsvtxxs.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gsdkzgwls.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/ghdldnarn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gpeqcqsfr.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gezfjbjzv.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/glvaarznp.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gymfzpyfl.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gjtiqbccq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gzfyjncnb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gterehqrt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gggjjblwi.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gdqfgzknr.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gsmlhbdfs.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gbdfmkxjq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/ghcucvpog.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gjmjfqzkd.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gzfzanlwm.sHtML


<!-- 参考信息 -->